---
title: Microcontroller Code
---

## Overview

The code is set to toggle an LED back and forth on pin RF3 and use a speaker when receiving an input. How this is done is this board recieves a digital input from the main board and receives in pin RD6, then I run a DAC (Digital to Analog Conversion) and output an analog signal to pin RA2. I then have a square wave that plays a sound. I have included my main.c file below.

## Main.c code

```c
/*
 * MAIN Generated Driver File
 * 
 * @file main.c
 * 
 * @defgroup main MAIN
 * 
 * @brief This is the generated driver implementation file for the MAIN driver.
 *
 * @version MAIN Driver Version 1.0.2
 *
 * @version Package Version: 3.1.2
*/

/*
© [2025] Microchip Technology Inc. and its subsidiaries.

    Subject to your compliance with these terms, you may use Microchip 
    software and any derivatives exclusively with Microchip products. 
    You are responsible for complying with 3rd party license terms  
    applicable to your use of 3rd party software (including open source  
    software) that may accompany Microchip software. SOFTWARE IS ?AS IS.? 
    NO WARRANTIES, WHETHER EXPRESS, IMPLIED OR STATUTORY, APPLY TO THIS 
    SOFTWARE, INCLUDING ANY IMPLIED WARRANTIES OF NON-INFRINGEMENT,  
    MERCHANTABILITY, OR FITNESS FOR A PARTICULAR PURPOSE. IN NO EVENT 
    WILL MICROCHIP BE LIABLE FOR ANY INDIRECT, SPECIAL, PUNITIVE, 
    INCIDENTAL OR CONSEQUENTIAL LOSS, DAMAGE, COST OR EXPENSE OF ANY 
    KIND WHATSOEVER RELATED TO THE SOFTWARE, HOWEVER CAUSED, EVEN IF 
    MICROCHIP HAS BEEN ADVISED OF THE POSSIBILITY OR THE DAMAGES ARE 
    FORESEEABLE. TO THE FULLEST EXTENT ALLOWED BY LAW, MICROCHIP?S 
    TOTAL LIABILITY ON ALL CLAIMS RELATED TO THE SOFTWARE WILL NOT 
    EXCEED AMOUNT OF FEES, IF ANY, YOU PAID DIRECTLY TO MICROCHIP FOR 
    THIS SOFTWARE.
*/
#include "mcc_generated_files/system/system.h"
#include <stdint.h>

/*
    Main application
*/

int main(void)
{
    SYSTEM_Initialize();
    DAC1_Initialize();


    uint8_t analog_out = 0; 
    int LED;

    while (1)
     {
        LED+=1;
        if (LED>=1500)
        {
            //LED blink timing
            IO_RF3_Toggle(); 
            LED = 0;
        }
     
     if (IO_RD6_PORT == 1)
     {
        // toggle between 180 and 0 ? square wave
        analog_out = (analog_out == 180) ? 0 : 180 ;
     }
    else
       {
        // silence
        analog_out = 0;
       }
         
        DAC1_SetOutput(analog_out);

         __delay_ms(5);   // change for pitch
    }
           
}
```

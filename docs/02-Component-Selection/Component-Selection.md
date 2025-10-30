---
title: Component Selection Example
---

## Examples

*Table 1: Component selection*

**Speaker**

| **Solution**                                                                                                                                                                                      | **Pros**                                                                                                                                    | **Cons**                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
|![Speaker Option 1 ](.png)
<br>Option 1.<br> SP-4005Y<br>$2.09/each<br>[link to product](https://www.digikey.com/en/products/detail/soberton-inc/SP-4005Y/9924431)                 | \* Inexpensive[^1]<br>\* 88 db output <br>\*Through hole soldered | \* Requires external components and support circuitry for interface<br>\* Needs special PCB layout. |
|<img width="970" height="728" alt="image" src="https://github.com/user-attachments/assets/e759554e-7d92-4457-a32f-5cc7db7a6c64" />
<br>\* Option 2. <br>\* Speaker - 3" Diameter - 4 Ohm 3 Watt <br>\* $1.95/each <br>\* [Link to product](https://www.adafruit.com/product/1314#description) | \* Cheaper  <br>\* 92 db output | * Larger Size <br> *Tariff May Apply |
|<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/b82a7736-236a-435b-a56d-7c9911414197" />
<br>\* Option 3. <br>\* Vansonic 50CS08FH-1 Round Ferrite Speaker <br>\* $0.59/each <br>\* [Link to product](https://www.jameco.com/z/50CS08FH-1-Vansonic-Round-Ferrite-Speaker-1-94-Diameter-8-ohm-0-4-Watt-200-Hz-to-5-kHz_2328575.html) | \* Cheaper  <br>\* 85 db output | * Sound quality is not good <br> *Supporting Circuit needed |

**Choice:** Option 3: Vansonic 50CS08FH-1 Round Ferrite Speaker

**Rationale:** We already have a capable speaker we were given in class, which reduces shipping time and is already soldered and ready to plug into the circuit.

**Solenoid Motor**

| **Solution**                                                                                                                                                                                      | **Pros**                                                                                                                                    | **Cons**                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
|<img width="970" height="728" alt="image" src="https://github.com/user-attachments/assets/2b05872e-3e23-478f-9d25-b759202749ff" />
<br>Option 1.<br> Plastic Water Solenoid Valve - 12V - 1/2" Nominal <br>$6.95/each<br>[link to product](https://www.adafruit.com/product/997)                 | \* Inexpensive[^1]<br>\* Compatible with PSoC<br>\                                           | \* Requires external components and support circuitry for interface<br>\* Needs special PCB layout. |
|<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/a199710d-34a3-4170-a1e1-5ec0078e723d" />
<br>\* Option 2. <br>\* 12V Solenoid Valve - 3/4" - 1046 <br>\* $9.62/each <br>\* [Link to product](https://www.digikey.com/en/products/detail/sparkfun-electronics/10456/5684378) | \* Smaller  <br>\* Operates at 0.2~8 bar | * 0°C ~ 75°C <br> *Tariff May Apply |
|<img width="150" height="100" alt="image" src="https://github.com/user-attachments/assets/5583143f-d1e5-407f-9964-3e7c33353db1" />
<br>\* Option 3. <br>\* DFRobot FIT0617 Solenoid Valve <br>\* $25/each <br>\* [Link to product](https://www.mouser.com/ProductDetail/DFRobot/FIT0617?qs=T3oQrply3y%2Fjsecd34PRgA%3D%3D) | \* Direct connection to Microcontroller  <br>\* Valve and DC Motor integrated | * Larger Size <br> *Estimated 44% Tariff |

**Choice:** Option 3: DFRobot FIT0617 Solenoid Valve

**Rationale:** Because we didn't use most of the budget on the Speaker, I think we can spend some here to get a really plug-and-play solenoid motor that fits directly with the PIC Nano.

**MOSFET**

| **Solution**                                                                                                                                                                                      | **Pros**                                                                                                                                    | **Cons**                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
|<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/749d155d-21b8-488c-92cd-9c02dfc82ca9" />
<br>Option 1.<br> AOT2618L <br>$1.66/each<br>[link to product](https://www.digikey.com/en/products/detail/alpha-omega-semiconductor-inc/AOT2618L/3603378)                 | \* Inexpensive[^1]<br>\* Compatible with PSoC<br>                                         | \* Requires external components and support circuitry for interface<br>\* Needs special PCB layout. |
|<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/6470c0e6-83db-4919-b957-d2624f7f0ed7" />
<br>\* Option 2. <br>\* NDP6060L <br>\* $2.63/each <br>\* [Link to product](https://www.digikey.com/en/products/detail/onsemi/NDP6060L/244273) | \* 60 V 48 Amp  <br>\* 471 in stock | * Onsemi is from AZ <br> *more expensive |
|<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/de1b6310-40f5-4351-a05a-6c91c1164abf" />
<br>\* Option 3. <br>\* STP55NF06 <br>\* $1.47/each <br>\* [Link to product](https://www.digikey.com/en/products/detail/stmicroelectronics/STP55NF06/603802) | \* Cheapest  <br>\* 60 V 50 Amp \ *Lowest manufactuerer lead time| <br> * No real negatives  |

**Choice:** Option 3 or 1

**Rationale:** In between 3 and 1 because option 1 I already have and do not need to wait, but option 3 might just be better overall in terms of price and functionality. All in all, Option 1 is the easiest because I already have it on hand.




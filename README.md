So i am trying to make a NFC sticker which will be the shape of the hackclub Orpheous sticker i will make it into a pretty looking PCB which will have a NFC chip and a coil which will pick up electromagnetic waves convert them into electrical signals and then light up an LED.

# Overview
This is a Orpherous flag sticker shaped PCB which uses a NFC ICs and an energy buffering mechanism to store enough power to light up a LED
once the pcb is fabricated The original hakc club fag sticker can be sticked on top of this pcb after which the ICs and electronics won't be visible and then once we bring this near a NFC reader or any electromangentic coil which is actively pulsing energy Then this NFC's electromagnetic coil picks up that charge and then it stores all the charge inside of a energy buffer which stores enough energy to light up 3 led's and hence make the sticker glow 

# Schematics 
<img width="916" height="621" alt="image" src="https://github.com/user-attachments/assets/26c020c0-db32-42f3-a533-56aee9a37eb9" />

**The main ICs used inside this system are**
1. ST25DV04K - This is a NFC enegry harvester IC which takes the RF Signals as the input and then converts it into stable DC electic voltage
2. BD58xxE - This is a very efficient voltage detection IC which detects the flow of energy inside the circuit
3. Metic 0603 Capscitors and LEDs are used for keeping the circuit small enough to fit on a sticker

# Routing
<img width="930" height="480" alt="image" src="https://github.com/user-attachments/assets/68062253-43c8-4659-a2d1-08c28e4cb36a" />
<img width="878" height="475" alt="image" src="https://github.com/user-attachments/assets/640e8efb-8df1-4a1b-868b-48296a56164d" />

The entire edge.cuts layes is a complx polygon which was required to be traced by hand in order to make the proper Outter PCB edge outline
The main paw had the RF antenna with 4 circualr loops each 0.25mm thick 
The main ICs is seated on the flag part
There are 3 leds 2 on the paw and one on the flag 
All are bright enough to illuminate the Sticker fully 

# 3D render 
<img width="518" height="286" alt="image" src="https://github.com/user-attachments/assets/fb65c6be-12f7-48ac-8645-3953365c71db" />

This render appears green because it was rendered inside Kicad 
I will use a White PCB ,golden pads and Black silkscreen from JLCPCB for making this look even prettier 

# Final render
<img width="926" height="423" alt="image" src="https://github.com/user-attachments/assets/199e4363-3a08-4688-8e13-5fe010a320a3" />

# BOM
| Designator | Component | Package | Qty | Est. Unit Price (USD) | Total Price (USD) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **U1** | ST25DV04K (NFC Harvester IC) | SO8 | 1 | $0.90 | $0.90 |
| **U2** | BD48K23G (2.3V Voltage Supervisor) | SOT-23-3 | 1 | $0.30 | $0.30 |
| **C2** | 10 µF Capacitor | 0603 | 1 | $0.02 | $0.02 |
| **C3** | 100 nF Capacitor | 0603 | 1 | $0.01 | $0.01 |
| **R1, R2, R3** | 330 Ω Resistor | 0603 | 3 | $0.01 | $0.03 |
| **D1, D2, D3** | LED (Any Color) | 0603 | 3 | $0.03 | $0.09 |

**Total Component Cost:** ~$1.35 per board
**PCB Ccost - 2.1$** 
**Total Estimated Cost (PCB + Components): ~$3.45 per unit**






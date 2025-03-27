# Business Card that Plays Pong
I wanted a business card that stood out. This went through 3 iterations before I got one that work, and 5 before I felt comfortable showing this to other people. It is a business card PCB that runs on a CR2032/2025 battery and utilizes a shift register to multiplex an 8x8 LED array. All of which is controlled with an STM32L010F4 (which isn't exactly necessary for this application as I am running it like any other STM32 microcontroller.).


<p align="center">
  <img src="/images/business_card_frnt.jpeg" width="350" alt="A picture of a green business card sized PCB that has an 8x8 display along with 2 buttons and 2 integrated circuits.">
  <img src="/images/business_card_back.jpeg" width="350" alt="The back of the business card has text that is blurred, but it is clear it is a person's business card.">
</p>


## How it was made

### Designed in KiCAD
I designed this in KiCAD over 5 iterations (one of the iterations only had a misplaced via). I wanted to use the ATMega328p microcontroller at first because it was the only microcontroller I had ever programmed. But after running into some simple and solveable issues, I realized this project was already going to take a while, so I might as well learn something new. This is why I decided to use the [STM32L010F4](https://www.st.com/en/microcontrollers-microprocessors/stm32l010f4.html) microcontroller for its "low power" utilities. I didn't end up using an of these low power utilities because the card ended up running fine on the button cell battery and the LEDs would end up being the majority of the current draw at any one moment.
![A screenshot of the schematic for the business card PCB. The image includes symbols for a shift register, microcontroller, 2 buttons, some resistors and capacitors, pin headers, an active oscillator, and 64 LEDs in an array.](/images/business_card_images/business_schematic.jpg)

Please don't judge my PCB design skills, I am (mostly) self-taught and this circuit does not require any high frequency or high voltage wiring techniques. I ordered the PCB from JLCPCB because no other PCB manufacturer comes close to their extremely low pricing ($4 for 5 PCBs, including shipping).
![A screenshot of a PCB design from KiCAD. It includes two layers](/images/business_card_images/business_pcb.jpg)
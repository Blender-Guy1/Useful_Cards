# Useful_Cards
This is a repository that contains cards that are useful or fun. This includes business cards that can play Pong and cards that act as simple electronics equipment for troubleshooting on the road.

## The Different Cards

### Business Card that Plays [Pong](https://en.wikipedia.org/wiki/Pong)
This went through 3 iterations before I got one that work, and 5 before I felt comfortable showing this to other people. It is a business card PCB that runs on a button cell battery and can play a any games that will run on the microcontroller. All of which is controlled with an [STM32L010F4](https://www.digikey.com/en/products/detail/stmicroelectronics/STM32L010F4P6/10063389) (which isn't exactly necessary for this application as I am running it like any other STM32 microcontroller.). More information can be found in the readme.md in the folder named "Business Card".


<p align="center">
  <img src="/images/business_card_frnt.jpeg" width="350" alt="A picture of a green business card sized PCB that has an 8x8 display along with 2 buttons and 2 integrated circuits.">
  <img src="/images/business_card_back.jpeg" width="350" alt="The back of the business card has text that is blurred, but it is clear it is a person's business card.">
</p>



### Why I wanted to make Business Cards

I exhibitted at [OpenSauce 2024](https://opensauce.com/) and had the pleasure to meet [Ben Eater](https://www.youtube.com/@BenEater). He handed me a business card that was a puzzle. When a CR2025 battery was inserted, the 8 LEDs on the PCB would blink "SHAKE ME" in ASCII. Once shaken, the card wrote Ben Eater in the air. This was by far the coolest electronics idea I had ever seen. This got me thinking for a while and eventually I decided to steal his idea and make a 3D holographic business card. But that would be pretty lazy and unoriginal, so I decided on something similar that was simple. This led me to creating a business card that could play pong. 
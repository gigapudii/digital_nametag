# Digital nametag
A digital nametag based on the Nokia 3310 screen, making you interesting during fairs.

## WHY
Often during fairs I feel that I'm not seen much. The digital nametag was created in order to be used as a conversation starter and to help show my creativity to the public. Aside of this, it gave me the possibility to present parts of my CV as well as my contact information.

![digital-nametag-front](https://i.imgur.com/008BkxN.jpg)

## HOW
For the nametag I needed a screen to begin with. Considering that Nokia 3310 screens are big enough and apparently are still sold online, I found a few to a low price. Aside of this, I needed an Attiny, a battery, a power-button to power up the screen, and another button to power up the backlight of the screen. 

As for the microcontroller, I chose the Attiny85 because it's a) low powered b) cheap and c) has just enough pins to drive the screen. The battery is a coin battery CR2032.

Since there is no board that fits the screen and the components, I had to create my own. To design the board I used Eagle CAD. The basic thought during this process was to make it "invisible", i.e. have it hidden behind the screen, and for it to have a small cut on the top on which I could hang it. Apart from this, the most important part was to make the correct connections between the board and the screen which was fairly straight forward. 

![digital-nametag-back](https://i.imgur.com/sH9JIlN.jpg)
![digital-nametag-size](https://i.imgur.com/yzrTcCb.jpg)

As for the software, I used a [library](https://github.com/platisd/nokia-5110-lcd-library) for this particular Nokia screen. 
Additionally, when screen is not updated, the microcontroller is in deep sleep to preserve the battery.

To create the images that were displayed on the screen I used Adobe Photoshop and the LCD Assistant.

## Components
* [Nametag PCB](https://oshpark.com/shared_projects/H9KOpiVm)
* Attiny85
* Coin battery CR2032
* Coin battery holder
* Power-button
* Backlight button
* Resistor (for the backlight)
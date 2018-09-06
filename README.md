# Digital nametag
A digital nametag based on the Nokia 3310 screen, making you interesting during fairs.

## WHY
Whenever I visit fairs, I often feel that I am not noticed very much. And when I do find someone to speak to, I sometimes find it hard to start a conversation. 

![digital-nametag-front](https://i.imgur.com/008BkxN.jpg)

## HOW
The solution is a digital nametag. It can be used as a conversation starter and help show your creativity to the public. Aside of this, it gives you the possibility to present parts of your CV as well as contact information without having to spell it out loud everytime.

For the nametag you will need a screen to begin with. Nokia 3310 screens are big enough and apparently still sold online. Aside of this, you will need an Attiny85, a coin cell battery (CR2032), an on/off switch, and a button to power up the backlight of the screen. 

As for the microcontroller, the Attiny85 is preferred because it's a) low powered b) cheap and c) has just enough pins to drive the screen.

To design the board, Eagle CAD was used. The basic thought during the design process was to make it "invisible", i.e. have it hidden behind the screen, and for it to have a small cut on the top to be hanged through. Apart from this, the most important part was to make the correct connections between the board and the screen which was fairly straight forward. 

![digital-nametag-back](https://i.imgur.com/TknoJRL.jpg)
![digital-nametag-size](https://i.imgur.com/yzrTcCb.jpg)

As for the software, the screen is controlled through an [Arduino library](https://github.com/platisd/nokia-5110-lcd-library). Additionally, when the creen is not updated, the microcontroller is in deep sleep to preserve the battery.

To create the images that were displayed on the screen, Adobe Photoshop and the LCD Assistant were mainly used.

## Components
* [Nametag PCB](https://oshpark.com/shared_projects/H9KOpiVm)
* Attiny85
* Coin cell battery CR2032
* Coin cell battery holder
* On/off switch
* Backlight button
* Resistor (for the backlight)
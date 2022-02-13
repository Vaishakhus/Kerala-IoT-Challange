# Kerala-IoT-Challange
> [**Foxlab Makerspace**](https://www.facebook.com/foxlabmakerspace/) in association with [**GTech - Group of Technology Companies**](https://atfg.gtechindia.org/) in Kerala is launching our prestigious program **“Kerala IoT Challenge 2021”**, with a vision to mould 100 IoT experts in Kerala, hosting on the µLearn platform. **Kerala IoT Challenge** is a program designed in 4 levels followed by a hackathon to identify and train quality industry leaders in the IoT domain, while any novice learner 
> # About Me 
> Hi,everyone I am Vaishakh U S ,Currently pursuing B-tech from RIT Kotayam,My field of intrests are
* public speaking
* IoT
* Automation
* Projects 

# Experiment-1 HELLO WORLD LED BLINKING
## Components Required
* Arduino Uno R3 *1
* Bread Board *1
* Jumper Wires(Male to male ) *2
* LED *1
* 220 Ohm resistor *1
* Usb A to B cable *1
## circuit diagram 
![](https://user-images.githubusercontent.com/95710924/153770168-8d2d390e-2e3d-4d3a-95f7-34660651d5c1.png)
## code
``` 
int ledPin=5;  //defining ledpin as pin 5
void setup() {
   pinMode(5,OUTPUT); //define pin5 as output type: 
}
void loop() {
  digitalWrite(ledPin,HIGH);//setting pin to on position
  delay(1000); //delay of 1 second
  digitalWrite(ledPin,LOW);//set led to off position
  delay(1000); //wait for a second
  
  

}

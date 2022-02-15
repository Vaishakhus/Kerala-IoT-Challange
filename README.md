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
```
## output 
LED will blink every second

# Experiment-2  TRAFFIC LIGHT
## COMPONENTS REQUIRED
* Arduino UNO
* A Breadboard
* Male to male jumper wires (x4)
* LED (Red,Yellow,Green)
* USB cable to connect the arduino
* Resistors (3x)
## Circuit Diagram
![ex2](https://user-images.githubusercontent.com/95710924/154120563-dc9b72f3-7445-42c7-939d-19ef4aab790a.png)
## code
```
int redled =10; // initialize digital pin 8.
int yellowled =7; // initialize digital pin 7.
int greenled =4; // initialize digital pin 4.
void setup()
{
pinMode(redled, OUTPUT);// set the pin with red LED as “output”
pinMode(yellowled, OUTPUT); // set the pin with yellow LED as “output”
pinMode(greenled, OUTPUT); // set the pin with green LED as “output”
}
void loop()
{
digitalWrite(greenled, HIGH);//// turn on green LED
delay(5000);// wait 5 seconds

digitalWrite(greenled, LOW); // turn off green LED
for(int i=0;i<3;i++)// blinks for 3 times
{
delay(500);// wait 0.5 second
digitalWrite(yellowled, HIGH);// turn on yellow LED
delay(500);// wait 0.5 second
digitalWrite(yellowled, LOW);// turn off yellow LED
} 
delay(500);// wait 0.5 second
digitalWrite(redled, HIGH);// turn on red LED
delay(5000);// wait 5 seconds
digitalWrite(redled, LOW);// turn off red LED
}
```
## output 
In Traffic light, the green LED blink about 5 second, then it is turnoff. Then the yellow LED blinks 3 times with a time interval of 0.5 second.Then the red LED blink about 5 seconds


# EXPERIMENT 3  LED CHASING EFFECT
## components required 
* Led x6
* Arduino board
* 220Ω resistor x6
* Breadboard
* wires
## circuit diagram
![ex 3](https://user-images.githubusercontent.com/95710924/154127155-acbd4c07-0b9a-4f9e-af69-f8a1c18b7366.png)
## code
```
int BASE = 2;  // the I/O pin for the first LED

int NUM = 6;   // number of LEDs

void setup()

{

   for (int i = BASE; i < BASE + NUM; i++) 
   
   {
   
     pinMode(i, OUTPUT);   // set I/O pins as output
     
   }
   
}

void loop()

{

   for (int i = BASE; i < BASE + NUM; i++) 
   
   {
   
     digitalWrite(i, LOW);    // set I/O pins as “low”, turn off LEDs one by one.
     
     delay(200);        // delay
     
   }
   
   for (int i = BASE; i < BASE + NUM; i++) 
   
   {
   
     digitalWrite(i, HIGH);    // set I/O pins as “high”, turn on LEDs one by one
     
     delay(200);        // delay
     
   }  
   
}
```
## output 
all LEDs will blink in sequence and after that all will switchon and off same time\

# EXPERIMENT 4 BUTTON CONTROLLED LED
## COMPONENTS REQUIRED
* Arduino Uno
* Button switch
* Red M5 LED
* 220ΩResistor
* 10KΩ Resistor
* Breadboard
* Jumper Wire
## Circuit Diagram
![ex4](https://user-images.githubusercontent.com/95710924/154128846-573a3c11-3c98-4471-9621-e7bf014ca1d9.png)





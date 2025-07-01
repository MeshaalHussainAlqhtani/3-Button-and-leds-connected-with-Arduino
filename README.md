# 3-Button-and-leds-connected-with-Arduino

*Circuit Explanation, This setup includes:
Arduino UNO
Breadboard, Wires connecting everything together, 3 push buttons,3 LEDs (with current-limiting resistors)
LEDs Description: LEDs placed on the breadboard, each connected to GND through a resistor 
Push Buttons Description:  buttons. Each has one leg connected to Arduino digital pins and the other to GND
Wiring:
-Button 1 → Arduino Digital Pin 2 (White wire)
-Button 2 → Arduino Digital Pin 3 (Red wire)
-Button 3 → Arduino Digital Pin 5 (Green wire)
-All buttons are also connected to GND.
-LEDs are connected through resistors to GND and their other side seems ready to be controlled by digital pins 

*Code Explanation:
const int button1=2;
const int button2=3;
const int button3=5;
void setup(){
  pinMode(button1,INPUT);
   pinMode(button2,INPUT);
   pinMode(button3,INPUT);
}
void loop(){
  int buttonState1=digitalRead(button1);
}
Each button pin is set as an INPUT, meaning the Arduino will read whether the button is pressed HIGH or LOW.
loop part:
int buttonState1 = digitalRead(button1);
-Reads the current state of button 1

*in summary:
-The photo shows 3 push buttons connected to Arduino inputs
LEDs are wired but unused so far — the code should be extended to control them based on button presses.

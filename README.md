# motor-encoder

https://www.tinkercad.com/things/6AATPQEhhvm


// C++ code
//
void setup()
{
    pinMode(ENCA,INPUT); // sets pin2 as the input
  pinMode(ENCB,INPUT); // sets pin4 as the input

  
  
  
 
}
void loop()
{
 
#define ENCA 2 // pin2 of the Arduino
#define ENCB 4 // Pin4 of the Arduino
int ENCA_DATA;
int ENCB_DATA;
  
  ENCA_DATA = digitalRead(ENCA); 
// We simply read Pin2 of the Arduino and store the result in variable ENCA_DATA
  ENCB_DATA = digitalRead(ENCB); 
// We simply read Pin3 of the Arduino and store the result in variable b
  Serial.print(ENCA_DATA*5); 
  Serial.print(" ");
  Serial.print(ENCB_DATA*5);
  Serial.println();
}

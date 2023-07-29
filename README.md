# SM_Electric_Task1
// LED and button Arduino circuit 
//Tinkercad link:  https://www.tinkercad.com/things/hHC73CG5uTm

//the Arduino code:

int buttonState = 0;
void setup()
{
  pinMode(2, INPUT); 
  pinMode(13, OUTPUT); 
}

void loop()
{
 
  buttonState = digitalRead(2); 
  
  if (buttonState == HIGH) {
   
    digitalWrite(13, HIGH);
  } else {
    
    digitalWrite(13, LOW);
  }
  delay(10); 

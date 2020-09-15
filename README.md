# ARDUINO-第五篇 
```c++
void setup() {
  // put your setup code here, to run once:
  pinMode(3,OUTPUT);
}
int i = 255;
int x = -15;
void loop() {
  // put your main code here, to run repeatedly:
  /*for(i=255 ; i>=0 ; i=i-15 )
  {
    analogWrite(3,i);
    delay(70);
  }
  for(i=0 ; i<255 ; i=i+15 )
  {
    analogWrite(3,i);
    delay(70);
  }*/
  if(i>=255||i<=0){x=-x;}
  i=i-x;
  analogWrite(3,i);
  delay(70);
}
```

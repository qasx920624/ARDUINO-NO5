# ARDUINO-第五篇 
呼吸燈</p>
程式如下</p>
```c++
void setup() {
  pinMode(3,OUTPUT);
}
int i = 255;
int x = -15;
void loop() {
  if(i>=255||i<=0){x=-x;}//如果常數i大於等於255"或"小於等於0,x變號
  i=i-x;
  analogWrite(3,i);
  delay(70);
}
```

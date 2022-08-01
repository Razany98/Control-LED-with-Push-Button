# Push Button 

one of the special components different from the on/off buttons for allowing the Arduino to on/off light without personal control. 

### Requested Materials: 
- Arduino UNO
- BreadBoard 
- Push Button 
- LED 
- Resistor 
- Jumper Wires 

### Connection: 

- Place the pushbutton anywhere between the two sides of the breadboard 
- Connect the led with the arduino board. 
- attach the resister to the button's leg
- supply the wires between the breadboard and the arduino. 
- Connect the wires as shown in the figure below. 

![](images/PushButton.png)

### Programming Code: 
```
void setup()
{
  pinMode(2, INPUT);
  pinMode(13, OUTPUT);
}

void loop()
{
  if(digitalRead(2) == 1)
  {
    digitalWrite(13, HIGH);
  }
  else 
  {
    digitalWrite(13, LOW);
  }
}
```

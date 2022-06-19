# arduino-code
i need an arduino code
im using an arduino mega with 6 dc motors, 3 drivers with a bluetooth module and im using this following code
void setup()
{
Serial.begin(9600);
pinMode(2,OUTPUT);
pinMode(3,OUTPUT);
pinMode(4,OUTPUT);
pinMode(5,OUTPUT);
pinMode(6,OUTPUT);
pinMode(7,OUTPUT);
pinMode(8,OUTPUT);
pinMode(9,OUTPUT);
pinMode(10,OUTPUT);
pinMode(11,OUTPUT);
pinMode(12,OUTPUT);
pinMode(13,OUTPUT);
}
void loop()
{
if(Serial.available()>0)
{
char data = Serial.read();
if (data == 'w')
{
digitalWrite(2,HIGH);
digitalWrite(4,HIGH);
digitalWrite(6,HIGH);
digitalWrite(8,HIGH);
digitalWrite(10,HIGH);
digitalWrite(12,HIGH);
digitalWrite(3,LOW);
digitalWrite(5,LOW);
digitalWrite(7,LOW);
digitalWrite(9,LOW);
digitalWrite(11,LOW);
digitalWrite(13,LOW);
}
else if(data == 's')

{
digitalWrite(2,LOW);
digitalWrite(4,LOW);
digitalWrite(6,LOW);
digitalWrite(8,LOW);
digitalWrite(10,LOW);
digitalWrite(12,LOW);
digitalWrite(3,HIGH);
digitalWrite(5,HIGH);
digitalWrite(7,HIGH);
digitalWrite(9,HIGH);
digitalWrite(11,HIGH);
digitalWrite(13,HIGH);

}
else if(data == 'd')

{
digitalWrite(2,HIGH);
digitalWrite(4,LOW);
digitalWrite(6,HIGH);
digitalWrite(8,LOW);
digitalWrite(10,HIGH);
digitalWrite(12,LOW);
digitalWrite(3,LOW);
digitalWrite(5,HIGH);
digitalWrite(7,LOW);
digitalWrite(9,HIGH);
digitalWrite(11,LOW);
digitalWrite(13,HIGH);

}
else if(data == 'a')

{
digitalWrite(2,LOW);
digitalWrite(4,HIGH);

digitalWrite(6,LOW);
digitalWrite(8,HIGH);
digitalWrite(10,LOW);
digitalWrite(12,HIGH);
digitalWrite(3,HIGH);
digitalWrite(5,LOW);
digitalWrite(7,HIGH);
digitalWrite(9,LOW);
digitalWrite(11,HIGH);
digitalWrite(13,LOW);

}
else if(data == 'f')
{
digitalWrite(2,LOW);
digitalWrite(4,LOW);
digitalWrite(6,LOW);
digitalWrite(8,LOW);
digitalWrite(10,LOW);
digitalWrite(12,LOW);
digitalWrite(3,LOW);
digitalWrite(5,LOW);
digitalWrite(7,LOW);
digitalWrite(9,LOW);
digitalWrite(11,LOW);
digitalWrite(13,LOW);
}
}
}

i would really appreaciate it if you would correct me or tell me where im wrong and what im missing.
thank you

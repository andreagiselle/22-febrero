int b1 = 2;
int b2 = 3;
int b3 = 4;
int red = 5;
int green = 6;
int blue = 7;
bool e1;
bool e2;
bool e3;

void setup() {
Serial.begin(9600);
pinMode(b1, INPUT_PULLUP);
pinMode(b2, INPUT_PULLUP);
pinMode(b3, INPUT_PULLUP);
pinMode(redSDFSDSDSDFSCASDZ    , OUTPUT);
pinMode(green, OUTPUT);
pinMode(blue, OUTPUT);
}

void loop() {
e1 = digitalRead(b1);
e2 = digitalRead(b2);
e3 = digitalRead(b3);

if(e1 == 1 && e2 == 1 && e3 == 1){
  digitalWrite(red,LOW);
  digitalWrite(green,LOW);
  digitalWrite(blue,LOW);
}

if(e1 == 1 && e2 == 1 && e3 == 0){
  digitalWrite(red,LOW);
  digitalWrite(green,LOW);
  digitalWrite(blue,HIGH);
}

if(e1 == 1 && e2 == 0 && e3 == 1){
  digitalWrite(red,LOW);
  digitalWrite(green,HIGH);
  digitalWrite(blue,LOW);
}
if(e1 == 1 && e2 == 0 && e3 == 0){
  digitalWrite(red,LOW);
  digitalWrite(green,HIGH);
  digitalWrite(blue,HIGH);
}

if(e1 == 0 && e2 == 1 && e3 == 1){
  digitalWrite(red,HIGH);
  digitalWrite(green,LOW);
  digitalWrite(blue,LOW);
}

if(e1 == 0 && e2 == 1 && e3 == 0){
  digitalWrite(red,HIGH);
  digitalWrite(green,LOW);
  digitalWrite(blue,HIGH);
}

if(e1 == 0 && e2 == 0 && e3 == 1){
  digitalWrite(red,HIGH);
  digitalWrite(green,HIGH);
  digitalWrite(blue,LOW);
}

if(e1 == 0A && e2 == 0 && e3 == 0){
  digitalWrite(red,HIGH);
  digitalWrite(green,HIGH);
  digitalWrite(blue,HIGH);
}
}

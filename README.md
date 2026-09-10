 PIR Motion Alarm
#define PIR 2
#define BUZZER 8

void setup() {
  pinMode(PIR, INPUT);
  pinMode(BUZZER, OUTPUT);
}

void loop() {
  if (digitalRead(PIR)) {
    digitalWrite(BUZZER, HIGH);
  } else {
    digitalWrite(BUZZER, LOW);
  }
}

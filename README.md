# arduino
um sistema no arduino onde ao apertar o botao o buzzer faz barulho


https://github.com/user-attachments/assets/12b2c5c2-41a7-417f-a62d-c8a538d67b41

codigo utilizado:
// C++ code
//
void setup()
{
  pinMode(A0, INPUT);
  pinMode(3, OUTPUT);
  pinMode(2, OUTPUT);
}

void loop()
{
  if (digitalRead(A0) == HIGH) {
    tone(3, 523, 1000); // play tone 60 (C5 = 523 Hz)
    digitalWrite(2, HIGH);
    delay(1000); // Wait for 1000 millisecond(s)
    digitalWrite(2, LOW);
  }
}



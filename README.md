const int ledPin = 7;

void setup() {
  pinMode(ledPin, OUTPUT);
}

void loop() {
  // 처음 1초간 LED 켜기
  digitalWrite(ledPin, HIGH);
  delay(1000);

  // 다음 1초 동안 LED 5회 깜빡임 (0.2초 주기)
  for (int i = 0; i < 5; i++) {
    digitalWrite(ledPin, LOW);
    delay(100);  // 0.1초 OFF
    digitalWrite(ledPin, HIGH);
    delay(100);  // 0.1초 ON
  }

  // LED 끄고 종료(while(1){} 무한루프)
  digitalWrite(ledPin, LOW);
  while (1) {
    // 무한루프
  }
}

  


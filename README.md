void setup() {
  pinMode(LED_BUILTIN, OUTPUT);   // Sätter LED på pin 13 
  Serial.begin(9600);             // Startar seriell kommunikation
  delay(1000);

  Serial.println("Arduino-test startar...");
}

void loop() {
  // Slå på LED
  digitalWrite(LED_BUILTIN, HIGH);
  Serial.println("LED ON");
  delay(500);

  // Slå av LED
  digitalWrite(LED_BUILTIN, LOW);
  Serial.println("LED OFF");
  delay(500);
}


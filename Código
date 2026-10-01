const int LDR_PIN = A0;
const int LED_VERDE = D5;
const int LED_VERMELHO = D6;

void setup() {
  Serial.begin(115200);

  pinMode(LED_VERDE, OUTPUT);
  pinMode(LED_VERMELHO, OUTPUT);
}

void loop() {
  // Lê o valor do LDR
  int valorLDR = analogRead(LDR_PIN);

  // Mostra o valor no Monitor Serial
  Serial.print("Valor do LDR: ");
  Serial.println(valorLDR);

  // Compara com o limite de 300
  if (valorLDR > 300) {
    digitalWrite(LED_VERDE, HIGH);
    digitalWrite(LED_VERMELHO, LOW);

    Serial.println("Luminosidade acima de 300 - LED VERDE");
  } 
  else {
    digitalWrite(LED_VERDE, LOW);
    digitalWrite(LED_VERMELHO, HIGH);

    Serial.println("Luminosidade igual ou abaixo de 300 - LED VERMELHO");
  }

  delay(500);
}

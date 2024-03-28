
int ledPinRed = 6; //Pino do LED VERMELHO

int ledPinGreen = 5; //Pino do LED VERDE

int sensorPin = 3; //ENTRADA PINO SENSOR

int leitura; // VARIAVEL MUDANÇA DE ESTADO

void setup() {
 
pinMode(ledPinRed,OUTPUT);

pinMode(ledPinGreen,OUTPUT);

pinMode(sensorPin,INPUT);

}

void loop() {

leitura = digitalRead(sensorPin);

  if (leitura == LOW) { 

      digitalWrite(ledPinGreen, LOW);
      
      digitalWrite(ledPinRed, HIGH);

      }
 
  else{ 
  
      digitalWrite(ledPinGreen, HIGH);
      
      digitalWrite(ledPinRed, LOW);
    
    }
}

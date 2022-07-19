# Alarme 

## Instruções:

COnstrução de um alarme, que apita ao detectar movimento e pode ser posicionado perto de portas a fins de segurança.

## Os componentes

Sensor de Movimento, Buzzer, LED, resistor, jumpers e arduino.

## Imagem das conexões do circuito
<img src="./imagens/conexoes.png">

## Imagem do circuito montado 
<img src="./imagens/foto.png">

## Vídeo no Youtube TROCAR
https://youtu.be/0L9eRKaqJ-0

## Código

#define pinBuzzer  8
#define pinSensorPIR  7
#define pinLed  9
bool valorSensorPIR;
int frequencia = 1000;
int tempoBuzzerLigado = 2000;

void setup() {
  pinMode(pinBuzzer, OUTPUT);
  pinMode(pinSensorPIR, INPUT);
  pinMode(pinLed, OUTPUT);
  Serial.begin(9600);
}


void loop() {
  valorSensorPIR = digitalRead(pinSensorPIR);
  if (valorSensorPIR) {
    ligarAlarme();
  } else {
    desligarAlarme();
  }
}

void ligarAlarme() {
  digitalWrite(pinLed, HIGH);
  tone(pinBuzzer, frequencia);
  delay(tempoBuzzerLigado);
  desligarAlarme();
}

void desligarAlarme() {
  digitalWrite(pinLed, LOW);
  noTone(pinBuzzer);
}


## Alunos:
João Pedro Soares Azevedo Calixto [(Calixto)]

Eduarda Neumasn Firstuadmanm [(Duda)]

Lucas de Souza Brandão [(Bombril)]

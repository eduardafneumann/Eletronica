# Alarme 

## Instruções:

Construção de um alarme, que apita ao detectar movimento e pode ser posicionado perto de portas a fins de segurança.

## Os componentes

Sensor de Movimento, Buzzer, LED, resistor, jumpers e arduino.

## Imagem das conexões do circuito
<img src="./imagens/conexoes.png">

## Imagem do circuito montado 
<img src="./imagens/foto.png">

## Vídeo no Youtube 
https://youtube.com/shorts/yVa9U3Thy9Y?feature=share

## O Sensor PIR:

Detecta movimento a partir da mudança de temperatura. Apesar de no cógido o sinal ter sido lido como binário, ao ser lido como analógico, retornou valores menores para temperaturas mais frias, a exemplo: 160 quando exposto a uma garrafa de água gelada, 165 em temperatura ambiente e 185 quando ativado por movimento humano. 
Visto de frente, há dois reguladores laranja: o da esquerda regula distância e o da direita sensibilidade.
Quando regulado para a menor distância, o sensor capta até por volta de 5m e a amplitude angular de detecção diminui. Não foi possível medir a distância máxima por conta de limitações físicas, mas sabe-se que a amplitude aumenta.
Quando a sensibilidade é regulada para o máximo, o alarme não para de tocar enquanto reconhecer movimento. Já quando mínima, há um atraso de 5-7 segundos para que dispare novamente.


## Alunos:
João Pedro Soares Azevedo Calixto [(Calixto)]

Eduarda Fritzen Neumann [(Duda)]

Lucas de Souza Brandão [(Bombril)]

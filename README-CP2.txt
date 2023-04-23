#Projeto alarme de nível de luz, umidade e temperatura com display utilizando arduino


###OBJETIVO
Fomos contratados pela Vinheria Agnello para desenvolver um sistema de monitoramento a ser instalado no ambiente em que os vinhos são armazenados. O dono da Vinheria informou que a qualidade do vinho é influenciada diretamente pelas condições de temperatura, umidade e luminosidade do ambiente. Após a primeira etapa concluída, onde fizemos um sistema que captava a luz do ambiente, o cliente pediu para implementarmos um monitoramento de temperatura e umidade também, além de mostrar a informação exata de qual temperatura e umidade está o depósito. Para isso, precisamos:

* Medir a temperatura e umidade do ambiente, para isso escolhemos o sensor integrado DHT11, que já possui uma biblioteca implementada para o Arduino. Precisamos aprender a instalar essa biblioteca no IDE do Arduino e utilizá-la para ler a temperatura e umidade do ambiente.
* Os proprietários querem ver os valores de temperatura e umidade de alguma forma, por isso sugerimos usar um display para mostrar esses valores.
* Os sinais de alerta foram bem aceitos, e os proprietários querem estender essa funcionalidade para temperatura e umidade, portanto, além de sinalizar com os LEDs e o Buzzer a luminosidade, também precisamos indicar quando a temperatura e/ou a umidade estiverem em níveis críticos.

Os principais requisitos do sistema são:

1. Enquanto o ambiente estiver escuro, o LED Verde deve ficar aceso;
2. Enquanto o ambiente estiver a meia luz, o LED amarelo deve ficar aceso e mensagem de “Ambiente a meia luz” deve ser mostrado no Display;
3. Enquanto o ambiente estiver totalmente iluminado, o LED vermelho deve ficar aceso e a mensagem “Ambiente muito claro” deve ser mostrado no display;
4. Enquanto o ambiente estiver totalmente iluminado, o Buzzer deve ficar ligado continuamente;
5. Enquanto o ambiente estiver com uma temperatura entre 10°C e 15°C, o Display deve informar “Temperatura OK” e também mostrar o valor da temperatura;
6. Enquanto o ambiente estiver com uma umidade entre 60% e 80%, o Display deve informar “Umidade OK”, e também mostrar o valor da umidade;
7. Os valores apresentados no display devem ser a média de pelo menos 5 leituras dos sensores, e os valores devem ser apresentados a cada 5 segundos;
8. Enquanto a temperatura estiver fora da faixa ideal, o LED Amarelo deve ficar aceso e o Buzzer deve ligar continuamente;
9. Enquanto a temperatura estiver fora da faixa ideal, o Display deve informar “Temp. Alta”, para valores acima de 15°C e também mostrar a temperatura;
10. Enquanto a temperatura estiver fora da faixa ideal, o Display deve informar “Temp. Baixa”, para valores abaixo de 10°C e também mostrar a temperatura;
11. Enquanto a umidade estiver fora da faixa ideal, o LED Vermelho deve ficar aceso e o Buzzer deve ligar continuamente;
12. Enquanto a umidade estiver fora da faixa ideal, o Display deve informar “Umidade Alta”, para valores acima de 70% e também mostrar a umidade;
13. Enquanto a umidade estiver fora da faixa ideal, o Display deve informar “Umidade Baixa”, para valores abaixo de 50% e também mostrar a umidade;


###DESCRIÇÃO
Este projeto tem como ideia implementar um sensor para monitorar a iluminação, temperatura e umidade presentes na sala em que são armazenados vinhos, tendo três níveis de alerta por LEDs: verde para condições ideais, amarelo para ficar alerta com a iluminação ou mostrar que a temperatura não está na faixa ideal, acionando também um buzzer, e vermelho no caso da luz chegar a níveis muito altos ou a umidade estar em uma faixa fora do ideal, que também aciona o buzzer. O sistema conta com um display que informa a cada 5 segundos quais as condições e níveis exatos da iluminação, temperatura e umidade.


###REQUISITOS DE HARDWARE
1x Placa Arduino
1x Fotoresistor LDR
1x Sensor de temperatura
1x Sensor integrado DHT11 (aqui representado com um potenciômetro)
1x Tela LCD 16x2
1x Buzzer
1x Protoboard
1x LED vermelho
1x LED amarelo
1x LED verde
5x Resistor 220 Ohm


###REQUISITOS DE SOFTWARE
Arduino IDE


###INSTALAÇÃO
Para utilizar este projeto, você precisará de:
* Um ambiente de desenvolvimento de sistemas de arduino e o código fornecido dentro do Tinkercad.
* Os materiais listados em "Requisitos".

1. Monte o sistema de arduino mostrado dentro da imagem do Tinkercad;
2. Conecte o arduino em um computador que possui o arduino IDE e faça upload do código mostrado dentro do link do Tinkercad.


###LINK TINKERCAD
https://www.tinkercad.com/things/dPdOiq5d3vR-copy-of-checkpoint-1-edge-computing-and-computer-systems/editel?sharecode=bRBw6KDVXH3Dg4FBL9Ub_hmIt20FhSmuJVYtuB1Rxks


###VIDEO SOBRE PROJETO
https://youtu.be/BcLCUqV64HY


###Grupo DeskTOPS
Enricco Rossi de Souza Carvalho Miranda | RM551717
Erick Carvalho Pereira | RM550772
Felipe de Vinicius Quinalha | RM98957
Gabriel Marquez Trevisan | RM99227
Silvia Kavabata | RM97650

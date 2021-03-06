

# Mastercard

## Roundtrip dos dados até a processadora
![alt text](https://github.com/thiagoliof/px/blob/master/roundtrip.jpg "roundtrip")

## Visão do modelo da processadora 

![alt text](https://github.com/thiagoliof/px/blob/master/arq.jpg "Arquitetura")


## Protocolo de comunicação MTI, Bitmaps e Data elements

Esses protocolos de comunicação são especificados no ISO 8583

fonte: https://en.wikipedia.org/wiki/ISO_8583

Segue alguns exemplos dos comandos enviados pelo servidor da Mastercard e seus devidos tratamentos:

| Tipo do Dado 	| Dado       	| Resultado    	| Regra                                                                       	|
|--------------	|------------	|--------------	|-----------------------------------------------------------------------------	|
| n 6          	| 201234     	| 201234       	| Campo numérico fixo com 6 posições                                          	|
| n 12         	| 10000      	| 000000010000 	| Campo numérico fixo com 12 posições                                         	|
| n 10         	| 1107221830 	| 1107221830   	| Campo numérico fixo com 10 posições                                         	|
| n 6          	| 123456     	| 123456       	| Campo numérico fixo com 6 posições                                          	|
| an ..25      	| A5DFGR     	| 06A5DFGR     	| Campo Alfanumérico com o máximo de 25 posições e dois dígitos de informação 	|

Para o processamento dessas mensagens o ideal é o uso de uma linguagem de baixo nível como o **Rusty**
https://www.rust-lang.org/learn/get-started



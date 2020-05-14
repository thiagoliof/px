

# Mastercard

## Arquitetura 

Inline-style: 
![alt text](https://github.com/thiagoliof/px/blob/master/arq.jpg "Arquitetura")


## Protocolo de comunicação MTI, Bitmaps e Data elements

Esses protocolos de comunicação são especificados no ISO 8583

fonte: https://en.wikipedia.org/wiki/ISO_8583

| Tipo do Dado 	| Dado       	| Resultado    	| Regra                                                                       	|
|--------------	|------------	|--------------	|-----------------------------------------------------------------------------	|
| n 6          	| 201234     	| 201234       	| Campo numérico fixo com 6 posições                                          	|
| n 12         	| 10000      	| 000000010000 	| Campo numérico fixo com 12 posições                                         	|
| n 10         	| 1107221830 	| 1107221830   	| Campo numérico fixo com 10 posições                                         	|
| n 6          	| 123456     	| 123456       	| Campo numérico fixo com 6 posições                                          	|
| an ..25      	| A5DFGR     	| 06A5DFGR     	| Campo Alfanumérico com o máximo de 25 posições e dois dígitos de informação 	|

Precisamos usar uma linguagem de baixo nível como **rusty**
https://www.rust-lang.org/learn/get-started



# O Programa Blink
O programa Blink é um dos exemplos mais básicos e tradicionais para quem está começando a trabalhar com microcontroladores, como o Arduino. Ele faz com que um LED pisque (ou "blink") repetidamente, ligando e desligando em intervalos regulares. Este exemplo é útil para testar se o ambiente de desenvolvimento e o hardware estão funcionando corretamente.

## Materiais necessários 
* Arduino Uno
* Protobord
* 01 Resistor 220 Ω
* 01 LED
* Fios de conexão

## Diagrama de montagem 
![Diagrama](https://github.com/Epaminondaslage/Aluno_Fulano_de_Tal/blob/main/Exercicio_em_Sala_1/Fig_pisca.jpg)

## Funcionamentos 
O código faz o LED embutido (geralmente conectado ao pino 13) ou um LED externo conectado a um pino digital piscar com intervalos de 1 segundo (1000 milissegundos). O ciclo de funcionamento é simples:

  1.O LED é ligado.
  2.Aguarda-se 1 segundo.
  3.O LED é desligado.
  4.Aguarda-se mais 1 segundo.
  
Este ciclo se repete indefinidamente enquanto o programa estiver em execução.

# Ligar e desligar o LED com o botão
Ao pressionar o botão liga o LED integrado no pino 13 da placa Arduino. O botão é conectado ao pino 2 (ou qualquer outra entrada digital) por um resistor pull-up de 10 kΩ. O resistor pull-up está conectado à terra. O outro contato do botão está conectado a uma fonte de alimentação de 5 V.

Quando o botão não é pressionado, o pino 2 da placa Arduino é conectado à terra por um resistor pull-up, e a entrada será LOW. Quando o botão é pressionado, a entrada digital será de 5V - nível HIGH.

É possível conectar este circuito ao contrário, com um resistor pull-up segurando a entrada HIGH e indo para o nível LOW quando o botão é pressionado. Nesse caso, o comportamento do esboço será invertido: o LED acende e apaga quando o botão é pressionado.

Se você desconectar a entrada digital do resistor, o LED poderá piscar aleatoriamente. Isso ocorre porque a entrada é "flutuante", o que significa que ela retorna aleatoriamente um nível HIGH ou LOW. É por isso que você precisa de um resistor pull-up.

## Materiais Necessários
* Arduino Uno
* 1 Botão de pressão
* 1 Resistor de 10 kΩ (pull-up)
* Fios de conexão (jumpers)
* Protoboard

## Diagrama
![WhatsApp Image 2024-09-20 at 21 30 30](https://github.com/user-attachments/assets/75e3ea34-e9a8-4b83-aa3c-d567c9959128)

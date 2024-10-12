# Projeto: Relógio com RTC DS3231 e Display 16x2 I2C

## Componentes Utilizados

 - **Arduino Uno**
  - Microcontrolador responsável por processar e exibir a hora e data no display LCD.

 - ## RTC DS3231 (Relógio de Tempo Real)
  - Um módulo que mantém o rastreamento preciso do tempo, mesmo quando o Arduino está desligado ou reiniciado. Esse módulo contém uma bateria de backup para garantir que o tempo seja mantido corretamente.


 - **Display LCD 16x2 com Interface I2C**
  - Permite a exibição de informações como a hora e a data. A interface I2C facilita a comunicação entre o display e o Arduino, utilizando apenas dois pinos (SDA e SCL) para enviar dados.



## Descrição do Projeto

Este projeto consiste em criar um relógio digital usando um Arduino Uno, um módulo RTC DS3231 e um Display LCD 16x2 com comunicação I2C. O objetivo é exibir a hora e a data no display de forma automática e precisa. O módulo RTC é responsável por manter o tempo atualizado, enquanto o Arduino lê os dados do RTC e os exibe no LCD.

## Funcionamento

### 1. Módulo RTC DS3231

O módulo RTC DS3231 é um relógio de tempo real que continua funcionando mesmo quando o sistema principal está desligado. Ele tem uma bateria de backup que garante que o tempo seja mantido com precisão. Assim que o Arduino é inicializado, ele verifica se o RTC está funcionando corretamente e, se necessário, ajusta a hora para a data e o tempo de compilação do código.

### 2. Exibição da Hora e Data no Display LCD

O Display LCD 16x2 é usado para mostrar a hora (em horas, minutos e segundos) e a data (dia, mês e ano). O Arduino se comunica com o display através da interface I2C, o que reduz a quantidade de pinos necessários para a conexão.

A linha superior do display exibe a hora atual no formato "HH:MM:SS".

A linha inferior exibe a data no formato "DD/MM/AAAA".


### 3. Atualização Automática

O sistema é programado para atualizar a hora e a data a cada segundo. Isso é feito através de um loop contínuo no Arduino, onde ele lê os valores atuais do módulo RTC e os exibe no LCD. O tempo é mantido com alta precisão, e a exibição é ajustada dinamicamente no display.

## Implementação

 - **1. Leitura de Dados do RTC**: O Arduino lê os dados de tempo (horas, minutos e segundos) e de data (dia, mês e ano) do módulo DS3231 a cada segundo.


 - **2. Exibição no Display LCD**: Os dados são formatados e exibidos no LCD, garantindo que a informação esteja clara e precisa.


 - **3. Manutenção do Tempo**: O módulo RTC DS3231 mantém o tempo mesmo quando o Arduino é desligado, garantindo que o relógio continue funcionando.

# Comunicação Serial e Controle de LEDs com RP2040 e BitDogLab 🎮💡

## Objetivos 🎯

Este projeto tem como objetivo consolidar os conceitos de comunicação serial em microcontroladores, com foco no RP2040 e na placa BitDogLab. Os principais objetivos são:

Compreender o funcionamento e a aplicação de comunicação serial (UART e I2C).

Manipular LEDs comuns e LEDs endereçáveis WS2812.

Trabalhar com botões de acionamento, interrupções e Debounce.

Desenvolver um projeto funcional que combine hardware e software.

## Descrição do Projeto 📝

O projeto utiliza os seguintes componentes conectados à placa BitDogLab:

Matriz 5x5 de LEDs (WS2812): Conectada à GPIO 7.

LED RGB: Com os pinos conectados às GPIO 11, GPIO 12 e GPIO 13.

Botão A: Conectado à GPIO 5.

Botão B: Conectado à GPIO 6.

Display SSD1306 (I2C): Conectado às GPIO 14 e GPIO 15.

## Funcionalidades ⚙️

### Modificação da Biblioteca font.h ✏️

Adicionar caracteres minúsculos à biblioteca font.h 

Criar novos caracteres de forma criativa para exibição no display SSD1306 

### Entrada de Caracteres via PC (Serial Monitor) 

Utilizar o Serial Monitor do VS Code para digitar os caracteres 

Cada caractere digitado deve ser exibido no display SSD1306 

Quando um número entre 0 e 9 for digitado, um símbolo correspondente ao número deve ser exibido na matriz 5x5 WS2812 

### Interação com o Botão A 🔘

Pressionar o Botão A alterna o estado do LED RGB Verde (ligado/desligado) 

O estado do LED deve ser registrado de duas formas:

Uma mensagem informativa sobre o estado do LED no display SSD1306 

Uma mensagem descritiva sobre a operação no Serial Monitor 

### Interação com o Botão B 🔘

Pressionar o Botão B alterna o estado do LED RGB Azul (ligado/desligado) 

O estado do LED deve ser registrado de duas formas:

Uma mensagem informativa sobre o estado do LED no display SSD1306 

Uma mensagem descritiva sobre a operação no Serial Monitor 

## Requisitos do Projeto 🛠️

Uso de Interrupções (IRQ): Todas as funcionalidades dos botões devem ser implementadas utilizando interrupções 

Debouncing: Implementar o tratamento de bouncing dos botões via software 

Controle de LEDs: O projeto deve usar LEDs comuns e LEDs WS2812, demonstrando controle de diferentes tipos de LEDs 

Utilização do Display SSD1306: Exibir caracteres maiúsculos e minúsculos para demonstrar o domínio do uso de bibliotecas e o protocolo I2C 

Envio de Informações pela UART: Comunicação serial via UART para envio de mensagens ao Serial Monitor

Organização do Código: O código deve ser bem estruturado, comentado e fácil de entender

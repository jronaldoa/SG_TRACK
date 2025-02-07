# SG Track

**SG Track** é um projeto que realiza comunicação serial entre um rastreador e um Arduino, integrando sensores e controle de dispositivos, como um sensor de chuva e módulo de MP3. O projeto foi desenvolvido para realizar a leitura de dados do rastreador e controlar o comportamento de dispositivos com base nesses dados.

## Funcionalidades

- **Comunicação Serial**: Recebe dados do rastreador via comunicação serial.
- **Controle de Status**: Exibe status e dados em um display LCD.
- **Sensores**: Integra um sensor de chuva para alterar comportamentos de controle.
- **Áudio**: Utiliza um módulo MP3 para tocar alertas e mensagens ao usuário.
- **Telemetria**: Envia e recebe dados periodicamente para controle remoto.

## Componentes Utilizados

- **Arduino**: Controla a lógica do projeto e gerencia as interações com os sensores e o display LCD.
- **Sensor de Chuva**: Para detecção de condições meteorológicas.
- **Módulo MP3 (JQ6500)**: Reproduz arquivos de áudio (alertas e mensagens).
- **LCD I2C**: Exibe informações de status e telemetria em tempo real.
- **Rastreador GPS**: Responsável por fornecer dados de localização e status do veículo.

## Como Funciona

1. O Arduino envia requisições periódicas para o rastreador via comunicação serial.
2. O rastreador retorna dados como status, localização e dados adicionais.
3. O Arduino processa esses dados, e conforme o estado do sensor de chuva ou a velocidade, altera a velocidade máxima permitida.
4. O sistema também toca áudios e exibe mensagens no display LCD.

## Requisitos

- **Arduino IDE**: Para compilar e fazer upload do código.
- **Bibliotecas**:
  - LiquidCrystal_I2C
  - SoftwareSerial
  - JQ6500_Serial
- **Placa Arduino**: Pode ser qualquer modelo compatível, como Arduino Uno ou Nano.

## Como Usar

1. Baixe o código fonte.
2. Abra o código no Arduino IDE.
3. Conecte o Arduino ao computador.
4. Carregue o código para a placa Arduino.
5. Conecte o rastreador, o sensor de chuva e o módulo MP3 ao Arduino conforme os pinos configurados no código.
6. Acompanhe os resultados no LCD e ouça os alertas sonoros.

## Licença

Este projeto é licenciado sob a [Licença MIT](LICENSE).

## Contribuindo

Se você deseja contribuir para o projeto, faça um fork do repositório e envie um pull request. As contribuições são bem-vindas!


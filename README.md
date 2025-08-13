# Smart-Planter
# Vaso Inteligente com Raspberry Pi e Interface Touchscreen

Bem-vindo ao repositório do Vaso Inteligente! Este é um projeto de automação residencial que visa cuidar de suas plantas de forma eficiente e interativa. Utilizando um Raspberry Pi 4, uma interface gráfica touchscreen e diversos sensores, este vaso automatiza a rega, monitora as condições do solo e da água, e fornece iluminação suplementar para o crescimento saudável da planta em ambientes fechados.

Toda a estrutura do vaso, incluindo os reservatórios e suportes, foi modelada em CAD e fabricada em uma impressora 3D, enquanto uma placa de circuito impresso (PCI) customizada foi desenvolvida para organizar e facilitar as conexões eletrônicas.

## 🌟 Funcionalidades Principais

* [cite_start]**Interface Gráfica Touchscreen**: Uma tela de 7 polegadas sensível ao toque permite a visualização e o controle de todas as funções do vaso. [cite: 4, 8]
* [cite_start]**Rega Automatizada e Manual**: Programe horários específicos para a irrigação ou acione a bomba de água manualmente com um único toque. [cite: 8, 232, 290]
* [cite_start]**Monitoramento de Sensores**: Acompanhe em tempo real o nível do reservatório de água e a umidade do solo. [cite: 5, 233, 234]
* [cite_start]**Iluminação para Crescimento (Grow Light)**: Uma fita de LED com espectro de luz específico para plantas pode ser ligada e desligada pela tela, potencializando o desenvolvimento em locais com pouca luz natural. [cite: 8]
* [cite_start]**Design Integrado e Modular**: O corpo do vaso, impresso em 3D, foi projetado para abrigar todos os componentes eletrônicos de forma organizada, com reservatórios separados para água e terra. [cite: 62, 68]

## 🛠️ Hardware Utilizado

| Componente | Descrição |
| :--- | :--- |
| **Processador** | [cite_start]Raspberry Pi 4 B, programado em Python. [cite: 6] |
| **Display** | [cite_start]Display Raspberry Pi 7" Touchscreen oficial. [cite: 4] |
| **Sensores** | [cite_start]Sensor de umidade de solo inoxidável e sensor de nível de água tipo boia. [cite: 5] |
| **Atuadores** | [cite_start]Mini Bomba D'Água Submersa e Fita de LED para cultivo. [cite: 4, 8] |
| **Placa de Circuito** | [cite_start]PCI customizada, projetada no software Proteus e fresada em uma CNC. [cite: 2, 36, 56] |
| **Fonte** | [cite_start]Fonte DC de 5 volts para alimentar todo o sistema. [cite: 4] |
| **Estrutura** | [cite_start]Peças modeladas e impressas em 3D com filamento PLA. [cite: 170, 188] |

## 💻 Software e Desenvolvimento

* [cite_start]**Linguagem de Programação**: Python. [cite: 6]
* [cite_start]**Sistema Operacional**: Raspbian, instalado em um cartão SD. [cite: 7]
* [cite_start]**Interface Gráfica (GUI)**: Desenvolvida com a biblioteca **PyQt5**, proporcionando uma interface visualmente agradável e funcional. [cite: 191]
* [cite_start]**Controle das GPIOs**: Utilização da biblioteca `RPi.GPIO` para interagir com os sensores e atuadores conectados ao Raspberry Pi. [cite: 247]
* [cite_start]**Modelagem 3D**: As peças mecânicas foram projetadas em software CAD e fatiadas no Simplify3D para a impressão. [cite: 187]
* [cite_start]**Design da PCI**: O esquemático e o layout da placa foram elaborados no software **Proteus**, e o processo de fresagem foi programado no **vCarve**. [cite: 36]

## 📊 Diagrama de Funcionamento

O fluxo do programa segue uma lógica clara para garantir o cuidado com a planta:

1.  [cite_start]**Início do Programa**: O sistema é inicializado. [cite: 303]
2.  [cite_start]**Leitura dos Sensores**: O sensor de nível e o de umidade realizam leituras e exibem os dados na tela. [cite: 304, 305]
3.  [cite_start]**Agendamento**: O usuário pode programar um horário específico para a rega. [cite: 307]
4.  [cite_start]**Verificação de Horário**: O sistema compara o horário atual com o agendado. [cite: 308]
    * [cite_start]Se for o horário, a planta é regada. [cite: 310]
    * [cite_start]Caso contrário, o sistema aguarda. [cite: 311]
5.  [cite_start]**Ação Manual**: A qualquer momento, o usuário pode apertar o botão "Regar" para acionar a bomba imediatamente. [cite: 309, 310]

---
[cite_start]*Este projeto foi desenvolvido no âmbito do OCEAN Brasil, com a colaboração de Jadson Maciel e Emanuel Silva, sob a supervisão de Almir Kimura Junior.* [cite: 30, 31, 177, 182]

# Impressora Braille com Arduino Mega

## Descrição do Projeto

Este projeto consiste no desenvolvimento de uma **impressora Braille de baixo custo**, capaz de converter textos digitados pelo usuário em **impressões físicas em Braille**.  
O sistema utiliza um **Arduino Mega** em conjunto com um **Shield CNC**, motores de passo e **solenoides**, permitindo o controle preciso da posição e da marcação dos pontos.

A solução foi pensada para aumentar a **acessibilidade de pessoas com deficiência visual**, oferecendo uma alternativa portátil e mais acessível às impressoras Braille comerciais.

---

## Recursos Utilizados

### Hardware

- Arduino Mega
- Shield CNC
- CNC com 3 motores de passo (eixos X e Y(Bi-motor))
- Solenoides (atuadores)
- Relés para acionamento dos solenoides
- Fonte de alimentação externa

### Software

- Interface própria para digitação e configuração do texto
- Firmware em Arduino para controle dos motores e solenoides
- Comunicação Serial entre computador e microcontrolador

---

## Arquitetura do Sistema

O projeto é dividido em duas partes principais:

### 1️Interface do Usuário (Software)

O usuário tem acesso a um software próprio que permite:

- Digitar o texto que será convertido em Braille
- Configurar:
  - Espaçamento entre letras
  - Espaçamento entre linhas
  - Tamanho dos pontos
  - Margens da página
- Acompanhar a impressão em **tempo real**
- Visualizar a correspondência entre caracteres e símbolos em Braille

### Comunicação com o Arduino

A interface envia os dados ao Arduino da seguinte forma:

- O texto é convertido em **matrizes de pontos Braille**
- Cada **linha** é enviada separadamente via **Serial**
- O Arduino só recebe a próxima linha após confirmar que a anterior foi impressa

### Controle no Arduino Mega

O Arduino é responsável por:

- Interpretar a matriz recebida
- Transformar os dados em coordenadas físicas (X e Y)
- Controlar os motores da CNC
- Acionar os **solenoides via relés** para marcar os pontos no papel
- Gerenciar:
  - Sistema de coordenadas
  - Comando de **Home**
  - Alternância inteligente entre dois solenoides para maior velocidade

---

## Esquema do Circuito (Fritzing)

> Substitua o arquivo abaixo pela imagem real do seu projeto.

![Esquema de ligação no Fritzing](./docs/fritzing_conexao.png)

---

## Vídeo do Projeto

> Substitua o link abaixo pelo link do seu vídeo (YouTube, por exemplo).

```html
<iframe 
  width="560" 
  height="315" 
  src="https://www.youtube.com/embed/SEU_VIDEO_AQUI" 
  title="Vídeo do Projeto - Impressora Braille"
  frameborder="0" 
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
  allowfullscreen>
</iframe>

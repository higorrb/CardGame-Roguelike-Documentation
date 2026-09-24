# CardGame-Roguelike

> **Protótipo de Jogo de Cartas (Em Desenvolvimento)**

Este projeto é um estudo técnico desenvolvido na **Godot Engine** utilizando **GDScript**. O objetivo principal é construir um sistema funcional de combate em turnos inspirado em jogos de *deckbuilding*, com foco em uma arquitetura modular e lógica de sistemas robusta.

## Funcionalidades Técnicas

* **Sistema de Combate em Turnos:** Gerenciamento de estados (*State Machine*) que controla com precisão as transições entre o turno do jogador e o turno da IA do inimigo.
* **Gerenciamento de Mão e Baralho:** Sistema responsável pelo manuseio de dados das cartas, cobrindo ações como comprar do baralho, limitar tamanho da mão e mover cartas para o descarte. Inclui uma interface interativa de *arrastar e soltar* (*drag and drop*) para ativação.
* **Mecânicas Baseadas em Dados:** Implementação de rolagens aleatórias (D4, D6, D20) com suporte a modificadores dinâmicos para cálculos de dano e cura.
* **Tomada de Decisão da IA:** Lógica de comportamento inimigo baseada em regras que avaliam a porcentagem de vida atual para decidir dinamicamente entre ações ofensivas (Ataque) ou defensivas (Cura).
* **Sistema de Efeitos de Status:** Estrutura escalável para aplicar e rastrear múltiplos efeitos de status (ex: Fraqueza, Crítico, Escudos e Cura Contínua).
* **UI Dinâmica e Feedback Visual:** Atualizações de HUD em tempo real, contando com sistema de texto flutuante (*Floating Combat Text*) e um registro detalhado de eventos (*Combat Log*).

## Tecnologias e Arquitetura

* **Engine:** Godot 4.3
* **Linguagem:** GDScript
* **Padrões de Projeto (*Design Patterns*):**
  * Comunicação baseada em **Sinais (*Signals*)** para desacoplamento completo da UI.
  * **Métodos Estáticos** para instanciação e manipulação otimizada de efeitos visuais.

## Documentação Visual

### 1. Sistema de Intenção e Status

A IA do inimigo exibe ícones indicando sua próxima ação e atualiza os modificadores de dano em tempo real com base nos efeitos de status ativos.

<img width="1272" height="717" alt="Sistema de Intenção e Status" src="https://github.com/user-attachments/assets/85c7ac27-d14d-4c0a-a9e8-87c00a626fba" />

---

### 2. Registro de Combate e Eventos

O sistema fornece um histórico detalhado de cada rolagem de dados e ação executada, garantindo total transparência no fluxo do jogo.

<img width="770" height="238" alt="Registro de Combate e Eventos" src="https://github.com/user-attachments/assets/b62a4819-70ce-43d3-9867-f9ea1dd18655" />

---

### 3. Feedback Visual (Texto Flutuante)

Cálculos de dano e cura em tempo real são exibidos diretamente sobre os alvos usando textos coloridos e animados.

<img width="1231" height="692" alt="Feedback Visual com Texto Flutuante" src="https://github.com/user-attachments/assets/8cacd5ab-765c-49a7-9ed0-e3193d6013eb" />


Documentação Visual

1. Sistema de Intenção e Status
A IA do inimigo exibe ícones indicando sua próxima ação e atualiza modificadores de dano com base nos efeitos de status ativos.

<img width="1272" height="717" alt="image" src="https://github.com/user-attachments/assets/85c7ac27-d14d-4c0a-a9e8-87c00a626fba" />

3. Registro de Combate e Eventos
O sistema fornece um histórico detalhado de cada rolagem de dados e ação executada, garantindo transparência nas mecânicas do jogo.

<img width="770" height="238" alt="image" src="https://github.com/user-attachments/assets/b62a4819-70ce-43d3-9867-f9ea1dd18655" />

3. Feedback Visual (Texto Flutuante)
Cálculos de dano e cura em tempo real são exibidos diretamente sobre as entidades por meio de rótulos com código de cores.

<img width="1231" height="692" alt="image" src="https://github.com/user-attachments/assets/8cacd5ab-765c-49a7-9ed0-e3193d6013eb" />

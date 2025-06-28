# GeraCalcFreqMoodle - Gerador de Cálculo de Frequência para Moodle

Uma ferramenta web simples e poderosa desenvolvida para auxiliar professores e educadores que utilizam a plataforma Moodle a automatizar o cálculo de frequência (presença) dos estudantes.

A aplicação gera uma fórmula compatível com o **Livro de Notas** do Moodle, que calcula a frequência final com base na participação do aluno nas atividades propostas, e não em suas notas.

## 🎯 O Problema que Resolve

Calcular a frequência no Moodle pode ser um processo manual e demorado. A plataforma permite cálculos complexos no Livro de Notas, mas criar a fórmula correta para registrar presença (ou seja, se o aluno entregou uma atividade, independentemente da nota) não é uma tarefa trivial. Esta ferramenta elimina essa complexidade, gerando a fórmula exata em segundos.

## ✨ Features

-   **Geração Automática de Fórmula:** Insira os IDs das atividades do Moodle e seus respectivos pesos para gerar a fórmula instantaneamente.
-   **Cálculo por Participação:** A lógica considera que o aluno esteve "presente" em uma atividade se obteve qualquer nota superior a zero.
-   **Pesos Configuráveis:** Atribua pesos diferentes para cada atividade, permitindo que algumas contem mais para a frequência final.
-   **Interface Simples:** Adicione ou remova campos de atividade de forma dinâmica.
-   **Cópia Fácil:** Um botão "Copiar para a área de transferência" facilita a inserção da fórmula no Moodle.
-   **Client-Side:** Funciona inteiramente no navegador, sem necessidade de servidor ou conexão com a internet.

## 🚀 Como Usar a Ferramenta

1.  **Acesse a Ferramenta:** Abra o arquivo `index.html` em seu navegador.
2.  **Identifique as Atividades no Moodle:**
    -   No Moodle, vá para "Configuração do Livro de Notas".
    -   Certifique-se de que cada atividade que contará para a frequência tenha um **Número de ID**. Se não tiver, você pode adicionar um (ex: `ativ1`, `prova1`, `trab1`).
3.  **Preencha os Campos na Ferramenta:**
    -   Para cada atividade, insira o **ID** (ex: `ativ1`) no campo da esquerda.
    -   No campo da direita, defina o **peso** daquela atividade para o cálculo da frequência (use `1` para pesos iguais).
    -   Clique no botão `<i class="fas fa-plus"></i> Adicionar item` se precisar de mais campos.
4.  **Gere e Copie a Fórmula:**
    -   Clique em `<i class="fas fa-calculator"></i> Gerar cálculo`.
    -   A fórmula completa aparecerá na área de texto.
    -   Clique em `<i class="fas fa-copy"></i> Copiar para a área de transferência`.
5.  **Cole no Moodle:**
    -   No Moodle, crie um novo **Item de nota** dentro de uma categoria de Frequência.
    -   Vá em "Editar" -> "Editar Cálculo" neste item.
    -   Cole a fórmula gerada no campo "Cálculo" e salve.

## 🛠️ Tecnologias Utilizadas

-   **HTML5**
-   **CSS3**
-   **JavaScript (Vanilla JS)**
-   **Font Awesome** (para os ícones)

## 📂 Como Executar Localmente

Como o projeto é feito apenas com tecnologias front-end, basta clonar ou baixar o repositório e abrir o arquivo `index.html` em qualquer navegador moderno.

```bash
git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/seu-usuario/seu-repositorio.git)
cd seu-repositorio
# Abra o arquivo index.html no navegador

Esta aplicação foi desenvolvida para a Universidade Federal de São Carlos (UFSCar) por Gidenilson Santiago, baseada em um algoritmo elaborado por Glauber Santiago, em 2020.


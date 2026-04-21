# Custo-Benefício de Jogos na Steam  
## Análise Exploratória do Valor Percebido pelo Jogador

---

## 1. Contexto

Diante da grande quantidade de jogos disponíveis na Steam, o jogador enfrenta dificuldade
para identificar quais títulos realmente oferecem bom valor pelo preço cobrado. Jogos podem
apresentar preços semelhantes, mas diferenças significativas em termos de tempo de jogo e
avaliação dos usuários, o que dificulta a comparação direta do valor percebido. Nesse cenário,
torna-se relevante utilizar dados para apoiar a decisão de compra, permitindo identificar quais
jogos oferecem melhor custo-benefício e quais podem estar sendo subvalorizados.
---

## 2. Storytelling

Um jogador com orçamento limitado deseja comprar um novo jogo, mas enfrenta uma
dúvida recorrente: será que o preço cobrado realmente corresponde à qualidade e ao tempo de
diversão que ele irá obter? Ao explorar a loja, ele encontra títulos com valores semelhantes, mas
sem uma forma clara de comparar o retorno que cada um oferece. Além disso, ele suspeita que
alguns jogos bem avaliados e com alto engajamento passam despercebidos por terem menor
popularidade. Diante disso, surge um problema analítico: como utilizar dados disponíveis para
identificar quais jogos oferecem melhor custo-benefício e quais títulos de alta qualidade estão
sendo subestimados?

---

## 3. Objetivo

Analisar os jogos pagos disponíveis na Steam com o propósito de comparar o valor
percebido dos títulos em relação ao custo por hora jogada, à avaliação dos usuários e à
popularidade estimada, do ponto de vista do jogador interessado em tomar decisões de compra
mais informadas, no contexto de uma análise exploratória baseada em dados públicos da
plataforma Steam.

---

## 4. Questões de Pesquisa

### Q1 — Custo-benefício por faixa de preço
A relação entre preço, tempo médio de jogo e avaliação dos usuários permite
identificar diferenças claras de custo-benefício entre os títulos pagos na Steam?

- H1: Existem diferenças observáveis de custo-benefício entre grupos de jogos
quando se considera preço, tempo de jogo e avaliação dos usuários.
- H0: Não é possível observar diferenças claras de custo-benefício entre os jogos ao
considerar preço, tempo de jogo e avaliação dos usuários

---

### Q2 — Identificação de Hidden Gems
É possível identificar, entre os jogos com menor número de proprietários, títulos
com alto custo-benefício que possam ser considerados hidden gems?

- H1: Existem jogos que combinam simultaneamente score de custo-benefício >=
P75, Steam Rating >= P75 e número de proprietários <= P25, configurando hidden
gem identificáveis no conjunto analisado.
- H0: Nenhum jogo satisfaz simultâneamente os três critérios de classificação de
forma relevante no conjunto analisado.

---

### Q3 — Retenção de jogadores
Jogos com melhor custo-benefício tendem a apresentar maior retenção de
jogadores ao longo do tempo?

- H1: Jogos com melhor custo-benefício tendem a apresentar maior permanência dos
jogadores ao longo do tempo
- H0: Não há uma tendência clara de que jogos com melhor custo-benefício
mantenham os jogadores por mais tempo

---

## 5. Métricas Utilizadas

### 5.1 Custo por Hora Jogada
Quanto o jogador paga, em média, por cada hora de jogo. Principal indicador de
custo-benefício

---

### 5.2 Steam Rating
Proporção de avaliações positivas em relação ao total de avaliações. Indica a
qualidade percebida pelo jogador

---

### 5.3 Score de Custo-Benefício
Pontuação composta que combina custo por hora e avaliação, permitindo
ordenar e comparar jogos de forma objetiva.
---

### 5.4 Hidden Gems
Classifica um jogo como hidden gem quando apresenta simultaneamente alto
custo-benefício, alta avaliação e baixa popularidade. Identifica títulos que o
jogador provavelmente não conhece mas que valeriam a compra.

---

### 5.5 Índice de Retenção
Classifica um jogo como hidden gem quando apresenta simultaneamente alto
custo-benefício, alta avaliação e baixa popularidade. Identifica títulos que o
jogador provavelmente não conhece mas que valeriam a compra.
---

## 6. Dataset

- Fonte: Steam Spy API  
- Aproximadamente 10.000 jogos  
- Unidade de análise: jogo individual  

---

## 7. Metodologia

A análise foi conduzida nas seguintes etapas:

1. Carregamento dos dados  
2. Limpeza e pré-processamento  
3. Cálculo das métricas  
4. Análise exploratória dos dados  
5. Avaliação das hipóteses propostas  

---

## 8. Tecnologias Utilizadas

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Jupyter Notebook  

---

## 11. Autores

- Wagner Oliveira de Quadros  
- João Victor Tubino Martins  

---


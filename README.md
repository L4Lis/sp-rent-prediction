# 🏠 SP Rent Prediction

Este repositório documenta meu primeiro estudo prático sobre Data Science, aplicado ao mercado imobiliário. Como estudante, meu objetivo é demonstrar o processo de análise de dados, desde o tratamento inicial até a criação de modelos preditivos.


## 📌 Status do Projeto
- [x] **Fase 1: Análise Exploratória de Dados (EDA)** - Concluído.
- [x] **Fase 2: Modelagem e Machine Learning** - Concluído.
- [x] **Fase 3: Avaliação de Resultados** - Concluído.


## 🔍 O que foi desenvolvido (Fase 1: EDA)

Nesta primeira etapa, foquei na Análise Exploratória de Dados (EDA). Algumas das principais decisões que tomei durante o processo:

* **Tratamento de Outliers:** Notei que valores extremos (acima de R$ 15.000) aumentavam a média de forma artificial. Optei por filtrar esses dados para focar no mercado residencial padrão.
* **Engenharia de Dados:** Limpei os nomes dos bairros na coluna `District` para facilitar a visualização e garantir gráficos mais legíveis.
* **Insights Extraídos:**
   * A área do imóvel (`Size`) é o fator de maior correlação com o preço (0.71).
   * Curiosamente, o número de vagas de garagem (`Parking`) mostrou-se mais impactante no valor do aluguel do que o número de quartos (`Rooms`).


## 🤖 O que foi desenvolvido (Fase 2 e 3: Modelagem)

Nesta etapa, transformei os insights da EDA em um modelo preditivo para estimar o valor do aluguel:

* **Preparação dos Dados (encoding):** Utilizei a técnica de One-Hot encoding, para transformar a coluna `District` em variáveis numéricas (o que resultou em 107 colunas para análise).
* **Algoritmo:** Utilizei Regressão Linear com a biblioteca Scikit-Learn.
* **Divisão de Dados:** Separei o dataset em 80% para treino e 20% para teste.
* **Performance:** O modelo alcançou um R² Score de 0.7414. Isso significa que as variáveis escolhidas explicam cerca de 74% da variação dos preços de aluguel em SP.


## 📈 Insights da Modelagem

O modelo revelou o "peso" financeiro de algumas variáveis. De acordo com os coeficientes da Regressão Linear, os bairros que mais aumentam o valor do aluguel no dataset são:

1. Iguatemi (+ R$ 4.316)
2. Itaim Bibi (+ R$ 3.327)
3. Vila Olímpia (+ R$ 2.457)


## 🛠️ Tecnologias e Bibliotecas:

* **Manipulação:** Pandas e Numpy.
* **Visualização:** Seaborn e Matplotlib.
* **Machine Learning:** Scikit-Learn (LinearRegression, train_test_split).
* **Persistência:** Joblib (para salvar o modelo treinado).


## 📂 Estrutura de Pastas

```
├── data/
│   ├── raw/            # Dados originais
│   └── processed/      # Dados limpos
├── models/             # Modelo treinado em pkl
├── notebooks/          # Notebooks de EDA e Modelagem
└── README.md
```

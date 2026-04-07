# 🏠 SP Rent Prediction

Este repositório documenta meu estudo prático sobre Ciência de Dados aplicada ao mercado imobiliário. Como estudante, meu objetivo aqui é demonstrar o processo de análise de dados, desde o tratamento inicial até a criação de modelos preditivos.

## 📌 Status do Projeto
- [x] **Fase 1: Análise Exploratória de Dados (EDA)** - Concluído.
- [ ] **Fase 2: Modelagem e Machine Learning** - 🟢 Em desenvolvimento.
- [ ] **Fase 3: Avaliação de Resultados** - Aguardando.

## 🔍 O que foi desenvolvido (Fase 1: EDA)

Nesta primeira etapa, foquei na Análise Exploratória de Dados (EDA). Algumas das principais decisões que tomei durante o processo:

* **Tratamento de Outliers:** Notei que valores extremos (acima de R$ 15.000) aumentavam a média de forma artificial. Optei por filtrar esses dados para focar no mercado residencial padrão.
* **Engenharia de Dados:** Limpei os nomes dos bairros na coluna `District` para facilitar a visualização e garantir gráficos mais legíveis.
* **Insights Extraídos:** * A área do imóvel (`Size`) é o fator de maior correlação com o preço (0.71).
    * Curiosamente, o número de vagas de garagem (`Parking`) mostrou-se mais impactante no valor do aluguel do que o número de quartos (`Rooms`).

## 🛠️ Tecnologias e Bibliotecas
Utilizei Python com as bibliotecas **Pandas** para manipulação, e **Seaborn/Matplotlib** para as visualizações estatísticas.

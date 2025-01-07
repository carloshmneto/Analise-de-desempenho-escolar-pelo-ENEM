# Analise-de-desempenho-escolar-pelo-ENEM

Esse projeto pretende analisar o desempenho escolar de diversos alunos ao redor do brasil, realizando uma comparação com diferentes variáveis socioeconômicas e observando correlações relevantes. Para isso, foi utilizada a base de dados de Microdados do ENEM 2022, com informações sobre todos os alunos inscritos no processo seletivo e suas respostas ao questionário socioeconômico obrigatório preenchido pelos mesmos. A partir desses dados, foram aplicadas diversas técnicas diferentes de modelos de dados para previsão da nota de cada estudante, utilizando modelos de tipo regressão, com métodos paramétricos (como Lasso, Ridge) e não paramétricos (como RandomForest, XGBoost).

## Como executar o projeto
Conta somente com os arquivos `codigo.ipynb`, junto com a base de dados. Para execução do projeto, deve-se baixar os dados fornecidos, fazer upload dos mesmos em um Drive pessoal, e a partir desse momento rodar o Notebook em uma plataforma que suporte esse tipo de arquivo, a fim de se obter os resultados.

## Resultados

| Modelo                     | MSE       | R²   |
|----------------------------|-----------|-------|
| Boosting                  | 5204.113  | 0.349 |
| Redes Neurais             | 5346.793  | 0.331 |
| Floresta Aleatória        | 5371.164  | 0.328 |
| Ridge                     | 5436.250  | 0.321 |
| Lasso                     | 5436.310  | 0.320 |
| Mínimos Quadrados         | 5459.920  | 0.322 |
| Forward Stepwise          | 5459.930  | 0.322 |
| K-Nearest Neighbours (KNN)| 5504.797  | 0.311 |

Baseando-se no menor MSE e maior R², o melhor modelo é o Boosting, que pertence à categoria de modelos não paramétricos. Isso sugere que modelos não paramétricos podem capturar melhor as relações não lineares ou complexas presentes nos dados. Por outro lado, os modelos paramétricos (como Ridge e Mínimos Quadrados) têm desempenho competitivo, mas geralmente assumem suposições mais rígidas sobre a estrutura dos dados. A escolha final dependerá do contexto mas, dados os resultados obtidos, os modelos não paramétricos aparentam ser mais adequados, inclusive por serem mais flexíveis em cenários com complexidade elevada.

## Contato
- [Meu LinkedIn](https://www.linkedin.com/in/carlos-neto-5668b0265/)
- Email: carloshmneto@usp.br

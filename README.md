# Demand Forecasting

Projeto de previsão de demanda utilizando histórico de vendas e Machine Learning.

# Observação

Os dados utilizados neste projeto são sintéticos e foram criados para fins de estudo e demonstração.

## Objetivo

Estimar a quantidade de unidades vendidas no próximo mês com base no histórico de vendas.

## Tecnologias utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Etapas do projeto

1. Carregamento dos dados
2. Tratamento das datas
3. Agregação das vendas por mês
4. Análise da demanda mensal
5. Criação de variáveis para o modelo
6. Separação entre treino e teste
7. Treinamento do modelo Random Forest
8. Avaliação do modelo
9. Comparação com um baseline
10. Previsão da demanda futura

## Modelo

Foi utilizado o `RandomForestRegressor` do Scikit-learn.

As variáveis utilizadas foram:

- Mês
- Ano
- Quantidade vendida no mês anterior

## Resultados

O modelo apresentou:

- MAE: 547,76 unidades
- RMSE: 568,90 unidades

Como comparação, um modelo baseline baseado na demanda do mês anterior apresentou MAE de 567,25 unidades.

A previsão realizada pelo modelo para setembro de 2026 foi de aproximadamente:

**8.879 unidades**

## Conclusão

O modelo conseguiu melhorar o erro em relação ao baseline, embora a diferença tenha sido pequena. O projeto demonstra um fluxo completo de Machine Learning aplicado à previsão de demanda, desde a preparação dos dados até a avaliação e previsão futura.

## Estrutura

```text
demand-forecasting/
├── data/
│   └── vendas.csv
├── models/
├── notebooks/
│   └── 01_previsao_demanda.ipynb
├── src/
├── .gitignore
└── README.md
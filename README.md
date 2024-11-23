# **Sistema de Previsão e Otimização de Carregamento de Veículos Elétricos 🚗⚡**
# Integrantes: Rodrigo Sakaguchi - RM88010 // Marcelo Kutudjian Filho - RM93124

## **Descrição do Projeto**
Este projeto visa a criação de um sistema de **Inteligência Artificial** para **otimizar o carregamento de veículos elétricos**. Utilizamos técnicas de **Machine Learning** para prever a demanda de energia em estações de carregamento, ajudando a otimizar a gestão dos recursos energéticos, reduzir custos e melhorar a eficiência energética.

## **Objetivo**
O objetivo é prever a quantidade de energia necessária (`kwhTotal`) para futuras sessões de carregamento, utilizando dados históricos e informações adicionais sobre as estações e sessões de carregamento. Com essa previsão, podemos otimizar o uso da infraestrutura de carregamento, economizar custos operacionais e garantir uma melhor gestão da energia disponível.

## **Dados Utilizados**
O projeto utiliza um dataset chamado `station_data_dataverse`(https://www.kaggle.com/datasets/michaelbryantds/electric-vehicle-charging-dataset?select=station_data_dataverse.csv)
que contém as seguintes colunas:

- **sessionId**: Identificador único da sessão de carregamento.
- **kwhTotal**: Quantidade total de energia carregada (em kWh).
- **dollars**: Custo da sessão de carregamento (em dólares).
- **chargeTimeHrs**: Tempo de carregamento (em horas).
- **distance**: Distância percorrida pelo veículo após o carregamento.
- **userId**: Identificador do usuário que realizou o carregamento.
- **stationId**: Identificador da estação de carregamento.
- **locationId**: Identificador da localização da estação.
- **managerVehicle**: Tipo ou categoria do veículo sendo carregado.
- **facilityType**: Tipo de instalação onde o carregamento ocorreu.

## **Tecnologias Utilizadas**
- **Python**: Linguagem principal para análise de dados e Machine Learning.
- **Pandas**: Para manipulação e análise dos dados.
- **NumPy**: Para operações matemáticas e tratamento de arrays.
- **Scikit-learn**: Biblioteca de Machine Learning usada para treinar o modelo.
- **Matplotlib** & **Seaborn**: Para visualização de dados e gráficos de desempenho do modelo.

## **Estrutura do Projeto**
1. **Carregamento e Análise de Dados**: Importação dos dados e análise exploratória para entender padrões e identificar possíveis problemas, como valores ausentes.
2. **Pré-processamento dos Dados**: Limpeza e transformação dos dados para preparar o dataset para o treinamento do modelo de Machine Learning.
3. **Treinamento do Modelo**: Utilização do algoritmo **Random Forest** para treinar o modelo preditivo baseado nos dados históricos.
4. **Avaliação do Modelo**: Avaliação do desempenho do modelo utilizando métricas como **MAE**, **MSE** e **RMSE**, e visualização dos resultados.

## **Resultados Obtidos**
Após o treinamento e avaliação do modelo, foram obtidos os seguintes resultados:

Erro Médio Absoluto (MAE): [Valor do MAE] - Indica a média dos erros em relação às previsões de energia, em kWh.
Erro Quadrático Médio (MSE): [Valor do MSE] - Mede a média dos erros ao quadrado, dando mais peso a erros maiores.
Raiz do Erro Quadrático Médio (RMSE): [Valor do RMSE] - Fornece uma métrica de erro na mesma unidade da variável prevista (kWh).
Os gráficos gerados mostram que o modelo foi capaz de capturar bem as tendências gerais da demanda de energia, embora haja algumas discrepâncias em situações específicas.

## **Conclusão**
O sistema desenvolvido foi eficaz em prever a demanda de energia para o carregamento de veículos elétricos. As previsões fornecidas pelo modelo de Machine Learning ajudam na otimização do uso de energia e na redução de custos operacionais. Utilizar essas previsões permite ajustar a operação das estações de carregamento para horários de menor custo e otimizar o uso da infraestrutura existente.

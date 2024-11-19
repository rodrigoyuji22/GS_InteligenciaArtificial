# **Sistema de Previsão e Otimização de Carregamento de Veículos Elétricos 🚗⚡**

## **Descrição do Projeto**
Este projeto visa a criação de um sistema de **Inteligência Artificial** para **otimizar o carregamento de veículos elétricos**. Utilizamos técnicas de **Machine Learning** para prever a demanda de energia em estações de carregamento, ajudando a otimizar a gestão dos recursos energéticos, reduzir custos e melhorar a eficiência energética.

## **Objetivo**
O objetivo é prever a quantidade de energia necessária (`kwhTotal`) para futuras sessões de carregamento, utilizando dados históricos e informações adicionais sobre as estações e sessões de carregamento. Com essa previsão, podemos otimizar o uso da infraestrutura de carregamento, economizar custos operacionais e garantir uma melhor gestão da energia disponível.

## **Dados Utilizados**
O projeto utiliza um dataset chamado `station_data_dataverse` que contém as seguintes colunas:

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

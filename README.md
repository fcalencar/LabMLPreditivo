# Previsão de Vendas de Sorvete com Machine Learning

## 🎯 Objetivo

O objetivo deste projeto é desenvolver uma solução de **regressão preditiva** utilizando Machine Learning para prever as vendas de sorvete com base na temperatura diária. Este projeto foi implementado na plataforma **Azure**, com foco em escalabilidade, rastreabilidade e reprodutibilidade.

## ✅ Principais metas do projeto

- **Treinar um modelo de Machine Learning** capaz de prever o volume de vendas de sorvete com base na temperatura do dia.
- **Registrar e gerenciar o ciclo de vida do modelo usando o MLflow**, facilitando o rastreamento de experimentos, versões e métricas.
- **Implementar o modelo em um ambiente de cloud computing (Azure)**, possibilitando previsões em tempo real via endpoints de inferência.
- **Construir um pipeline estruturado de Machine Learning**, garantindo um fluxo de trabalho automatizado e reprodutível para as etapas de treinamento, validação e testes.

## ☁️ Tecnologias e serviços utilizados

- **Azure Machine Learning** para desenvolvimento, versionamento e deployment de modelos.
- **MLflow** para rastreamento de experimentos e gerenciamento de modelos.
- **Azure Pipelines / Azure ML Pipelines** para automação de tarefas de ML.
- **Python** e bibliotecas como `scikit-learn`, `pandas`, `matplotlib`, entre outras.

## 🚀 Como executar

### Carregar o Dataset

- Vá para "Data" (Dados) no menu esquerdo.
- Clique em "Create" > "From local files".
- Escolha seu arquivo venda_sorvetes.csv.
- Defina o tipo como Tabular e clique em "Next".
- Use o delimitador correto (vírgula ,) e confirme as colunas (data, temperatura, venda).
- Salve o dataset.






## 🛠️ Publicar e Implantar (opcional)

Se o modelo for satisfatório:

- Registre o modelo no workspace.
- Crie um serviço de inferência.
- Gere uma API REST para consumir o modelo com novos dados.

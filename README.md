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

### 1. Carregar o Dataset

1. Vá para "Data" (Dados) no menu esquerdo.
2. Clique em "Create" > "From local files".
3. Escolha seu arquivo venda_sorvetes.csv.
4. Defina o tipo como Tabular e clique em "Next".
5. Use o delimitador correto (vírgula ,) e confirme as colunas (data, temperatura, venda).
6. Salve o dataset.

### 2. Criar um Compute Instance

1. No menu esquerdo, clique em **Compute**.
2. Na aba **Compute Instances**, clique em **+ New**.
3. Escolha um nome, tipo de máquina (por exemplo: `Standard_DS11_v2`) e clique em **Create**.
4. Aguarde o status mudar para **Running**.

### 3. Fazer Upload do Notebook

1. Vá para **Notebooks** no menu lateral.
2. Clique em **+ Upload** e selecione o arquivo `regressao_sorvetes.ipynb`.
3. Clique com o botão direito no notebook e escolha **Open in Notebook Editor**.

### 4. Executar o Notebook

1. No topo do editor de notebook, selecione o **Compute Instance** criado anteriormente.
2. Aguarde a conexão com o kernel (ícone verde).
3. Execute as células uma por uma (Shift + Enter) ou clique em **Run all**.

### 5. (Opcional) Fazer Upload do CSV

Se o arquivo `venda_sorvetes.csv` não estiver no ambiente, você pode:

1. Ir em **Notebooks > Files > Upload** e fazer o upload do `venda_sorvetes.csv`.
2. Certificar-se de que o caminho do arquivo no notebook esteja correto:
```python
df = pd.read_csv('venda_sorvetes.csv')
```

## 🛠️ Publicar e Implantar (opcional)

Se o modelo for satisfatório:

- Registre o modelo no workspace.
- Crie um serviço de inferência.
- Gere uma API REST para consumir o modelo com novos dados.

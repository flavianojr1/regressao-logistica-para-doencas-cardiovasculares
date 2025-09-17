# Projeto: Regressão Logística para Doenças Cardiovasculares

## Descrição
Este projeto utiliza um modelo de Regressão Logística para prever a probabilidade de pacientes apresentarem doenças cardiovasculares com base em dados históricos. O objetivo é construir um modelo preditivo eficiente e realizar análises exploratórias para entender melhor os fatores associados às doenças cardiovasculares.

## Estrutura do Projeto
O projeto está estruturado em um Jupyter Notebook com as seguintes etapas principais:

1. **Carregamento e Tratamento de Dados**:
   - Leitura da base de dados `CARDIO_BASE.csv`.
   - Tratamento de valores nulos e duplicados.
   - Análise de outliers e ajustes nos dados.

2. **Análise Exploratória de Dados (EDA)**:
   - Criação de gráficos para análise bivariada entre variáveis como idade, peso, colesterol e a presença de doenças cardiovasculares.
   - Geração de uma matriz de correlação para identificar relações entre as variáveis.

3. **Pré-processamento**:
   - Separação da base em treino e teste.
   - Padronização das variáveis para evitar viés no modelo.
   - Verificação do balanceamento dos dados.

4. **Treinamento do Modelo**:
   - Treinamento de um modelo de Regressão Logística.
   - Extração dos coeficientes e pontos de interceptação do modelo.
   - Avaliação das métricas de desempenho na base de treino.

5. **Teste do Modelo**:
   - Avaliação do modelo na base de teste.
   - Geração da curva AUC-ROC para análise do desempenho do modelo.

6. **Conclusões**:
   - Discussão sobre os resultados obtidos e insights gerados a partir do modelo e das análises.

## Requisitos
- Python 3.8+
- Bibliotecas:
  - pandas
  - matplotlib
  - seaborn
  - scikit-learn
  - imbalanced-learn

## Como Executar
1. Clone este repositório:
   ```bash
   git clone https://github.com/flavianojr1/regressao-logistica-para-doencas-cardiovasculares.git
   ```
2. Navegue até o diretório do projeto:
   ```bash
   cd regressao-logistica-para-doencas-cardiovasculares
   ```
3. Instale as dependências necessárias:
   ```bash
   pip install -r requirements.txt
   ```
4. Abra o arquivo Jupyter Notebook:
   ```bash
   jupyter notebook "Profissao Cientista de Dados M27 Pratique.ipynb"
   ```
5. Execute as células do notebook sequencialmente.

## Base de Dados
A base de dados utilizada neste projeto contém as seguintes variáveis:
- **age**: Idade dos pacientes.
- **gender**: Gênero (1: Homem, 2: Mulher).
- **height**: Altura dos pacientes (em cm).
- **weight**: Peso dos pacientes (em kg).
- **gluc**: Nível de glicose.
- **smoke**: Fumante (1: Sim, 0: Não).
- **alco**: Consumo de álcool (1: Sim, 0: Não).
- **active**: Realiza atividades físicas (1: Sim, 0: Não).
- **cardio_disease**: Presença de doença cardiovascular (1: Sim, 0: Não).

## Resultados
- O modelo apresentou uma acurácia de aproximadamente 64% tanto na base de treino quanto na base de teste.
- A curva AUC-ROC indicou um desempenho moderado do modelo.
- Variáveis como idade, peso e colesterol mostraram correlação positiva com a presença de doenças cardiovasculares.

## Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.

## Licença
Este projeto está licenciado sob a licença MIT.
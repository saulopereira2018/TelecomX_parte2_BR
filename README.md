# TelecomX_parte2_BR
# Autor: Saulo Pereira da Silva


📊 Análise de Evasão de Clientes (Churn) em Telecomunicações
Este projeto foca na análise e modelagem preditiva da evasão de clientes (churn) no setor de telecomunicações. Utilizaremos dados de clientes para identificar os principais fatores que levam à desistência do serviço e construir modelos de Machine Learning capazes de prever quais clientes têm maior probabilidade de evadir.

🎯 Objetivo do Projeto
O objetivo principal é identificar padrões e características de clientes que evadem, bem como desenvolver modelos preditivos que permitam à empresa tomar ações proativas para retenção.

🚀 Etapas do Projeto
O projeto é dividido nas seguintes etapas principais:

1. 📂 Extração e Carregamento de Dados
Carregar o dataset de clientes de telecomunicações (formato CSV) que foi previamente tratado e limpo.

Garantir que o arquivo contém apenas as colunas relevantes, com dados corrigidos e padronizados da parte 1 do desafio Telecom X.

2. 🧹 Pré-processamento de Dados
Remoção de Colunas Irrelevantes: Eliminar colunas que não agregam valor à análise ou aos modelos preditivos, como identificadores únicos de cliente (customerID).

Encoding de Variáveis Categóricas: Transformar variáveis textuais (categóricas) em formato numérico, utilizando OneHotEncoder, para torná-las compatíveis com algoritmos de Machine Learning.

Verificação e Balanceamento de Classes: Analisar a proporção da variável alvo (Churn) para identificar desequilíbrios. Se necessário, aplicar técnicas de balanceamento de classes como SMOTE para criar um dataset mais equilibrado, o que é crucial para o desempenho do modelo em classes minoritárias.

3. 📈 Análise Exploratória e Seleção de Variáveis
Análise de Correlação: Visualizar a matriz de correlação entre as variáveis numéricas para identificar relacionamentos, especialmente com a variável Churn.

Análises Direcionadas: Investigar a relação de variáveis-chave como tenure (tempo de contrato) e TotalCharges (total gasto) com a evasão, utilizando gráficos como boxplots.

Normalização/Padronização: Preparar os dados numéricos utilizando StandardScaler para modelos que são sensíveis à escala (ex: Regressão Logística, KNN). Modelos baseados em árvore (ex: Árvore de Decisão, Random Forest) não exigem essa etapa.

4. 🤖 Modelagem Preditiva
Separação de Dados: Dividir o dataset em conjuntos de treino e teste (com uma proporção comum de 70/30 ou 80/20) para avaliar o desempenho dos modelos de forma justa. A estratificação pela variável alvo é aplicada para manter a proporção de Churn em ambos os conjuntos.

Criação e Treinamento de Modelos: Construir e treinar pelo menos dois modelos de Machine Learning distintos:

Regressão Logística: Um modelo linear que exige dados padronizados.

Árvore de Decisão: Um modelo baseado em árvore que não necessita de padronização.

Avaliação do Modelo: Avaliar o desempenho de cada modelo utilizando métricas como Relatório de Classificação (Precision, Recall, F1-Score) e Matriz de Confusão.

5. 📋 Interpretação e Conclusões
Análise de Importância das Variáveis: Investigar quais variáveis são mais relevantes para a previsão de evasão em cada modelo:

Regressão Logística: Analisar os coeficientes para entender a contribuição de cada variável.

Árvore de Decisão: Utilizar a funcionalidade feature_importances_ para identificar as variáveis mais impactantes.

Relatório Final: Elaborar um relatório detalhado destacando os principais fatores que influenciam a evasão, comparando o desempenho dos modelos e propondo estratégias de retenção de clientes baseadas nos insights obtidos.

🛠️ Ferramentas e Bibliotecas Utilizadas
Python

Pandas: Manipulação e análise de dados.

NumPy: Suporte a operações numéricas.

Matplotlib e Seaborn: Visualização de dados.

Scikit-learn (sklearn): Pré-processamento de dados, modelos de Machine Learning e avaliação de modelos.

Imbalanced-learn (imblearn): Para técnicas de balanceamento de classes (ex: SMOTE).

⚙️ Como Executar o Projeto
Clone o Repositório: (Assumindo que o código estará em um repositório)

Bash

git clone <URL_DO_REPOSITORIO>
cd <NOME_DO_REPOSITORIO>
Preparação do Ambiente:

Certifique-se de ter o Google Colab configurado ou um ambiente Python com as bibliotecas listadas instaladas.

Instale as bibliotecas necessárias:

Bash

pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
Carregue o Dataset:

Faça o upload do seu arquivo CSV tratado (ex: TelecomX_Tratado.csv) para o ambiente do Google Colab (via menu "Arquivos" > "Fazer upload") ou monte seu Google Drive e forneça o caminho correto no script.

Execute o Notebook/Script:

Abra o arquivo .ipynb (se for um notebook Jupyter/Colab) ou execute o script Python (.py) célula por célula ou o arquivo completo.

🤝 Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests.


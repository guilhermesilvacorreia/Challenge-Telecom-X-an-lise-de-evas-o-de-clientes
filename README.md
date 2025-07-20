# Previsão de Evasão de Clientes para a Telecom X

 

Este projeto de Data Science tem como objetivo desenvolver um modelo de Machine Learning capaz de prever a evasão de clientes (churn) para uma empresa fictícia do setor de telecomunicações, a "Telecom X". A partir de um conjunto de dados contendo informações contratuais e de faturamento, o pipeline completo foi construído, desde o tratamento dos dados até a avaliação de modelos e a proposição de estratégias de retenção baseadas nos insights gerados.

## 🎯 Objetivos do Projeto

- **Preparar os dados para modelagem:** Realizar limpeza, tratamento e normalização.
- **Analisar e tratar o desbalanceamento de classes:** Utilizar a técnica SMOTE para criar um conjunto de dados de treino robusto.
- **Treinar e comparar múltiplos modelos de classificação:** Avaliar o desempenho da Regressão Logística e do Random Forest.
- **Avaliar o desempenho dos modelos:** Utilizar métricas como Acurácia, Precisão, Recall e F1-Score.
- **Identificar os principais fatores de evasão:** Analisar a importância das variáveis (feature importance) do melhor modelo.
- **Propor ações estratégicas:** Traduzir os resultados técnicos em recomendações de negócio para a equipe de retenção.

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** Python 3
- **Bibliotecas Principais:**
  - `Pandas`: para manipulação e análise de dados.
  - `Numpy`: para operações numéricas.
  - `Matplotlib` e `Seaborn`: para visualização de dados.
  - `Scikit-learn`: para pré-processamento, modelagem e avaliação.
  - `Imbalanced-learn`: para balanceamento de classes (SMOTE).
- **Ambiente:** Jupyter Notebook / Google Colab

## 🚀 Como Executar o Projeto

Siga as instruções abaixo para executar a análise em seu ambiente local.

### Pré-requisitos

- Python 3.8 ou superior
- `pip` (gerenciador de pacotes do Python)

### Instalação

1.  Clone o repositório para a sua máquina local:
    ```bash
    git clone [URL_DO_SEU_REPOSITORIO]
    ```
2.  Navegue até o diretório do projeto:
    ```bash
    cd nome-do-diretorio-do-projeto
    ```
3.  Instale as dependências necessárias:
    ```bash
    pip install -r requirements.txt
    ```
    *(**Nota:** Se o arquivo `requirements.txt` não existir, você pode instalá-las manualmente: `pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn jupyterlab`)*

### Execução

1.  Certifique-se de que o arquivo de dados `dados_tratados.csv` está no mesmo diretório do notebook.
2.  Inicie o Jupyter Lab (ou Jupyter Notebook):
    ```bash
    jupyter lab
    ```
3.  Abra o arquivo do notebook (`analise_evasao_telecom_x.ipynb`, por exemplo).
4.  Execute as células do notebook em ordem sequencial para replicar a análise e os resultados.

## 📈 Resumo dos Resultados

- **Análise Inicial:** O conjunto de dados original era desbalanceado, com aproximadamente 26% dos clientes classificados como "evasão". A técnica SMOTE foi aplicada com sucesso no conjunto de treino para corrigir esse viés.
- **Modelo Campeão:** O modelo **Random Forest** apresentou o melhor desempenho geral, superando a Regressão Logística, especialmente nas métricas mais importantes para o problema de negócio.

| Métrica | **Random Forest** |
| :--- | :---: |
| Acurácia | 0.76 |
| Precisão | 0.62 |
| Recall | **0.54** |
| F1-score | **0.58** |

- **Principais Fatores de Evasão:** As variáveis que mais influenciaram a previsão de evasão, segundo o modelo, foram:
  1.  `Faturamento_Total`
  2.  `Meses_Contrato`
  3.  `Faturamento_Mensal`

## 💡 Conclusões e Ações Estratégicas

Com base na análise, foram propostas três estratégias de retenção:
1.  **Criação de um Sistema de Pontuação de Risco:** Utilizar o modelo para gerar uma lista priorizada de clientes para a equipe de retenção contatar.
2.  **Programa de Fidelidade para Novos Clientes:** Focar em ações de engajamento para clientes com poucos meses de contrato.
3.  **Análise de Percepção de Valor:** Investigar o motivo da evasão em clientes com faturas mensais altas, mas que são recentes na base.

## ✒️ Autor

- **[Guilherme Silva]**
- [Seu LinkedIn ](www.linkedin.com/in/guilherme-silva-ti)
- [Seu GitHub ](https://github.com/guilhermesilvacorreia)

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.
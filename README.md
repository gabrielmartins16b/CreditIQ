# 💳 CreditIQ — Previsão de Score de Crédito com Machine Learning

> Modelo de Inteligência Artificial para classificação automática do score de crédito de clientes bancários em **Bom**, **Ok** ou **Ruim**.

---

## 📋 Sobre o Projeto

Este projeto foi desenvolvido para um banco com o objetivo de automatizar a análise de crédito dos seus clientes. A partir de dados históricos de clientes, são treinados modelos de Machine Learning capazes de prever o score de crédito de novos clientes de forma rápida e precisa.

O score de crédito é classificado em três categorias:

| Categoria | Significado |
|-----------|-------------|
| 🟢 Good   | Boa situação de crédito |
| 🟡 Standard | Situação de crédito regular (Ok) |
| 🔴 Poor   | Má situação de crédito |

---

## 🚀 Funcionalidades

- Importação e exploração da base de dados de clientes
- Pré-processamento e codificação de variáveis categóricas com `LabelEncoder`
- Treinamento de dois modelos de IA:
  - 🌳 **Random Forest** (Árvore de Decisão)
  - 📍 **K-Nearest Neighbors (KNN)**
- Avaliação de acurácia e seleção do melhor modelo
- Análise das features mais importantes para determinar o score
- Previsão automática do score de crédito para novos clientes

---

## 🧰 Tecnologias Utilizadas

- **Python 3**
- [Pandas](https://pandas.pydata.org/) — Manipulação e análise de dados
- [Scikit-learn](https://scikit-learn.org/) — Machine Learning
  - `RandomForestClassifier`
  - `KNeighborsClassifier`
  - `LabelEncoder`
  - `train_test_split`
  - `accuracy_score`

---

## 📁 Estrutura do Projeto

```
creditiq/
│
├── inicial.ipynb           # Notebook principal com todo o pipeline
├── clientes.csv            # Base de dados de clientes para treino
├── novos_clientes.csv      # Base de novos clientes para previsão
└── README.md               # Documentação do projeto
```

---

## ⚙️ Como Executar

### 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/creditiq.git
cd creditiq
```

### 2. Instale as dependências

```bash
pip install pandas scikit-learn
```

### 3. Adicione os arquivos de dados

Coloque os arquivos `clientes.csv` e `novos_clientes.csv` na raiz do projeto.  
> Os arquivos originais da aula estão disponíveis [aqui](https://drive.google.com/drive/folders/1FbDqVq4XLvU85VBlVIMJ73p9oOu6u2-J?usp=drive_link).

### 4. Execute o notebook

Abra e execute o arquivo `inicial.ipynb` no Jupyter Notebook ou JupyterLab:

```bash
jupyter notebook inicial.ipynb
```

---

## 🔄 Pipeline do Projeto

```
1. Entender o desafio do negócio
       ↓
2. Importar a base de dados (clientes.csv)
       ↓
3. Pré-processar os dados (LabelEncoder)
       ↓
4. Separar em treino (70%) e teste (30%)
       ↓
5. Treinar os modelos (Random Forest + KNN)
       ↓
6. Avaliar a acurácia e escolher o melhor modelo
       ↓
7. Prever o score de novos clientes
```

---

## 📊 Resultados

O modelo de **Random Forest** apresentou o melhor desempenho e foi selecionado para realizar as previsões em novos clientes. A análise de importância das features revelou quais características dos clientes mais influenciam na definição do score de crédito.

---

## 🤝 Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir uma *issue* ou enviar um *pull request*.

---

## 📄 Licença

Este projeto está sob a licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.

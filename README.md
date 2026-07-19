# Falhou? Eu Avisei AI

## 📖 Sobre o projeto

O **Falhou? Eu Avisei AI** é um modelo de Machine Learning desenvolvido para prever falhas em máquinas industriais a partir de dados operacionais e de processo. O objetivo é identificar, com antecedência, equipamentos com maior probabilidade de falha, permitindo que ações de manutenção sejam realizadas antes que ocorram paradas inesperadas.

A solução foi desenvolvida como projeto avaliativo do Módulo 1 do curso de Desenvolvimento de IA para Análise Preditiva e contempla todas as etapas de um pipeline de Machine Learning, desde a análise exploratória dos dados até o treinamento e avaliação de modelos preditivos.

---

## 🎯 Problema que o software resolve

O software resolve o problema de tentar prever quais máquinas de uma indústria vão falhar. Com essa informação os funcionários podem se preparar para trocar ou consertar as máquinas, reduzindo despesas, paradas não programadas da produção ou desperdício de recursos.

---

## 📊 Dados

O projeto utiliza um conjunto de dados sobre máquinas industriais. As variáveis usadas para treinar o modelo são: 

- Tipo;
- Temperatura do ar;
- Temperatura do processo;
- Velocidade de rotação;
- Torque;
- Desgaste da ferramenta;

A variável alvo do problema é:

- **falha_maquina**

---

## ⚙️ Etapas do projeto

O desenvolvimento foi dividido nas seguintes etapas:

1. Análise exploratória (EDA);
2. Limpeza e tratamento dos dados (Data Prep);
3. Feature Engineering;
4. Divisão e balanceamento dos dados;
5. Escalonamento de variáveis;
6. Ajuste de parâmetros e combate ao overfitting;
7. Avaliação da Acurácia e Veredito Final;

---

## 🧠 Modelos utilizados

Foram treinados dois modelos de classificação:

- K-Nearest Neighbors (KNN)
- Árvore de Decisão (Decision Tree)

Os hiperparâmetros avaliados foram:

### KNN

- K = 3
- K = 5
- K = 7

### Árvore de Decisão

- max_depth = 3
- max_depth = 5
- max_depth = None

---

## 🛠️ Técnicas utilizadas

Durante o desenvolvimento foram aplicadas diversas técnicas de Ciência de Dados, incluindo:

- Análise Exploratória de Dados (EDA);
- Tratamento de valores ausentes;
- Detecção de duplicatas;
- Feature Engineering;
- Balanceamento de classes utilizando SMOTE;
- Padronização de variáveis com StandardScaler;
- Divisão em treino e teste utilizando Stratified Sampling;
- Ajuste de hiperparâmetros;
- Avaliação utilizando acurácia.

---

## 💻 Tecnologias e bibliotecas utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn
- Jupyter Notebook
- Ipykernel
- Python-dotenv

---

## 📈 Fluxo do projeto

```text
Dataset
    │
    ▼
Análise Exploratória
    │
    ▼
Limpeza dos Dados
    │
    ▼
Feature Engineering
    │
    ▼
Divisão Treino/Teste
    │
    ▼
Balanceamento (SMOTE)
    │
    ├──────────────┐
    ▼              ▼
StandardScaler   Árvore de Decisão
(KNN)
    │              │
    ▼              ▼
Treinamento dos Modelos
    │
    ▼
Avaliação
```

---

## ▶️ Como executar

### 1. Clone o repositório

```bash
git clone https://github.com/CherylHenkels/sctec-projeto1.git
```

### 2. Acesse a pasta

```bash
cd sctec-projeto1
```

### 3. Crie um ambiente virtual

```bash
python -m venv .venv
```

### 4. Ative o ambiente virtual

Linux/macOS

```bash
source .venv/bin/activate
```

Windows

```bash
.venv\Scripts\activate
```

### 5. Instale as dependências

```bash
pip install -r requirements.txt
```

### 6. Execute o notebook

Abra e execute o arquivo `main.ipynb`.

---

## 📌 Estrutura do projeto

```text
.
├── data/
│   ├── anotações do Departamento de Engenharia.docx
│   └── manutencao_preditiva.csv
├── output/
│   └── Imagens geradas no notebook
├── main.ipynb
├── requirements.txt
├── README.md
└── .gitignore
```

---

## 🚀 Melhorias futuras

Algumas melhorias que podem ser implementadas são:

- Avaliar outros modelos;
- Selecionar variáveis a partir de feature importance;
- Testar retirar variáveis correlacionadas;
- Desenvolver um front-end para o modelo;

---

## 🎥 Video de demonstração

https://drive.google.com/file/d/1VVfb7-ftdTvmr5aPQqgO0aSECfT_qV3P/view?usp=sharing

---

## 👩‍💻 Autora

Projeto desenvolvido por [**Cheryl Henkels**](https://github.com/CherylHenkels)

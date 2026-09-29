# Forest Cover Type - IA Analysis 🌲📈

Este projeto consiste em uma análise completa e no desenvolvimento de modelos de inteligência artificial (Machine Learning) para classificar tipos de cobertura florestal com base em dados estritamente cartográficos e ecológicos, sem o uso de sensoriamento remoto.

## 🎯 Objetivos do Projeto
O trabalho foi estruturado para cumprir rigorosamente os seguintes requisitos de análise acadêmica/científica:
- Breve descrição das características e as classes do classificador.
- Análise Exploratória de Dados (EDA) compreensiva.
- Separação e tratamento dos dados.
- Treinamento de diversos Modelos de Classificação.
- Ilustração das Matrizes de Confusão.
- Extração de Métricas de precisão, revocação, f1-score e acurácia.
- Discussão aprofundada dos resultados frente ao desbalanceamento das classes.

## 📊 Conjunto de Dados (Dataset)
Os dados foram extraídos da base pública **UC Irvine Machine Learning Repository**, especificamente o dataset [Covertype (ID: 31)](https://archive.ics.uci.edu/dataset/31/covertype).

- **Total de Observações:** ~581.000 células geográficas de 30x30m.
- **Variável Alvo (Target):** `Cover_Type` (7 classes possíveis, variando de Pinheiros a Álamos).
- **Features Preditoras:** 54 variáveis (10 contínuas, referentes a medições topográficas e de luz solar, e 44 binárias One-Hot referentes aos tipos de solo e áreas de preservação).

## 🧠 Modelos Treinados
O pipeline de *Machine Learning* foi alimentado com dados escalonados via `StandardScaler` e incluiu o treinamento dos seguintes algoritmos:
1. Regressão Logística
2. Árvore de Decisão
3. Naive Bayes (Gaussian)
4. Rede Neural: Perceptron Simples
5. Rede Neural: Multi-Layer Perceptron (MLP) *(com 2 camadas ocultas de 50 e 20 neurônios)*
6. K-Nearest Neighbors (KNN)

## 🛠️ Tecnologias e Bibliotecas Utilizadas
- `Python 3.x`
- `ucimlrepo` (Para requisição e carga da base de dados)
- `pandas` e `numpy` (Manipulação de DataFrames e Arrays)
- `matplotlib` e `seaborn` (Visualização gráfica e Heatmaps)
- `scikit-learn` (Pré-processamento, Treinamento e Métricas)

## 🚀 Como Executar

1. Clone este repositório.
2. Certifique-se de instalar as dependências (você pode fazer isso via pip ou criar um ambiente virtual).
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn ucimlrepo
   ```
3. Abra e execute o notebook principal `main_notebook.ipynb` em sequência (célula por célula) para observar as etapas desde o download dos dados até o veredito final com o gráfico comparativo de F1-Score vs Acurácia.

---
Desenvolvido para fins de estudo e aprofundamento prático no pipeline de Data Science e Classificação de Machine Learning.
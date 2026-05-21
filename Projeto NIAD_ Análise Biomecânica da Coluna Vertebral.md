# Projeto NIAD: Análise Biomecânica da Coluna Vertebral

## 📄 Descrição do Projeto

Este projeto foi desenvolvido como parte do entregável da Trilha de Aprendizado do NIAD (Núcleo de Ciência de Dados e Inteligência Artificial), com foco em **Análise, Limpeza e Modelagem Preditiva**. O objetivo principal é aplicar técnicas de Machine Learning para classificar a condição da coluna vertebral (Normal ou Anormal) com base em um conjunto de características biomecânicas.

## 📊 Dataset Escolhido

O dataset utilizado para este projeto é o **"Vertebral Column Dataset"** [1], que contém dados biomecânicos de 310 pacientes, cada um classificado como "Normal" ou "Anormal" em relação à sua coluna vertebral. As características incluem:

*   `pelvic incidence`
*   `pelvic tilt`
*   `lumbar lordosis angle`
*   `sacral slope`
*   `pelvic radius`
*   `grade of spondylolisthesis`

## 🎯 Principais Desafios

Os principais desafios enfrentados neste projeto incluíram:

1.  **Limpeza e Pré-processamento de Dados:** Garantir a qualidade dos dados, tratando valores nulos e outliers para evitar distorções nos modelos.
2.  **Análise Exploratória de Dados (EDA):** Compreender as distribuições das variáveis, suas relações e identificar padrões que pudessem influenciar a classificação.
3.  **Engenharia de Variáveis:** Preparar os dados para os modelos de Machine Learning, incluindo a codificação da variável alvo e a padronização das features numéricas.
4.  **Modelagem Preditiva:** Selecionar, treinar e otimizar modelos de classificação (Random Forest e Gradient Boosting) para obter a melhor performance possível na previsão da condição da coluna vertebral.
5.  **Avaliação do Modelo:** Interpretar métricas de desempenho como Acurácia, F1-Score e Matriz de Confusão para validar a eficácia dos modelos.

## 📈 Interpretação dos Resultados

Após a aplicação das etapas de limpeza, EDA, engenharia de variáveis e modelagem, os modelos de Machine Learning foram capazes de classificar a condição da coluna vertebral com alta precisão. As métricas de avaliação, como o F1-Score e a acurácia, indicaram um bom desempenho, demonstrando a capacidade dos modelos em distinguir entre colunas "Normal" e "Anormal".

As matrizes de confusão geradas para cada modelo forneceram insights detalhados sobre os tipos de erros (falsos positivos e falsos negativos), permitindo uma compreensão mais aprofundada da performance do classificador.

## 📁 Estrutura do Repositório

```
.
├── main_fixed.ipynb          # Notebook Jupyter com a análise completa, limpeza, EDA e modelagem
├── Dataset_spine.csv         # Dataset original utilizado no projeto
├── Entregáveldalistadeaprendizado-1.pdf # PDF com as instruções do projeto
├── README.md                 # Este arquivo
└── graficos_coluna/          # Diretório contendo os gráficos gerados durante a EDA e avaliação dos modelos
    ├── 01_distribuicao_class_att.png
    ├── 02_distribuicao_numericas.png
    ├── 03_correlacao.png
    ├── 04_confusion_matrix_rf.png
    └── 05_confusion_matrix_gb.png
```

## 🔗 Referências

[1] **Vertebral Column Dataset**: Disponível em [https://www.kaggle.com/datasets/uciml/biomechanical-features-of-orthopedic-patients](https://www.kaggle.com/datasets/uciml/biomechanical-features-of-orthopedic-patients)

# Projeto NIAD: Inteligência Artificial na Biomecânica da Coluna Vertebral

## 📄 Descrição do Projeto
Este projeto foi desenvolvido como o entregável final da Trilha de Aprendizado do **NIAD (Núcleo de Inteligência Artificial e Ciência de Dados)**. O objetivo principal foi criar um sistema de classificação capaz de diagnosticar automaticamente condições da coluna vertebral (Normal vs. Anormal) utilizando medidas biomecânicas.

A implementação foca na **qualidade dos dados através de uma limpeza estatística rigorosa**, permitindo que o modelo **Random Forest** opere com máxima eficiência de forma simples e direta.

## 🎯 Estratégia Técnica

### 1. Limpeza de Dados (Tratamento de Outliers via IQR)
Para evitar que o modelo aprendesse padrões distorcidos por erros de medição ou casos extremos, aplicamos a técnica de **Amplitude Interquartil (IQR)**:
* **Identificação:** Calculamos os quartis (Q1 e Q3) para cada variável numérica.
* **Filtro:** Removemos registros que estavam fora dos limites estatísticos aceitáveis ($Q1 - 1.5 \times IQR$ e $Q3 + 1.5 \times IQR$).
* **Impacto:** Isso resultou em um dataset mais estável, focado na biologia real da maioria dos pacientes.



[Image of Box plot showing outliers and IQR]


### 2. O Modelo: Random Forest (Floresta Aleatória)
Optamos pelo **Random Forest Classifier** por ser um algoritmo de "ensemble" extremamente resiliente:
* **Simplicidade:** O modelo não exige normalização ou padronização de escala, mantendo as grandezas físicas originais.
* **Robustez:** Ele utiliza múltiplas árvores de decisão que votam no resultado, o que previne o "overfitting" e aumenta a confiabilidade do diagnóstico.



## 📈 Interpretação dos Resultados
O modelo final atingiu uma **Acurácia de 84%**.

* **Matriz de Confusão:** O gráfico demonstra que o modelo é particularmente eficaz em identificar casos **Anormais**, o que é o foco principal para triagem e rastreio médico biomecânico.
* **Objetividade:** Ao focar no Random Forest e na limpeza IQR, o código tornou-se modular e fácil de explicar em uma apresentação técnica.



## 📁 Estrutura do Repositório
* `main_fixed.ipynb`: Notebook Jupyter com o código completo de limpeza, treinamento e visualização.
* `Dataset_spine.csv`: Base de dados original utilizada.
* `README.md`: Documentação das decisões técnicas e resultados.

## 🛠️ Tecnologias
* **Linguagem:** Python
* **Bibliotecas:** Pandas, NumPy, Scikit-Learn e Matplotlib.

---

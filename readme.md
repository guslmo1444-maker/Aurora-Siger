# 🚀 Projeto Aurora-Siger

## 📌 Descrição
Este projeto tem como objetivo simular e analisar condições de lançamento de foguetes a partir de dados de telemetria.

Utilizando Python, foram aplicadas regras baseadas em limites operacionais para classificar automaticamente o status da missão.

---

## ⚙️ Tecnologias Utilizadas
- Python
- Pandas
- Matplotlib
- Jupyter Notebook

---

## 🧠 Lógica do Algoritmo

O sistema avalia os seguintes critérios:

- Integridade estrutural
- Pressão do tanque
- Nível de energia
- Temperatura interna
- Funcionamento dos módulos:
  - Navegação
  - Propulsão
  - Comunicação

### Possíveis resultados:
- ❌ DECOLAGEM ABORTADA  
- ⚠️ PRONTO PARA DECOLAR COM ALERTA  
- ✅ PRONTO PARA DECOLAR  

---

## 📊 Resultados

- ❌ Decolagens abortadas: **305**
- ✅ Pronto para decolar: **195**

---

## 📈 Distribuição dos Resultados


![alt text](image.png)
---

## 🚨 Principais Causas de Abortamento

- 🔋 Energia: 239 ocorrências  
- ⚙️ Módulos: 46 ocorrências  
- 🌡️ Pressão: 42 ocorrências  
- 🌡️ Temperatura: 20 ocorrências  

![alt text](image-1.png)

---

## 🔍 Análise

A principal causa de abortamento está relacionada ao **nível de energia insuficiente**, indicando que este é o fator crítico no sistema.

Falhas em módulos também apresentam impacto relevante, enquanto temperatura e pressão têm menor influência relativa.

---

## 🧾 Estrutura do Projeto

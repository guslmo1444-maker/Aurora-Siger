# 🚀 Aurora-Siger

Projeto de simulação e análise de lançamento de foguetes utilizando programação, modelagem física e análise de dados.

---

## 📌 Introdução

A exploração espacial depende fortemente da análise contínua de dados de telemetria para garantir a segurança e a confiabilidade das missões. Sistemas de lançamento de foguetes utilizam diversos sensores para monitorar variáveis críticas como temperatura, pressão, integridade estrutural e funcionamento de módulos essenciais.

A interpretação correta desses dados é fundamental para determinar se as condições operacionais estão adequadas para a realização de uma decolagem segura.

Nesse contexto, a análise de dados e o desenvolvimento de algoritmos de decisão tornam-se ferramentas essenciais para apoiar o processo de avaliação das condições de lançamento.

---

## 🎯 Objetivo

Desenvolver um algoritmo capaz de:

- Analisar dados de telemetria  
- Classificar automaticamente o estado da missão  
- Apoiar a decisão de lançamento  

### Possíveis resultados:
- ✅ Pronto para decolagem  
- ⚠️ Pronto para decolagem com alerta  
- ❌ Decolagem abortada  

---

## ⚙️ Algoritmo de Verificação

O sistema utiliza regras baseadas em limites operacionais para avaliar:

- Integridade estrutural  
- Pressão do tanque  
- Nível de energia  
- Temperatura interna  
- Temperatura externa  
- Funcionamento de módulos críticos  

### 🧠 Lógica do algoritmo

```python
if integridade_estrutural == 0:
    resultado = "DECOLAGEM ABORTADA"

elif pressao_tanque < 95 or pressao_tanque > 105:
    resultado = "DECOLAGEM ABORTADA"

elif nivel_energia < 80:
    resultado = "DECOLAGEM ABORTADA"

elif temperatura_interna < 15 or temperatura_interna > 35:
    resultado = "DECOLAGEM ABORTADA"

elif modulo_critico == "FALHA":
    resultado = "DECOLAGEM ABORTADA"

elif temperatura_externa > 45:
    resultado = "PRONTO PARA DECOLAR COM ALERTA"

else:
    resultado = "PRONTO PARA DECOLAR"
    
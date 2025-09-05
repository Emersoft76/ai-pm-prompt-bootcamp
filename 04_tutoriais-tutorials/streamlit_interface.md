# 🎛️ Tutorial: Criando Interfaces com Streamlit

---

## 🇧🇷 Introdução

O Streamlit permite criar interfaces web interativas com Python, sem precisar escrever HTML/CSS.

## 🇺🇸 Introduction

Streamlit allows you to build interactive web interfaces using Python, without writing any HTML/CSS.

---

## 📦 Instalação

```bash
pip install streamlit
```

---

## ▶️ Executar app

```
streamlit run nome_do_arquivo.py
````

---

## 🧪 Exemplo simples

```python
import streamlit as st

st.title("Assistente com IA")
nome = st.text_input("Digite seu nome:")
if nome:
    st.write(f"Olá, {nome}! Bem-vindo ao bootcamp.")
```

---

## 📌 Dica

Combine com OpenAI API ou LangChain para criar apps inteligentes com chatbots, resumos, assistentes, etc.

---

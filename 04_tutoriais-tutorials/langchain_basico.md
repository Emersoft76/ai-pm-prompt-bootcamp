# 🧩 Tutorial: Começando com LangChain

---

## 🇧🇷 Introdução

LangChain é um framework para construir aplicações com LLMs de forma modular, incluindo prompts, memória, cadeias e agentes.

## 🇺🇸 Introduction

LangChain is a framework for building modular applications with LLMs, including prompts, memory, chains, and agents.

---

## 📦 Instalação

```bash
pip install langchain openai
```

---

## 🔗 Exemplo simples com prompt

```python
from langchain.chat_models import ChatOpenAI
from langchain.prompts import ChatPromptTemplate

llm = ChatOpenAI(temperature=0.5)

prompt = ChatPromptTemplate.from_template("Traduza para o inglês: {texto}")
chain = prompt | llm

resposta = chain.invoke({"texto": "Eu gosto de IA"})
print(resposta.content)
```

---

## 📌 Recursos úteis

* Documentação: https://docs.langchain.com
* Templates, memória, e agentes podem ser encadeados

---

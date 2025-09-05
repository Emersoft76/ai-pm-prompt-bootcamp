# ✍️🧠 Lab Avançado: Prompt Engineering Expert

---

## 🇧🇷 Objetivo

Neste lab, você vai explorar técnicas avançadas de prompt engineering para LLMs — como few-shot prompting, chain-of-thought, embeddings e context injection.

## 🇺🇸 Objective

In this lab, you'll explore advanced prompt engineering techniques for LLMs — such as few-shot prompting, chain-of-thought, embeddings, and context injection.

---

## 📦 Tecnologias / Technologies

- OpenAI API
- LangChain
- Pinecone / FAISS (opcional para embeddings)
- PromptLayer (para rastreamento)

---

## 📌 Técnicas abordadas

### ✅ Few-shot prompting

```plaintext
Instrução + Exemplos + Pergunta
```

### ✅ Chain of Thought (CoT)

```plaintext
"Vamos pensar passo a passo..."
```

### ✅ Contextualização com embedding

* Armazene contextos em vetores
* Faça busca semântica por similaridade
* Injete o resultado no prompt

---

## 🧪 Exemplo de estrutura LangChain

```python
from langchain.chains import LLMChain
from langchain.prompts import PromptTemplate
from langchain.chat_models import ChatOpenAI

template = """Responda a pergunta com base no contexto abaixo:
{contexto}

Pergunta: {pergunta}"""

prompt = PromptTemplate.from_template(template)
llm = ChatOpenAI(temperature=0.3)
chain = LLMChain(prompt=prompt, llm=llm)

resposta = chain.run({
    "contexto": "O curso começa dia 15 de setembro.",
    "pergunta": "Quando começa o curso?"
})
print(resposta)
```

---

## 📈 Métricas sugeridas

* Acurácia contextual
* Taxa de erro por tipo de pergunta
* Custo por requisição

---

# ⚙️ Tutorial: Criando APIs com Flask e FastAPI

---

## Flask (básico)

### 📦 Instalação

```bash
pip install flask
```

## 📁 Exemplo

```python
from flask import Flask

app = Flask(__name__)

@app.route("/")
def home():
    return "API com Flask funcionando!"

if __name__ == "__main__":
    app.run(debug=True)
```

---

## FastAPI (avançado)

📦 Instalação

```
pip install fastapi uvicorn
```

📁 Exemplo

```python
from fastapi import FastAPI

app = FastAPI()

@app.get("/")
def root():
    return {"mensagem": "API com FastAPI funcionando!"}
```

▶️ Rodar servidor

```
uvicorn nome_do_arquivo:app --reload
```

---

🔐 Segurança

Use python-dotenv para guardar chaves de API:

```
pip install python-dotenv
```

Crie um arquivo .env:

```ini
OPENAI_API_KEY=xxxxx
```

---

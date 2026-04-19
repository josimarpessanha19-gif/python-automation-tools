# 🐍 Python Automation Tools

> Coleção de ferramentas e scripts de automação em Python para otimizar processos e integrar APIs.

[![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)
[![Author](https://img.shields.io/badge/Author-Josimar%20Pessanha-blueviolet?style=flat-square)](https://github.com/josimarpessanha19-gif)

---

## 📦 Projetos Incluídos

### 🤖 1. WhatsApp Bot
Bot automatizado para WhatsApp com respostas inteligentes e integração com IA.
```python
# Exemplo de uso
bot = WhatsAppBot(session="minha-sessao")
bot.on_message(lambda msg: bot.reply(msg, "Olá! Como posso ajudar?"))
bot.start()
```

### 🔗 2. API REST Client
Cliente HTTP robusto para integração com APIs externas.
```python
# Exemplo de uso
client = APIClient(base_url="https://api.exemplo.com", api_key="sua-chave")
response = client.get("/users", params={"page": 1})
print(response.json())
```

### 📊 3. Data Processor
Ferramenta para processamento e análise de grandes volumes de dados.
```python
# Exemplo de uso
processor = DataProcessor("dados.csv")
resultado = processor.aggregate(group_by="categoria", sum_cols=["valor"])
processor.export(resultado, "relatorio.xlsx")
```

### ☁️ 4. AWS Automation
Scripts para automação de tarefas na AWS (S3, EC2, Lambda).
```python
# Exemplo de uso
aws = AWSManager(region="us-east-1")
aws.s3.upload_file("arquivo.pdf", bucket="meu-bucket", key="uploads/arquivo.pdf")
print("Upload concluído!")
```

---

## 🛠️ Tecnologias

| Tecnologia | Uso |
|-----------|-----|
| Python 3.11+ | Linguagem principal |
| Requests / HTTPX | Chamadas HTTP |
| Selenium / Playwright | Automação Web |
| boto3 | AWS SDK |
| pandas | Processamento de dados |
| python-dotenv | Variáveis de ambiente |

---

## 🚀 Como Usar

```bash
# Clone o repositório
git clone https://github.com/josimarpessanha19-gif/python-automation-tools.git

# Entre na pasta
cd python-automation-tools

# Instale as dependências
pip install -r requirements.txt

# Configure as variáveis de ambiente
cp .env.example .env
# Edite o .env com suas credenciais

# Execute
python main.py
```

---

## 📁 Estrutura do Projeto

```
python-automation-tools/
├── 📂 bots/
│   ├── whatsapp_bot.py
│   └── telegram_bot.py
├── 📂 api/
│   ├── client.py
│   └── webhooks.py
├── 📂 aws/
│   ├── s3_manager.py
│   └── ec2_manager.py
├── 📂 data/
│   └── processor.py
├── requirements.txt
├── .env.example
└── README.md
```

---

## 👨‍💻 Autor

**Josimar Pessanha de Aguiar**
- 📧 josimarpessanha19@gmail.com
- 💼 [LinkedIn](https://www.linkedin.com/in/josimar-pessanha-de-aguiar-7a99a9356/)
- 🐙 [GitHub](https://github.com/josimarpessanha19-gif)

---

⭐ Se este projeto te ajudou, deixe uma estrela!

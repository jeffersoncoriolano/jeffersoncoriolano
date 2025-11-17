# 👋 Olá, eu sou Jefferson Coriolano

### Engenheiro de Automação por formação, **Engenheiro de Dados** por profissão com ênfase em:

- **Python**
- **SQL (PostgreSQL, Supabase, MySQL, SQLite)**
- **ETL / ELT**
- **Databricks**
- **PySpark**
- **Manipulação e transformação de dados**
- **Automatização de pipelines**
- **Git**

### 🛠️ Outras skills que fazem parte do meu kit:

- **N8N** – Criação de fluxos de automação low-code
- **Integrações com APIs**
- **Uso prático de IA generativa (Google Gemini, OpenAI) para automações de processos**

### 🚀 Estilo de aprendizado:

Prefiro aprender **resolvendo problemas reais**, criando soluções práticas (muitas vezes nascidas de necessidades pessoais).

---

### 📌 Projetos em destaque:

#### 1. Pipeline Serverless de Processamento de Dados de Velocidade (AWS)

**Arquitetura Geral**
- S3 (raw XLSX)
 → Lambda (trigger)
 → AWS Glue (ETL: XLSX → CSV)
 → S3 (processed)
 → Lambda (ingestão)
 → RDS MySQL
 → S3 (processed_ingested)

**Principais Recursos**
- Particionamento por year=YYYY/month=MM seguindo modelo de Data Lake
- Glue executando conversão e limpeza de arquivos com mais de 500k linhas
- Lambda com:
  - batch insert configurável (ex.: 5k)
  - retry com exponential backoff
  - reconexão automática ao banco
  - prevenção de reprocessamento (arquivamento após ingestão)
  - suporte a deduplicação (INSERT IGNORE)
- Pipeline totalmente escalável e de baixo custo (pay-per-use)

**Tecnologias**
- AWS: S3, Lambda, Glue, RDS MySQL, CloudWatch, IAM
- Python: pandas, boto3, PyMySQL
- Padrões: Data Lake, ETL/ELT, arquitetura serverless

**Resultado**
Pipeline robusto que:
- Automatiza todo o fluxo de processamento dos arquivos de velocidade
- Insere milhões de registros no banco com resiliência
- Mantém trilha auditável via processed_ingested
- Cria base sólida para BI, análises de tráfego e projetos de Mobilidade Urbana Inteligente

---
 
#### 2. **Automação de controle de gastos via Telegram + IA + PostgreSQL + N8N:**  
[👉 Ver no GitHub](https://github.com/jeffersoncoriolano/controle-de-gastos-automatizado-n8n-postgresql-ai)

---

### 📈 Próximos passos:

- Aprimorar minhas skills em **Databricks**, **Spark** e processamento distribuído
- Me aprofundar em **pipelines de dados em escala**
- Explorar ferramentas de orquestração como **Airflow**

---

### 📬 Vamos conversar?

Se quiser trocar uma ideia ou tiver alguma vaga/projeto relacionado a dados ou automação:

👉 [Meu LinkedIn](https://www.linkedin.com/in/jeffersoncoriolano/)  
👉 Ou pode abrir uma issue por aqui no GitHub

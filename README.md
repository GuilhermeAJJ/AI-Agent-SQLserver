# 🤖 AI-Agent-SQLServer

Agente de IA conectado ao SQL Server para consultas de agendamentos.

---

## 📌 Sobre o Projeto

Bem-vindo ao meu primeiro projeto de **AI Agent** 🚀

Este projeto consiste na criação de um **Agente de Inteligência Artificial** focado na consulta de agendamentos de uma empresa do setor de **Agenciamento Marítimo**.

O agente é capaz de interpretar solicitações em linguagem natural e realizar consultas diretamente em um banco **SQL Server**, retornando informações de forma automatizada.

A arquitetura foi construída utilizando:

- **n8n** → Orquestração de workflows e agente de IA  
- **SQL Server** → Base de dados de agendamentos  
- **Evolution API** → Integração com WhatsApp  
- **Docker** → Containerização do ambiente  

---

## 🐳 Instalação via Docker

A forma mais fácil de executar o projeto é via **Docker Compose**.

### 1️⃣ Pré-requisitos

Antes de iniciar, instale:

- [Docker](https://www.docker.com/)
- Docker Compose (já incluso no Docker Desktop)

---

### 2️⃣ Baixar arquivos do projeto

Baixe os arquivos:

- `docker-compose.yaml`
- `.env`

Coloque ambos na mesma pasta.

---

### 3️⃣ Subir os containers

Abra o **PowerShell** (ou terminal) dentro da pasta onde estão os arquivos e execute:

```bash
docker compose up -d



🌐 Acessos do Ambiente

Após subir os serviços, acesse:

Serviço	URL	Descrição
n8n	http://localhost:5678
	Criação e configuração dos workflows
Evolution API	http://localhost:8080
	API para WhatsApp e integrações
⚙️ Configuração do n8n

Ao acessar o n8n pela primeira vez:

Preencha as informações iniciais.

Utilize um e-mail válido.

Você receberá uma KEY de ativação.

Insira a KEY para liberar os Community Nodes.

Ambiente pronto para uso ✅

📲 Configuração da Evolution API (WhatsApp)

Para conectar:

Acesse: http://localhost:8080

Informe a API_KEY do arquivo .env.

Gere o QR Code.

Escaneie no WhatsApp.

Conexão concluída ✅

🔗 Integração Evolution API → n8n

Passos:

Crie um node Webhook no n8n.

Defina um path.

Exemplo:

/webhook/whatsapp-agent


Configure na Evolution API:

http://n8n:5678/webhook/whatsapp-agent


Ative o workflow.

🧠 Funcionalidades do Agente

Consulta de agendamentos via linguagem natural

Integração com SQL Server

Respostas automatizadas via WhatsApp

Memória de contexto (quando configurado)

Automação de fluxos operacionais

🛠️ Tecnologias Utilizadas

n8n

SQL Server

Evolution API

Docker

IA / LLMs

Webhooks

APIs REST

<div align="center">

# Olá, eu sou o Rafael 👋

**Sr. Product Manager | Co-Founder @ GAIA | AI & Data**

📍 Belo Horizonte, Brasil · [LinkedIn](https://www.linkedin.com/in/rafael-leite-macedo/) 
 [Portfólio](https://www.grupogaiatech.com.br)

</div>

---

### 🧭 O que eu faço

Sou Product Manager sênior e uso IA e automação como ferramenta de trabalho, não só como discurso. Em vez de esperar backlog de engenharia pra validar uma hipótese, eu mesmo construo o protótipo: automações, agentes, análises de dados — o suficiente pra testar uma ideia com dados reais antes de escalar.

Como Co-Founder da GAIA (SaaS B2B/B2G de Gestão de Arborização Urbana), aplico isso no dia a dia: uso IA para acelerar discovery, automatizar processos operacionais e construir ferramentas internas que tirariam semanas de um time de eng. para entregar.

### 🛠️ Como eu construo

| Área | Ferramentas |
|---|---|
| **Automação & Workflows** | n8n, Webhooks, APIs REST, WhatsApp Cloud API, Telegram Bot API |
| **Dados para decisão de produto** | SQL, análise de dados de produto |
| **IA aplicada** | Python, TypeScript, MCP (Model Context Protocol), RAG, LLMs com fallback entre provedores (Groq, Workers AI, Gemini), guardrails e testes de prompt injection |
| **Infra serverless** | Cloudflare Workers, D1, Vectorize, Wrangler |
| **Qualidade** | TDD com Vitest, regressão de segurança para agentes, design orientado à LGPD |
| **Product Management** | Discovery, priorização, roadmap, escrita de specs |

---
### 🤖 Projeto em destaque — Agente de atendimento no WhatsApp

Agente de IA que atende leads e dúvidas do Grupo GAIA direto no WhatsApp, em produção. Ele entende a intenção da pessoa, responde com base em uma base de conhecimento própria, qualifica o contato e avisa o time comercial quando há uma oportunidade real. Quando a pergunta foge do que pode responder com segurança, encaminha para uma pessoa em vez de arriscar uma resposta.

O que ele faz:
- **RAG sobre base própria:** busca vetorial para responder só com o que a empresa afirma, sem inventar preço, prazo ou promessa.
- **Regras fixas antes do modelo:** temas sensíveis (pagamento, LGPD, urgência, cadastro de profissionais) têm resposta determinística, sem depender do LLM.
- **Cadeia de LLMs com fallback:** Groq como principal, com Workers AI e Gemini de reserva, para manter o atendimento no ar mesmo com limite de uso.
- **Guardrails de saída:** a resposta do modelo é validada antes de ir ao cliente; se violar uma regra, vira encaminhamento humano.
- **Segurança e privacidade:** suíte de regressão contra prompt injection e mascaramento de dados pessoais (CPF, CNPJ, registro de conselho) antes de armazenar ou enviar ao modelo, além de aceite e opção de sair (SAIR).
- **Operação:** qualificação do lead, registro em planilha, agenda e aviso por Telegram.

Construído com TDD, com mais de 570 testes automatizados, em parceria com o Claude.

**Stack:** TypeScript · Cloudflare Workers, D1 e Vectorize · Workers AI, Groq e Gemini · WhatsApp Cloud API · Google Sheets e Calendar · Telegram Bot API · Vitest · Zod

🔒 Código privado (uso comercial do Grupo GAIA). Posso apresentar o caso e a arquitetura em conversa.

---
### 🚀 Projeto em destaque — GAIA Hub

Marketplace B2C para regularização ambiental urbana, do zero à produção. Conecta proprietários que precisam regularizar a supressão ou poda de uma árvore junto à prefeitura de São Paulo, profissionais habilitados (biólogos e topógrafos) que executam o serviço técnico, e a equipe da GAIA, que intermedia todo o processo.

Conduzi o produto do zero ao ar — modelagem do fluxo de conformidade (32 etapas, 5 fases, com responsável e regra de transição em cada uma), arquitetura técnica, segurança de dados e operação em produção. Todo o código, da primeira linha à infraestrutura de deploy automatizado, foi escrito em parceria com o Claude, incluindo a investigação e correção de bugs reais em produção.

**Stack:** React + TanStack Start · Supabase (Postgres, RLS, Auth) · Cloudflare Workers · GitHub Actions

🔗 [gaia-arboriza.com.br](https://www.gaia-arboriza.com.br) Repositório privado B2G/B2B (produto comercial em produção)

---
### 📫 Contato

[LinkedIn](https://www.linkedin.com/in/rafael-leite-macedo/) · rafaelcicloga@gmail.com

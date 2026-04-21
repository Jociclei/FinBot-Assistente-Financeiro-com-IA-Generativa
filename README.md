# 💸 FinBot — Assistente Financeiro com IA Generativa

> Experiência digital de relacionamento financeiro guiada por inteligência artificial, com linguagem natural, simulações e contexto personalizado.

---

## 📌 Sobre o Projeto

O **FinBot** é uma solução de atendimento financeiro inteligente desenvolvida como desafio de conclusão de trilha, integrando **IA Generativa**, **Python**, **análise de dados** e **boas práticas de UX**. O objetivo é oferecer ao usuário uma experiência clara, segura e personalizada ao interagir com informações e serviços financeiros.

A proposta vai além de um simples chatbot: o sistema compreende linguagem natural, mantém contexto entre interações, realiza simulações financeiras e explica produtos de forma acessível — simulando o comportamento de um assistente bancário digital de alta qualidade.

---

## ✨ Funcionalidades

- 🤖 **FAQ Inteligente** — Responde perguntas frequentes sobre produtos e serviços financeiros com linguagem natural
- 🧮 **Simulações Financeiras** — Cálculos demonstrativos de juros, parcelas, rendimentos e projeções
- 📦 **Explicação de Produtos** — Descrições contextualizadas de produtos como CDB, Tesouro Direto, cartões e crédito pessoal
- 🧠 **Persistência de Contexto** — Mantém o histórico da conversa para respostas mais relevantes e personalizadas
- 🔐 **Interações Seguras** — Sem coleta de dados sensíveis; foco em orientação e educação financeira
- 🎯 **UX Centrado no Usuário** — Fluxo de conversa guiado por princípios de clareza, feedback imediato e acessibilidade

---

## 🛠️ Tecnologias Utilizadas

| Camada | Tecnologia |
|---|---|
| Linguagem | Python 3.11+ |
| IA Generativa | API OpenAI / Google Gemini / Anthropic Claude |
| Interface | Streamlit / Gradio |
| Gerenciamento de Contexto | LangChain / histórico customizado |
| Dados & Simulações | Pandas, NumPy |
| Controle de Versão | Git & GitHub |

---

## 🗂️ Estrutura do Projeto

```
finbot/
├── app.py                  # Ponto de entrada da aplicação
├── config.py               # Configurações e variáveis de ambiente
├── requirements.txt        # Dependências do projeto
│
├── core/
│   ├── llm_client.py       # Integração com modelo de linguagem
│   ├── context_manager.py  # Persistência e histórico de contexto
│   └── prompt_templates.py # Templates de prompts por intenção
│
├── features/
│   ├── faq.py              # Módulo de perguntas frequentes
│   ├── simulacoes.py       # Cálculos e simulações financeiras
│   └── produtos.py         # Explicações de produtos financeiros
│
├── ux/
│   ├── components.py       # Componentes reutilizáveis de interface
│   └── messages.py         # Mensagens padrão e fallbacks
│
└── tests/
    ├── test_simulacoes.py
    └── test_faq.py
```

---

## 🚀 Como Executar

### Pré-requisitos

- Python 3.11+
- Chave de API do modelo de linguagem (OpenAI, Gemini ou Claude)

### Instalação

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/finbot.git
cd finbot

# Crie e ative o ambiente virtual
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows

# Instale as dependências
pip install -r requirements.txt
```

### Configuração

Crie um arquivo `.env` na raiz do projeto:

```env
LLM_API_KEY=sua_chave_aqui
LLM_MODEL=gpt-4o          # ou gemini-pro, claude-3-sonnet, etc.
APP_ENV=development
```

### Execução

```bash
streamlit run app.py
```

Acesse em `http://localhost:8501`

---

## 💬 Exemplos de Interação

```
👤 Usuário: Qual a diferença entre CDB e Tesouro Direto?
🤖 FinBot: Ótima pergunta! O CDB é emitido por bancos privados...

👤 Usuário: Se eu investir R$ 5.000 no CDB por 12 meses com 12% ao ano, quanto terei?
🤖 FinBot: Vamos simular! Com R$ 5.000 a 12% a.a. por 12 meses...
           💰 Montante bruto: R$ 5.600,00
           📊 IR descontado (17,5%): R$ 105,00
           ✅ Valor líquido estimado: R$ 5.495,00

👤 Usuário: E se for por 24 meses?
🤖 FinBot: Considerando o mesmo investimento por 24 meses... [contexto mantido]
```

---

## 📐 Princípios de UX Aplicados

- **Clareza** — Respostas objetivas, sem jargões desnecessários
- **Feedback imediato** — Confirmação visual de cada entrada do usuário
- **Prevenção de erros** — Validações e mensagens de orientação
- **Consistência** — Padrão de linguagem e tom ao longo de toda a conversa
- **Acessibilidade** — Interface responsiva e linguagem inclusiva

---

## 🧪 Testes

```bash
pytest tests/ -v
```

---

## 📈 Aprendizados da Trilha Aplicados

- ✅ Engenharia de Prompts (system prompts, few-shot examples, chain-of-thought)
- ✅ Integração com APIs de LLMs
- ✅ Gestão de contexto e memória conversacional
- ✅ Python para automação e cálculos
- ✅ Princípios de UX aplicados à IA conversacional
- ✅ Boas práticas de segurança e privacidade

---

## ⚠️ Aviso Legal

> Este assistente tem finalidade **educacional e demonstrativa**. As simulações e informações fornecidas não constituem aconselhamento financeiro. Consulte sempre um profissional habilitado para decisões de investimento.

---

## 🤝 Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests.

---

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

<div align="center">
  Desenvolvido com 💙 durante a trilha de IA & Tecnologia
</div>

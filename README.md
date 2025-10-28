# 📌 Sistema de Suporte com Serviços de IA

---

<details open>
  <summary>🎯 <strong>Descrição do Desafio</strong></summary>

O projeto visa desenvolver um sistema integrado de suporte técnico para uma empresa de médio porte.  
O objetivo é substituir o atual processo de recebimento de chamados por e-mail, permitindo o registro centralizado das solicitações.  
A inteligência artificial (IA) será usada para sugerir soluções de forma automática ou encaminhar os chamados ao técnico adequado, com base nas instruções fornecidas pelo time de desenvolvimento.

</details>

---

<details>
  <summary>📋 <strong>Backlog do Produto</strong></summary>

| ID   | Item do Backlog | Prioridade | Sprint | Status   |
|------|------------------|-------------|---------|-----------|
| RF1  | Implementar sistema de Login | Alta | Sprint 1 | Pendente |
| RF2  | Criar telas distintas para Administrador e Usuário Comum | Alta | Sprint 1 | Pendente |
| RF3  | Funcionalidade para abrir chamado | Alta | Sprint 1 | Pendente |
| RF4  | Permitir edição de chamado | Média | Sprint 2 | Pendente |
| RF5  | Adicionar campo de descrição do chamado | Alta | Sprint 1 | Pendente |
| RF6  | Definir nível de prioridade do chamado | Alta | Sprint 2 | Pendente |
| RF7  | Definir tipo de chamado | Média | Sprint 2 | Pendente |
| RF8  | Indicar setor para o qual o chamado deve ser aberto | Média | Sprint 2 | Pendente |
| RF9  | Notificação para o Técnico receber o chamado | Alta | Sprint 3 | Pendente |
| RF10 | Implementar IA para analisar texto e sugerir solução ao técnico | Alta | Sprint 3 | Pendente |
| RF11 | Técnico finalizar atendimento registrando o procedimento realizado | Alta | Sprint 3 | Pendente |
| RF12 | Sistema armazenar histórico do que foi feito, quando e por quem | Alta | Sprint 4 | Pendente |

</details>

---

<details>
  <summary>📆 <strong>Cronograma de Evolução do Projeto (Visual)</strong></summary>

| Sprint | Período | Documentação |
|--------|----------|--------------|
| Sprint 1 | 15/09 – 01/10 | [📄 Docs Sprint 1](#) |
| Sprint 2 | 02/10 – 18/10 | [📄 Docs Sprint 2](#) |
| Sprint 3 | 19/10 – 25/10 | [📄 Docs Sprint 3](#) |
| Sprint 4 | 26/10 – 02/11 | [📄 Docs Sprint 4](#) |

</details>

---

<details>
  <summary>🧾 <strong>Tabela Descritiva das Sprints</strong></summary>

| Período | Documentação da Sprint | 
|----------|------------------------|
| Sprint 1 | [📄 Link Documentação](#) | 
| Sprint 2 | [📄 Link Documentação](#) | 
| Sprint 3 | [📄 Link Documentação](#) | 
| Sprint 4 | [📄 Link Documentação](#) | 

</details>

---

<details>
  <summary>🛠️ <strong>Tecnologias Utilizadas</strong></summary>

- **Linguagens:** Python, HTML, CSS e JavaScript  
- **Frameworks:** Kivy, ReactJS e React Native  
- **Banco de Dados:** SQL Server  
- **Ferramentas:** GitHub, Trello e Figma  

</details>

---

<details>
  <summary>🏗️ <strong>Estrutura do Projeto</strong></summary>

 📁 SISTEMA_SUPORTE_IA/
│
├── 📁 backend/                # Projeto Python (Servidor, API e lógica de IA)
│   ├── 📁 app/                 # Onde o código principal da aplicação vive
│   │   ├── 📁 routes/           # Define os endpoints da API (ex: /login, /chamados)
│   │   ├── 📁 services/         # Contém a lógica de negócio e regras da IA
│   │   ├── 📁 models/           # Define as tabelas do banco de dados (ex: Usuário, Chamado)
│   │   ├── 📁 schemas/          # Validação de dados de entrada/saída (Pydantic, etc.)
│   │   └── __init__.py
│   ├── 📁 migrations/         # Arquivos de migração do banco de dados (Alembic)
│   ├── 📁 tests/              # Testes unitários e de integração
│   ├── .env                  # Variáveis de ambiente (chave da API, string do BD)
│   ├── main.py               # Ponto de entrada para iniciar o servidor
│   └── requirements.txt      # Lista de dependências Python (pip)
│
├── 📁 frontend-web/           # Projeto Web (ReactJS para Técnicos/Admin)
│   ├── public/
│   │   └── index.html
│   ├── src/
│   │   ├── 📁 assets/         # Imagens, fontes e ícones
│   │   ├── 📁 components/     # Componentes reutilizáveis (Botão, Input, Card)
│   │   ├── 📁 hooks/          # Hooks customizados (ex: useAuth)
│   │   ├── 📁 pages/          # Telas principais (Login, DashboardAdmin, DetalheChamado)
│   │   ├── 📁 services/       # Lógica de chamada da API (ex: api.js com Axios)
│   │   ├── 📁 context/        # Contexto global (ex: AuthContext)
│   │   ├── App.js            # Componente raiz
│   │   ├── index.js          # Ponto de entrada do React
│   │   └── routes.js         # Definição das rotas da aplicação web
│   └── package.json          # Dependências do frontend web (npm)
│
├── 📁 frontend-mobile/        # Projeto Mobile (React Native + Expo para Usuários)
│   ├── assets/               # Fontes, ícones e imagens
│   ├── src/
│   │   ├── 📁 components/     # Componentes reutilizáveis (CardChamado, BotaoCustomizado)
│   │   ├── 📁 hooks/          # Hooks customizados
│   │   ├── 📁 navigation/     # Gerenciamento de navegação (Stack e Tab Navigators)
│   │   ├── 📁 screens/        # Telas do app (Login, MeusChamados, AbrirChamado)
│   │   ├── 📁 services/       # Configuração da API para o mobile
│   │   └── 📁 context/        # Contexto de autenticação do usuário
│   ├── App.js                # Ponto de entrada do app (Expo)
│   ├── app.json              # Configurações do projeto Expo
│   └── package.json          # Dependências do projeto mobile (npm/yarn)
│
├── 📁 docs/                   # Toda a documentação do projeto (Manual, DoR/DoD)
│   ├── Manual_Usuario.md
│   ├── DoD_DoR.md
│   └── Sprints/
│       ├── Sprint_1.md
│       └── ...
│
└── README.md                 # O arquivo que você está lendo


</details>

---

<details>
  <summary>📖 <strong>Execução, Uso e Testes</strong></summary>

### 🔹 Frontend  
1. Acesse a pasta `/frontend-web`  
2. Execute `npm install`  
3. Inicie com `npm start`  

### 🔹 Backend  
1. Acesse a pasta `/backend`  
2. Instale dependências com `pip install -r requirements.txt`  
3. Rode o servidor com `python app.py`  

### 🔹 Mobile  
1. Acesse `/frontend-mobile`  
2. Execute `npm install`  
3. Inicie com `npx expo start`  

</details>

---

<details>
  <summary>📂 <strong>Link para Pasta de Documentação</strong></summary>

📁 [Acessar Documentação](#)

</details>

---

<details>
  <summary>👥 <strong>Equipe</strong></summary>

| Nome | Papel | GitHub |
|------|--------|--------|
| Lucas de Oliveira Silva | Desenvolvedor Frontend | [GitHub](https://github.com/Kript0-Web) |
| Samuel Jhonata de Lima | Desenvolvedor Backend | [GitHub](https://github.com/SamuJL) |
| Gabriel Oliveira dos Santos | Analista de Requisitos | [GitHub](https://github.com/gabrielods14) |
| João Gabriel Goulart Silva | UX/UI Designer | [GitHub](https://github.com/Goulart06) |
| Thiago Almeida Ribeiro | QA / Testes | [GitHub](https://github.com/Thiagoalmeida74) |
| Gabriel Silva Guimarães | DevOps | [GitHub](https://github.com/guimagabs) |

</details>

---

<details>
  <summary>📘 <strong>Outros Elementos Obrigatórios</strong></summary>

### 🗂️ Pasta de Documentação
- [Checklist de DoR e DoD](#)
- [DoR e DoD por Sprint](#)
- [Manual do Usuário](#)

</details>

# 📌 Sistema de Suporte com Serviços de IA — *HelpWave*

---

<details open>
  <summary>🎯 <strong>Descrição do Desafio</strong></summary>

O **HelpWave** é um sistema integrado de suporte técnico voltado para empresas de médio porte.  
Seu principal objetivo é substituir o processo tradicional de recebimento de chamados por e-mail, centralizando as solicitações em uma plataforma unificada.  

O sistema utiliza **Inteligência Artificial (IA)** para analisar automaticamente as descrições dos chamados, sugerindo soluções ao técnico responsável.  
A solução é multiplataforma — abrangendo **Web**, **Mobile** e **Desktop** — e conta com três perfis principais de usuário:  
**Administrador**, **Suporte Técnico** e **Colaborador**.

</details>

---

<details>
  <summary>📋 <strong>Backlog do Produto</strong></summary>

| ID   | Item do Backlog | Prioridade | Sprint | Status   |
|------|------------------|-------------|---------|-----------|
| RF01 | Implementar autenticação e controle de acesso com níveis de permissão (Administrador, Suporte, Colaborador) | Alta | Sprint 1 | Pendente |
| RF02 | Permitir cadastro de novos usuários (Administrador) | Alta | Sprint 1 | Pendente |
| RF03 | Permitir edição de informações de usuários (Administrador) | Média | Sprint 1 | Pendente |
| RF04 | Permitir exclusão de usuários cadastrados, com validação de vínculos a chamados ativos | Média | Sprint 1 | Pendente |
| RF05 | Permitir abertura de chamados com título, descrição e categoria (Colaborador) | Alta | Sprint 2 | Pendente |
| RF06 | Permitir acompanhamento de chamados abertos e seus status (Colaborador) | Alta | Sprint 2 | Pendente |
| RF07 | Visualizar todos os chamados do sistema com filtros avançados (Administrador) | Alta | Sprint 2 | Pendente |
| RF08 | Exibir chamados atribuídos a cada técnico (Suporte Técnico) | Média | Sprint 2 | Pendente |
| RF09 | Integrar IA para sugerir soluções automáticas com base na descrição do chamado | Alta | Sprint 3 | Pendente |
| RF10 | Permitir que o técnico analise, aceite, modifique ou rejeite a sugestão da IA | Alta | Sprint 3 | Pendente |
| RF11 | Registrar a solução aplicada no chamado (Suporte Técnico) | Alta | Sprint 3 | Pendente |
| RF12 | Concluir chamado resolvido e notificar colaborador (Suporte Técnico) | Alta | Sprint 3 | Pendente |
| RF13 | Gerar relatórios administrativos e de desempenho (Administrador) | Média | Sprint 4 | Pendente |
| RF14 | Visualizar relatórios técnicos de produtividade (Suporte Técnico) | Média | Sprint 4 | Pendente |

</details>

---

<details>
  <summary>📆 <strong>Cronograma de Evolução do Projeto (Visual)</strong></summary>

| Sprint | Período | Entregas Principais |
|--------|----------|---------------------|
| Sprint 1 | 15/09 – 01/10 | Autenticação, login e gerenciamento de usuários (CRUD completo) |
| Sprint 2 | 02/10 – 18/10 | Módulo de chamados (abertura, acompanhamento e visualização por perfil) |
| Sprint 3 | 19/10 – 03/11 | Integração com IA e fluxo de resolução de chamados (sugestão, análise e conclusão) |
| Sprint 4 | 04/11 – 20/11 | Relatórios administrativos e técnicos com filtros e exportação |

</details>

---

<details>
  <summary>🧾 <strong>Tabela Descritiva das Sprints</strong></summary>

| Período | Funcionalidades Desenvolvidas | Documentação da Sprint | Vídeo no YouTube |
|----------|-------------------------------|------------------------|------------------|
| Sprint 1 | Login, autenticação e CRUD de usuários | [📄 Documentação Sprint 1](https://github.com/SamuJL/Projeto-Unip/blob/main/docs/sprints/sprint1.md) | [🎥 Incremento 1](#) |
| Sprint 2 | Abertura, acompanhamento e visualização de chamados (Admin, Colaborador e Suporte) | [📄 Documentação Sprint 2](https://github.com/SamuJL/Projeto-Unip/blob/main/docs/sprints/sprint2.md) | [🎥 Incremento 2](#) |
| Sprint 3 | Integração da IA e gerenciamento completo do ciclo de chamados | [📄 Documentação Sprint 3](https://github.com/SamuJL/Projeto-Unip/blob/main/docs/sprints/sprint3.md) | [🎥 Incremento 3](#) |
| Sprint 4 | Relatórios administrativos e técnicos de produtividade | [📄 Documentação Sprint 4](https://github.com/SamuJL/Projeto-Unip/blob/main/docs/sprints/sprint4.md) | [🎥 Incremento 4](#) |

</details>

---

<details>
  <summary>🛠️ <strong>Tecnologias Utilizadas</strong></summary>

### 🧩 **Arquitetura Geral**
- Sistema distribuído com **Backend centralizado (API REST)**, integrando os módulos Web, Mobile e Desktop.  
- Comunicação via **HTTP/JSON** com autenticação baseada em tokens.  
- Hospedagem e serviços em nuvem através da **Azure Cloud**.

### ⚙️ **Backend Centralizado (API de Banco de Dados)**
- **Linguagem:** C# (.NET 8)  
- **ORM:** Entity Framework Core  
- **Banco de Dados:** SQL Server (Azure)

### 🌐 **Frontend Web**
- **Linguagens:** HTML, CSS, JavaScript  
- **Framework:** React  

### 🔧 **Backend Web**
- **Linguagem:** Python  
- **Framework:** Flask  

### 📱 **Mobile**
- **Linguagem:** JavaScript  
- **Framework:** React Native  

### 💻 **Desktop**
- **Linguagem:** Python  
- **Framework:** Kivy  

### ☁️ **Infraestrutura e Gestão**
- **Controle de Versão e Gestão de Projeto:** GitHub Projects  
- **Nuvem e Deploy:** Azure Cloud  

</details>

---

<details>
  <summary>🏗️ <strong>Estrutura do Projeto</strong></summary>

O projeto está dividido em módulos independentes integrados via API:

/backend-api → API central (C# .NET 8 + SQL Server Azure)
/backend-web → Backend Web (Python + Flask)
/frontend-web → Interface Web (React)
/frontend-mobile → Aplicativo Mobile (React Native)
/frontend-desktop → Aplicação Desktop (Python + Kivy)
/docs → Documentações e relatórios de Sprints


</details>

---

<details>
  <summary>📖 <strong>Execução, Uso e Testes</strong></summary>

### 🔹 Frontend Web  
1. Acesse a pasta `/frontend-web`  
2. Execute `npm install`  
3. Inicie com `npm start`  

### 🔹 Backend Web  
1. Acesse a pasta `/backend-web`  
2. Instale dependências com `pip install -r requirements.txt`  
3. Inicie o servidor com `python app.py`  

### 🔹 Backend Centralizado  
1. Acesse a pasta `/backend-api`  
2. Configure o **connection string** do SQL Server (Azure)  
3. Execute a API com `dotnet run`  

### 🔹 Mobile  
1. Acesse `/frontend-mobile`  
2. Execute `npm install`  
3. Inicie com `npx expo start`  

### 🔹 Desktop  
1. Acesse `/frontend-desktop`  
2. Execute `python main.py`  

</details>

---

<details>
  <summary>📂 <strong>Link para Pasta de Documentação</strong></summary>

📁 [Acessar Documentação](https://github.com/SamuJL/Projeto-Unip/blob/main/docs/Diagrama%20UML%20Sistema.asta)

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

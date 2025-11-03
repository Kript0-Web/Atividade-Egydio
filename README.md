# 📌 Sistema de Suporte com Serviços de IA — *HelpWave*

<details OPEN>
<summary><strong>🎯 Descrição do Desafio</strong></summary>

O **HelpWave** é um sistema integrado de suporte técnico voltado para empresas de médio porte. Seu principal objetivo é substituir o processo tradicional de recebimento de chamados por e-mail, centralizando as solicitações em uma plataforma unificada.

O sistema utiliza **Inteligência Artificial (IA)** para analisar automaticamente as descrições dos chamados, sugerindo soluções ao técnico responsável.
A solução é multiplataforma — abrangendo **Web**, **Mobile** e **Desktop** — e conta com três perfis principais de usuário:
**Administrador**, **Suporte Técnico** e **Colaborador**.
</details>

---

<details>
<summary><strong>📋 Backlog do Produto (Requisitos Funcionais)</strong></summary>

| ID | Item do Backlog | Prioridade | Sprint | Status |
|----|------------------|-------------|---------|---------|
| RF01 | Login no sistema com autenticação e controle de acesso por perfil (Administrador, Suporte, Colaborador) | Alta | Sprint 1 | Feito |
| RF02 | Cadastro de novos usuários (Administrador) | Alta | Sprint 1 | Feito |
| RF03 | Edição de informações de usuários (Administrador) | Média | Sprint 1 | Feito |
| RF04 | Exclusão de usuários, com bloqueio caso haja chamados ativos vinculados | Média | Sprint 1 | Feito |
| RF05 | Abertura de chamados por colaboradores (com título, descrição e categoria) | Alta | Sprint 2 | Feito |
| RF06 | Acompanhamento de chamados criados pelo colaborador | Alta | Sprint 2 | Feito |
| RF07 | Visualização geral de chamados (Administrador), com filtros por status, data e técnico responsável | Alta | Sprint 2 | Feito |
| RF08 | Visualização de chamados atribuídos ao técnico (Suporte Técnico) | Média | Sprint 2 | Feito |
| RF09 | Geração de relatórios administrativos de desempenho e chamados (Administrador) | Média | Sprint 3 | Feito |
| RF10 | Geração de relatórios técnicos individuais de produtividade (Suporte Técnico) | Média | Sprint 3 | Feito |
| RF11 | Recebimento automático de sugestão da IA para o chamado (Suporte Técnico) | Alta | Sprint 3 | Feito |
| RF12 | Análise da sugestão da IA pelo técnico (aceitar, modificar ou ignorar) | Alta | Sprint 3 | Feito |
| RF13 | Registro de solução pelo técnico e envio automático de notificação ao colaborador | Alta | Sprint 3 | Feito |
| RF14 | Avaliação da solução pelo colaborador (aceitar ou rejeitar), com atualização de status do chamado | Alta | Sprint 4 | Feito |

</details>

---

<details>
<summary><strong>📆 Cronograma de Evolução do Projeto</strong></summary>

| Sprint | Período | Entregas Principais |
|--------|----------|---------------------|
| Sprint 1 | 15/09 – 01/10 | Login, autenticação e CRUD de usuários |
| Sprint 2 | 02/10 – 18/10 | Abertura, acompanhamento e visualização de chamados |
| Sprint 3 | 19/10 – 03/11 | Integração com IA, registro e análise de soluções |
| Sprint 4 | 04/11 – 20/11 | Relatórios administrativos e avaliação de soluções |

</details>

---

<details>
<summary><strong>🧾 Tabela Descritiva das Sprints</strong></summary>

| Período | Funcionalidades Desenvolvidas | Documentação da Sprint |
|----------|-------------------------------|------------------------|
| Sprint 1 | Login e CRUD de usuários | [📄 Sprint 1](https://github.com/Kript0-Web/Atividade-Egydio/blob/main/Docs/Sprint/Sprint%201.md) |
| Sprint 2 | Chamados (abertura, acompanhamento e visualização) | [📄 Sprint 2](https://github.com/Kript0-Web/Atividade-Egydio/blob/main/Docs/Sprint/Sprint%202.md) |
| Sprint 3 | Integração IA, registro e sugestão de soluções | [📄 Sprint 3](https://github.com/Kript0-Web/Atividade-Egydio/blob/main/Docs/Sprint/sprint%203.md) |
| Sprint 4 | Relatórios e avaliação de soluções | [📄 Sprint 4](https://github.com/Kript0-Web/Atividade-Egydio/blob/main/Docs/Sprint/sprint%204.md) |

</details>

---

<details>
<summary><strong>🛠️ Tecnologias Utilizadas</strong></summary>

### 🧩 Arquitetura Geral
* Sistema distribuído com **API REST centralizada**
* Comunicação via **HTTP/JSON** e autenticação baseada em tokens
* Hospedagem e serviços em nuvem através da **Azure Cloud**

### ⚙️ Backend Centralizado (API de Banco de Dados)
* **Linguagem:** C# (.NET 8)
* **ORM:** Entity Framework Core
* **Banco de Dados:** SQL Server (Azure)

### 🌐 Frontend Web
* **Linguagens:** HTML, CSS, JavaScript
* **Framework:** React

### 🔧 Backend Web
* **Linguagem:** Python
* **Framework:** Flask

### 📱 Mobile
* **Linguagem:** JavaScript
* **Framework:** React Native

### 💻 Desktop
* **Linguagem:** Python
* **Framework:** Kivy

### ☁️ Infraestrutura e Gestão
* **Controle de Versão:** GitHub
* **Metodologia:** Scrum com Git Flow simplificado
* **Nuvem:** Azure Cloud

</details>

---

<details>
<summary><strong>🏗️ Estrutura do Projeto</strong></summary>
  
```
/api               → API central (C# .NET 8 + SQL Server Azure)
/web/backend       → Backend Web (Python + Flask)
/web/frontend      → Interface Web (React)
/mobile            → Aplicativo Mobile (React Native)
/desktop           → Aplicação Desktop (Python + Kivy)
/docs              → Documentações, sprints e manuais
```

</details>

---

<details>
<summary><strong>📖 Como Executar, Usar e Testar</strong></summary>
### 🔹 Backend Centralizado (API - C# / .NET 8)

```bash
cd api
dotnet restore
dotnet ef database update
dotnet run
```

A API ficará disponível localmente em `https://localhost:5001` (ou conforme `launchSettings.json`).

---

### 🔹 Backend Web (Python + Flask)

```bash
cd web/backend
python -m venv venv
venv\Scripts\activate  # Windows
source venv/bin/activate  # Linux/Mac
pip install -r requirements.txt
python app.py
```

Servidor iniciado em `http://127.0.0.1:5000/`.

---

### 🔹 Frontend Web (React)

```bash
cd web/frontend
npm install
npm start
```

Aplicação acessível em `http://localhost:3000/`.

---

### 🔹 Mobile (React Native)

```bash
cd mobile
npm install
npx expo start
```

Escaneie o QR Code com **Expo Go**.

---

### 🔹 Desktop (Python + Kivy)

```bash
cd desktop
pip install -r requirements.txt
python main.py
```

---


### ☁️ Infraestrutura e Gestão
* **Controle de Versão:** GitHub
* **Metodologia:** Scrum com Git Flow simplificado
* **Nuvem:** Azure Cloud

</details>

---

<details> <summary><strong>📂 Link para Documentação</strong></summary>
📁 [Acessar Documentação Completa](https://github.com/Kript0-Web/Atividade-Egydio/blob/main/Diagrama%20ASTAH/Diagrama%20UML%20Sistema.asta)

📄 [Checklist de DoR e DoD (Geral)](https://github.com/Kript0-Web/Atividade-Egydio/blob/main/Docs/Checklist_DoR_DoD.md)

---

</details>

---

<details> <summary><strong>👥 Equipe</strong></summary>

| Nome | Papel | GitHub | LinkedIn |
|------|--------|--------|-----------|
| Lucas de Oliveira Silva | FullStack Developer | [GitHub](https://github.com/Kript0-Web) | — |
| Samuel Jhonata de Lima | FullStack Developer | [GitHub](https://github.com/SamuJL) | — |
| Gabriel Oliveira dos Santos | FullStack Developer | [GitHub](https://github.com/gabrielods14) | — |
| João Gabriel Goulart Silva | FullStack Developer | [GitHub](https://github.com/Goulart06) | — |
| Thiago Almeida Ribeiro | FullStack Developer | [GitHub](https://github.com/Thiagoalmeida74) | — |
| Gabriel Silva Guimarães | FullStack Developer | [GitHub](https://github.com/guimagabs) | — |

---
</details>

---

<details> <summary><strong>🗂️ Pasta de Documentação</strong></summary>

A documentação do projeto está organizada em `/docs`, contendo:

- [📘 **Checklist de DoR (Definition of Ready)**](https://github.com/Kript0-Web/Atividade-Egydio/blob/main/Docs/Checklist_DoR_DoD.md)
- [📙 **Checklist de DoD (Definition of Done)**](https://github.com/Kript0-Web/Atividade-Egydio/blob/main/Docs/Checklist_DoR_DoD.md)
- [🏁 **Sprint 1 — Autenticação e Gerenciamento de Usuários**](https://github.com/Kript0-Web/Atividade-Egydio/blob/main/Docs/Sprint/Sprint%201.md)  
- [⚙️ **Sprint 2 — Módulo de Chamados e Visualizações por Perfil**](https://github.com/Kript0-Web/Atividade-Egydio/blob/main/Docs/Sprint/Sprint%202.md)  
- [🤖 **Sprint 3 — Integração com IA e Ciclo de Soluções**](https://github.com/Kript0-Web/Atividade-Egydio/blob/main/Docs/Sprint/sprint%203.md) 
- [📊 **Sprint 4 — Relatórios e Avaliação de Soluções**](https://github.com/Kript0-Web/Atividade-Egydio/blob/main/Docs/Sprint/sprint%204.md)
- [**Manual do Usuário e Diagramas UML**](https://github.com/Kript0-Web/Atividade-Egydio/blob/main/Docs/Manual_de_Usuario_HelpWave.md)
- </details>

---

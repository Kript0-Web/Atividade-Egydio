# Manual de Usuário e Catálogo de Funcionalidades - HelpWave

Sistema de Suporte Técnico com Inteligência Artificial

São José dos Campos, Outubro de 2025

---

## Histórico das Revisões

| Data | Versão | Descrição |
|------|--------|-----------|
| 15/10/2025 | V-001 | Criação do Documento |

**Autores:** Equipe de Desenvolvimento HelpWave

---

## SUMÁRIO

1. INTRODUÇÃO
   - 1.1 Objetivos do Documento
   - 1.2 Público Alvo
   - 1.3 Visão Geral do Sistema

2. MANUAL DE USO
   - 2.1 Acesso ao Sistema
   - 2.2 Página Inicial
   - 2.3 Criar Novo Chamado
   - 2.4 Visualizar Chamados em Andamento
   - 2.5 Detalhes e Atualização de Chamado
   - 2.6 Chamados Concluídos
   - 2.7 Relatórios e Estatísticas
   - 2.8 Recursos de Usuários
   - 2.9 Recursos Administrativos

3. CATÁLOGO DE FUNCIONALIDADES

4. CONCLUSÃO

---

## 1. INTRODUÇÃO

Este manual apresenta o funcionamento do sistema HelpWave, orientando usuários sobre navegação e funcionalidades disponíveis de acordo com o nível de permissão.

### 1.1 Objetivos do Documento

Fornecer referência completa de uso do sistema HelpWave para colaboradores, técnicos de suporte e administradores.

### 1.2 Público Alvo

- 👤 **Colaboradores**: Criam e acompanham seus próprios chamados
- 🛡️ **Técnicos de Suporte**: Gerenciam e resolvem chamados de todos os usuários
- 👨‍💼 **Administradores**: Gerenciam usuários e sistema
- 🎯 **Gestores**: Acompanham desempenho através de relatórios

### 1.3 Visão Geral do Sistema

O HelpWave é uma aplicação web para gestão de chamados técnicos com integração de IA para auxiliar na elaboração de respostas.

**Funcionalidades principais:**
1. Criar chamados técnicos
2. Visualizar e acompanhar status de chamados
3. Gerenciar chamados (Suporte/Admin)
4. Usar IA para gerar sugestões de resposta
5. Acessar relatórios e estatísticas
6. Gerenciar usuários (Administrador)

---

## 2. MANUAL DE USO

### 2.1 Acesso ao Sistema

#### Pré-requisitos
- Email cadastrado pelo administrador
- Navegador atualizado (Chrome, Firefox, Edge)
- Conexão com internet estável

#### Login
1. Acesse a URL do sistema
2. Digite seu **email** no campo "USUÁRIO"
3. Digite sua **senha** no campo "SENHA"
4. Clique em **"Entrar"**

💡 **Dica:** Use o ícone de olho para visualizar a senha enquanto digita.

🔒 **Nota:** O sistema não permite auto cadastro. Apenas usuários cadastrados pela administração têm acesso.

---

### 2.2 Página Inicial (Home)

Após o login, você verá:
- **Cabeçalho**: Logo HelpWave, nome do usuário e menu de configurações
- **Menu Lateral**: Navegação entre páginas
- **Cards de Acesso**: Funcionalidades disponíveis conforme sua permissão

#### Cards por Permissão

**Colaborador (Nível 1):**
- ✅ NOVO CHAMADO

**Suporte Técnico (Nível 2):**
- ✅ NOVO CHAMADO
- ✅ CHAMADOS EM ANDAMENTO
- ✅ CHAMADOS CONCLUÍDOS
- ✅ RELATÓRIOS

**Administrador (Nível 3):**
- ✅ Todos os cards acima
- ✅ CADASTRO DE FUNCIONÁRIO

---

### 2.3 Criar Novo Chamado

1. Clique no card **"NOVO CHAMADO"**
2. Preencha os campos:
   - **Tipo de Chamado**: Selecione (Suporte, Manutenção, Instalação, Consultoria, Emergência)
   - **Título**: Mínimo 5 caracteres, máximo 100
   - **Descrição**: Mínimo 10 caracteres, máximo 1000
3. Clique em **"CRIAR CHAMADO"**

**Tipos de Chamado:**
- **Suporte**: Dúvidas e assistência técnica
- **Manutenção**: Reparos e ajustes
- **Instalação**: Instalação de equipamentos/softwares
- **Consultoria**: Orientação técnica
- **Emergência**: Problemas críticos urgentes

💡 **Dica:** Seja específico na descrição. Informe o que está acontecendo, quando começou e o que já foi tentado.

---

### 2.4 Visualizar Chamados em Andamento

**Disponível para:** Suporte Técnico e Administradores

1. Clique no card **"CHAMADOS EM ANDAMENTO"**
2. Visualize a tabela com todos os chamados pendentes
3. Use a **barra de busca** para encontrar por título ou código
4. Use os **filtros** para ordenar por:
   - Código
   - Título
   - Prioridade
   - Data Limite
5. Clique em um chamado para ver detalhes

**Colunas da tabela:**
- Código
- Título
- Prioridade (ALTA, MÉDIA, BAIXA)
- Data Limite
- Status

---

### 2.5 Detalhes e Atualização de Chamado

**Disponível para:** Suporte Técnico e Administradores

Ao clicar em um chamado, você verá:
- Informações completas do chamado
- Campo para adicionar solução
- Opção de alterar status
- Botão **"GERAR SUGESTÃO COM IA"**

**Como atualizar:**
1. Digite a solução no campo correspondente
2. (Opcional) Use a IA para gerar sugestão automática
3. Selecione o novo **status**:
   - Aberto
   - Em Andamento
   - Resolvido
   - Fechado
4. Clique em **"SALVAR ALTERAÇÕES"**

💡 **Dica:** A IA analisa o problema e sugere uma resposta profissional. Revise e edite antes de salvar.

---

### 2.6 Chamados Concluídos

**Disponível para:** Suporte Técnico e Administradores

1. Clique no card **"CHAMADOS CONCLUÍDOS"**
2. Visualize o histórico de chamados resolvidos
3. Use busca e filtros como na página de chamados em andamento
4. Clique em um chamado para ver a solução aplicada

---

### 2.7 Relatórios e Estatísticas

**Disponível para:** Suporte Técnico e Administradores

A página de relatórios exibe:

**Métricas:**
- Total de Usuários
- Total de Chamados
- Chamados Resolvidos
- Chamados Em Andamento

**Usuários por Nível:**
- Colaboradores
- Suporte Técnico
- Administradores

**Status da API:**
- Conexão com banco de dados (Online/Offline)
- Tempo de resposta
- Status do serviço de IA

---

### 2.8 Recursos de Usuários

#### Menu Lateral (Sidebar)

- 🏠 **HOME**: Retorna à página inicial
- 📋 **CHAMADO**: Chamados em andamento (Suporte/Admin)
- 📊 **RELATÓRIOS**: Estatísticas (Suporte/Admin)
- ❓ **FQA**: Manual do sistema
- 📞 **CONTATO**: Informações de contato

#### Cabeçalho (Header)

- **Ícone de Usuário**: Clique para acessar perfil
- **Ícone de Engrenagem**: Menu com opções:
  - 👤 Perfil
  - 🚪 Logout

#### Editar Perfil

1. Clique no ícone de usuário ou "Perfil" no menu
2. Clique em **"EDITAR PERFIL"**
3. Modifique os campos desejados:
   - Nome Completo
   - E-mail
   - Telefone (opcional)
   - Cargo
4. Clique em **"SALVAR ALTERAÇÕES"**

❗ **Nota:** Permissão e senha não podem ser alteradas pelo perfil. Contate o administrador.

---

### 2.9 Recursos Administrativos

**Disponível para:** Apenas Administradores

#### Cadastrar Novo Funcionário

1. Clique no card **"CADASTRO DE FUNCIONÁRIO"**
2. Preencha os campos:
   - Nome Completo
   - E-mail (único)
   - Cargo
   - Senha (mínimo 6 caracteres)
   - **Permissão**: Escolha o nível (1-Colaborador, 2-Suporte, 3-Admin)
   - Telefone (opcional)
3. Clique em **"CADASTRAR"**

**Níveis de Permissão:**

| Nível | Nome | Funcionalidades |
|-------|------|-----------------|
| **1** | Colaborador | Criar chamados, ver próprios chamados |
| **2** | Suporte | Todas de Colaborador + gerenciar todos os chamados + relatórios |
| **3** | Admin | Todas de Suporte + cadastrar funcionários |

❗ **Alerta:** Use senhas temporárias seguras e oriente a troca no primeiro login.

---

## 3. CATÁLOGO DE FUNCIONALIDADES

| ID | Funcionalidade | Descrição | Status |
|----|----------------|-----------|--------|
| F01 | Login | Autenticação via email e senha | ✅ OK |
| F02 | Recuperação de Senha | Link para solicitar redefinição | ✅ OK |
| F03 | Dashboard | Página inicial com cards por permissão | ✅ OK |
| F04 | Criar Chamado | Formulário para criar chamados técnicos | ✅ OK |
| F05 | Validação de Formulários | Validação em tempo real | ✅ OK |
| F06 | Visualizar Chamados | Lista de chamados pendentes (Suporte/Admin) | ✅ OK |
| F07 | Busca e Filtros | Busca e ordenação de chamados | ✅ OK |
| F08 | Detalhes do Chamado | Visualização completa de informações | ✅ OK |
| F09 | Atualizar Status | Alteração de status do chamado | ✅ OK |
| F10 | Adicionar Solução | Campo para registrar solução | ✅ OK |
| F11 | Sugestão com IA | Geração de sugestões de resposta via IA | ✅ OK |
| F12 | Chamados Concluídos | Histórico de chamados resolvidos | ✅ OK |
| F13 | Relatórios | Estatísticas e métricas do sistema | ✅ OK |
| F14 | Status da API | Monitoramento de conexões e serviços | ✅ OK |
| F15 | Editar Perfil | Edição de dados pessoais | ✅ OK |
| F16 | Sidebar | Menu lateral de navegação | ✅ OK |
| F17 | Header | Cabeçalho com informações do usuário | ✅ OK |
| F18 | FQA | Manual interativo do sistema | ✅ OK |
| F19 | Contato | Informações de contato | ✅ OK |
| F20 | Cadastro de Funcionário | Criação de novos usuários (Admin) | ✅ OK |
| F21 | Gerenciamento de Permissões | Sistema de 3 níveis de acesso | ✅ OK |
| F22 | Controle de Acesso | Exibição condicional por permissão | ✅ OK |
| F23 | Logout | Finalização de sessão | ✅ OK |
| F24 | Notificações | Mensagens de feedback (Toast) | ✅ OK |
| F25 | Responsividade | Interface adaptável | ✅ OK |

---

## 4. CONCLUSÃO

O HelpWave centraliza e simplifica a gestão de chamados técnicos com integração de IA para otimizar respostas.

**Principais benefícios:**
- Centralização de solicitações técnicas
- Histórico completo e rastreável
- Acesso diferenciado por níveis
- Integração com IA
- Relatórios e estatísticas
- Interface intuitiva e segura

Para dúvidas adicionais, consulte a página FQA ou entre em contato através da página de contato.

---

**Elaborado por:** Equipe de Desenvolvimento HelpWave  
**Data:** Outubro de 2025  
**São José dos Campos**

# Information Architecture

## Objetivo

A Arquitetura da Informação (Information Architecture – IA) define a organização estrutural do Journal, estabelecendo como seus principais elementos se relacionam e como o usuário navega entre eles.

Diferentemente de uma arquitetura baseada em funcionalidades isoladas, o Journal foi concebido como um ambiente de organização pessoal inspirado em planners e fichários físicos, onde o usuário registra continuamente suas informações em documentos organizados por divisórias.

As ferramentas disponíveis (Agenda, Finanças, Pomodoro, entre outras) complementam essa experiência, mas não representam sua estrutura principal.

---

# Modelo Conceitual

O Journal é composto por cinco conceitos fundamentais.

```text
Journal
│
├── Dashboard
├── Divisórias
├── Documentos
├── Templates
└── Ferramentas
```

Cada um desses elementos possui uma responsabilidade específica dentro da plataforma.

---

# Dashboard

O Dashboard é o ponto inicial do Journal.

Seu objetivo não é apresentar todas as funcionalidades do sistema, mas ajudar o usuário a continuar sua rotina.

O Dashboard prioriza:

- documentos recentes;
- documentos favoritos;
- últimas divisórias acessadas;
- templates utilizados recentemente;
- tarefas pendentes;
- eventos próximos;
- sessões recentes;
- acesso rápido para criar um novo documento.

O Dashboard deve responder à pergunta:

> **"O que você deseja continuar fazendo hoje?"**

---

# Divisórias (Sections)

As divisórias representam os principais agrupadores de conteúdo do Journal.

Inspiradas em fichários e planners físicos, elas organizam documentos relacionados a um mesmo tema.

Exemplos:

- Vestibular
- Faculdade
- Concurso
- Trabalho
- Projetos
- Diário
- Estudos
- Pessoal

Cada usuário poderá criar, renomear, reorganizar e excluir suas próprias divisórias.

---

# Documentos (Documents)

O documento é a unidade principal do Journal.

Todo conteúdo produzido pelo usuário acontece dentro de um documento.

Um documento é uma folha contínua, sem divisão em páginas, permitindo que textos, imagens, diagramas, tabelas, checklists e outros elementos coexistam livremente.

Características:

- rolagem infinita;
- múltiplos tipos de conteúdo;
- salvamento automático;
- histórico de alterações (futuro);
- organização dentro de divisórias.

---

# Blocos (Blocks)

Os documentos são compostos por blocos.

Cada bloco representa um tipo de informação.

Exemplos:

- Texto
- Checklist
- Título
- Imagem
- Arquivo
- Código
- Tabela
- Citação
- Lista
- Diagrama
- Desenho (futuro)

Essa abordagem torna os documentos flexíveis e expansíveis.

---

# Templates

Templates são modelos utilizados para criar novos documentos.

Eles definem uma estrutura inicial, permitindo acelerar tarefas recorrentes.

Exemplos:

- Anotação de aula
- Diário
- Revisão
- Sessão de estudos
- Brainstorm
- Projeto
- Planejamento semanal

Após criado, o documento torna-se independente do template.

---

# Ferramentas

As ferramentas representam funcionalidades complementares do Journal.

Elas não constituem sua estrutura principal, mas interagem com documentos e divisórias.

Inicialmente o Journal contará com ferramentas como:

- Agenda
- Pomodoro
- Finanças (Cofrinho)

Novas ferramentas poderão ser adicionadas futuramente.

---

# Relação entre os elementos

```text
Template
      │
      ▼
Documento
      │
      ▼
Divisória
      │
      ▼
Dashboard
```

As ferramentas podem criar, atualizar ou consultar informações presentes nos documentos, sem alterar sua organização.

---

# Ferramentas Integradas

## Agenda

Responsável pelo gerenciamento de compromissos e eventos.

Integrações possíveis:

- criação de eventos;
- lembretes;
- calendário;
- tarefas;
- notificações.

Os eventos podem ser vinculados a documentos específicos.

---

## Finanças (Cofrinho)

Ferramenta destinada ao controle financeiro pessoal.

Permite registrar:

- receitas;
- despesas;
- categorias;
- metas;
- orçamento.

Registros financeiros podem ser associados a documentos quando fizer sentido.

---

## Pomodoro

Ferramenta voltada para gerenciamento de foco.

Permite:

- iniciar sessões;
- controlar intervalos;
- registrar tempo de estudo;
- atualizar estatísticas.

Uma sessão concluída poderá gerar automaticamente um registro dentro de um documento.

---

# Navegação

A navegação do Journal é composta por três níveis.

## Navegação Global

Sempre disponível.

Permite acessar:

- Dashboard
- Divisórias
- Ferramentas
- Pesquisa
- Perfil
- Configurações

---

## Navegação das Divisórias

Cada divisória funciona como uma árvore de navegação semelhante ao Explorer de um editor de código.

O usuário poderá:

- expandir;
- recolher;
- reorganizar;
- mover documentos.

---

## Navegação dos Documentos

Ao abrir um documento, o foco passa a ser totalmente o conteúdo.

As ferramentas permanecem acessíveis, mas discretas, permitindo concentração durante a escrita.

---

# Escalabilidade

A arquitetura foi planejada para permitir a inclusão de novos recursos sem modificar sua estrutura principal.

Exemplos:

- Assistente de IA
- Gamificação
- Widgets
- Integração com Google Calendar
- Sincronização em nuvem
- Biblioteca de templates
- Compartilhamento de documentos

Todos esses recursos serão adicionados como ferramentas ou serviços complementares, preservando o conceito central do Journal.

---

# Princípio Fundamental

A estrutura do Journal baseia-se em um conceito simples:

> O usuário organiza sua vida por meio de documentos contínuos agrupados em divisórias.

Todas as demais funcionalidades existem para enriquecer essa experiência, nunca para substituí-la.

Esse princípio orientará as decisões de UX, design e desenvolvimento ao longo da evolução do projeto.
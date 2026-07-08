# Information Architecture (IA)

> Versão 1.0

---

# 1. Objetivo

A Arquitetura da Informação do **Journal** define como as funcionalidades e os conteúdos da aplicação são organizados, apresentados e acessados pelo usuário.

Este documento estabelece a estrutura de navegação do sistema, servindo como referência para o desenvolvimento do UX/UI, Front-end, Back-end e modelagem de dados.

---

# 2. Princípios da Arquitetura

O Journal possui dois tipos de elementos:

## Funcionalidades do sistema

São recursos nativos da aplicação.

Existem para todos os usuários.

Exemplos:

- Dashboard
- Agenda
- Cronograma de Estudos
- Finanças
- Pomodoro
- Perfil
- Configurações

Esses elementos fazem parte da estrutura fixa da plataforma.

---

## Conteúdo do usuário

São elementos criados pelo próprio usuário.

Exemplos:

- Divisórias
- Folhas
- Notas
- Cronograma de Estudo Editado


Esses elementos pertencem ao usuário e podem variar conforme sua organização pessoal.

---

# 3. Estrutura Global

```text
Journal
│
├── Dashboard
├── Agenda
├── Notas
├── Cronograma de Estudos
├── Finanças
├── Fichários
├── Pomodoro
├── Perfil
├── Configurações
└── Sobre
```

---

# 4. Dashboard

O Dashboard representa a página inicial da aplicação.

Sua função é apresentar um ambiente de trabalho rápido, oferecendo acesso às atividades recentes e permitindo a criação de novos conteúdos.

## Componentes

### Templates com Últimos acessos (área central)

Exibe os documentos e funcionalidades recentemente utilizados em Templates.

Exemplos:

- Fichário: Matemática
- Agenda
- Finanças
- Cronograma

Limite de 6 templates.

Caso seja primeiro acesso, Templates com as funcionalidades:

- Nova Folha
- Agenda
- Notas
- Cronograma de Estudos
- Finanças
- Nova divisória.

Esses templates poderão ser expandidos futuramente.

### Menu Lateral Esquerdo

Menu lateral esquerdo com links para:

- Agenda
- Notas
- Cronograma de Estudos
- Finanças
- Divisórias (ou Nova divisória)

### Menu Lateral Direito

Menu lateral direito com links as últimas divisórias criadas.

Exemplo:
- Direito Constitucional
- Direito do consumidor
- Documentação Java
- Resumos de Filosofia
- CheatSheet
- Referência Bibliográfica
- + Nova Divisória

Limite até 8 divisórias recém acessadas.

---

# 5. Navegação Principal

A navegação principal é composta por 5 regiões.

## Navbar (Superior)

Elementos:

- Logo Journal
- Nome Journal
- Pomodoro
- Menu Hamburger

### Comportamento

Logo

→ retorna ao Dashboard

Nome Journal

→ retorna ao Dashboard

Pomodoro

→ abre a funcionalidade Pomodoro

Menu Hamburger

→ abre o menu completo da aplicação.

---

## Sidebar Esquerda

Responsável pelas funcionalidades permanentes do sistema.

Itens:

- Agenda
- Notas
- Cronograma de Estudos
- Finanças
- Divisórias (ou Nova divisória)

Esses itens existem independentemente do conteúdo criado pelo usuário.

---

## Sidebar Direita

Responsável pela navegação das Divisórias.

Exemplo:

```text


- Direito Constitucional
- Direito do consumidor
- Documentação Java
- Resumos de Filosofia
- CheatSheet
- Referência Bibliográfica
- + Nova Divisória
```

Caso exista apenas um fichário:

```text
Divisória

- Direito Constitucional

- + Novo Divisória
```

Esta barra é dinâmica e varia conforme os fichários criados pelo usuário.

---

## Footer

Itens previstos:

- © Journal
- Sobre
- Tutorial (futuro)
- Documentação
- Versão da aplicação

---

# 6. Menu Hamburger

O menu Hamburger reúne todas as funcionalidades da aplicação.

Itens:

- Dashboard
- Agenda
- Cronograma de Estudos
- Finanças
- Divisórias
- Pomodoro
- Perfil
- Configurações
- Sobre
- Sair

---

# 7. Organização das Divisórias

As divisórias representam a organização pessoal do usuário.

Exemplo:

```text
Vestibular

├── Matemática
├── Português
├── História
└── Biologia
```

Outro usuário pode possuir uma estrutura completamente diferente.

```text
Universidade

├── Algoritmos
├── Banco de Dados
├── Engenharia de Software
└── UX
```

Definir quantidade máxima com o Back-End.

---

# 8. Organização das Folhas

Cada divisória pode conter diversos folhas.

Exemplos:

- Anotações
- Resumos
- Exercícios
- Listas
- Planejamentos
- Arquivos

A estrutura fica organizada da seguinte forma:

```text
Journal

└── Divisória

    ├── Folha
    ├── Folha
    ├── Folha
    └── Folha
```

---

# 09. Hierarquia da Informação

A estrutura principal do Journal segue a seguinte organização:

```text
Journal

↓

Dashboard

↓

Divisórias

↓

Folha

↓

Conteúdo
```

---
# 10. Modelo Conceitual

O Journal é estruturado a partir de dois grandes conceitos: **funcionalidades do sistema** e **conteúdo criado pelo usuário**.

As funcionalidades fornecem os recursos da plataforma. O conteúdo representa a forma como cada usuário organiza suas informações.

```text
Journal
│
├── Funcionalidades
│   │
│   ├── Dashboard
│   ├── Agenda
│   ├── Notas
│   ├── Cronograma de Estudos
│   ├── Finanças
│   ├── Pomodoro
│   ├── Perfil
│   ├── Configurações
│   └── Sobre
│
└── Conteúdo do Usuário
    │
    ├── Divisórias
    │
    ├── Folhas
    │
    └── Conteúdo
```

## Relação entre os conceitos

O conteúdo criado pelo usuário é organizado de forma hierárquica.

```text
Journal

└── Divisória
    │
    ├── Folha
    │   │
    │   └── Conteúdo
    │
    ├── Folha
    │
    └── Folha
```

Cada **Divisória** funciona como um agrupador lógico de informações.

Cada **Folha** representa uma unidade de trabalho dentro da divisória e pode assumir diferentes formatos, como:

- Nota
- Agenda
- Cronograma de Estudos
- Planejamento Financeiro
- Lista
- Texto livre

O conteúdo de cada folha é definido pelo usuário e pode ser personalizado conforme sua necessidade.

## Princípio do modelo

O Journal não impõe uma estrutura fixa de organização.

Enquanto as funcionalidades permanecem iguais para todos os usuários, as divisórias e folhas são criadas livremente, permitindo que cada pessoa organize seus estudos, projetos e rotina de acordo com sua própria lógica.


# 11. Princípio Fundamental

O Journal separa claramente dois conceitos:

## Funcionalidades

Representam recursos oferecidos pela aplicação.

São fixas e iguais para todos os usuários.

---

## Organização

Representa a forma como cada usuário organiza sua própria vida.

Essa organização é totalmente personalizada através dos Fichários e Divisórias.

Dessa forma, dois usuários podem utilizar exatamente a mesma aplicação, mas possuir estruturas completamente diferentes de organização.

Este princípio orienta toda a Arquitetura da Informação do Journal.
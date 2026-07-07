# User Journey

## Objetivo

A User Journey (Jornada do Usuário) descreve como cada persona interage com o Journal para alcançar seus objetivos.

Seu propósito é compreender as necessidades do usuário em cada etapa da experiência, identificando oportunidades para criar uma interface simples, intuitiva e eficiente.

As jornadas apresentadas representam cenários comuns de utilização do Journal e servirão como referência para o desenvolvimento das funcionalidades, fluxos de navegação e experiência do usuário.

---

# Jornada 1 — Estudante do Ensino Médio

## Persona

**Ana Luiza** — 17 anos

Objetivo: organizar sua rotina para o vestibular.

---

## Cenário

É segunda-feira. Ana acabou de chegar da escola e precisa organizar sua semana antes de iniciar os estudos.

---

## Jornada

### 1. Acessa o Journal

Ana abre o aplicativo e visualiza seu Dashboard.

Ela consegue identificar rapidamente:

- compromissos do dia;
- tarefas pendentes;
- tempo disponível para estudo;
- roteiro de estudo;
- hábitos do dia.

---

### 2. Planeja sua semana

No módulo de Agenda ela:

- adiciona provas;
- registra trabalhos;
- organiza horários do cursinho;
- distribui blocos de estudo.

---

### 3. Organiza os estudos

No módulo de Estudos ela:

- escolhe a disciplina;
- estabelece quanto tempo irá estudá-la e organiza suas pausas;
- cria notas do que fazer durante as pausas de estudo;
- registra o conteúdo estudado;
- marca revisões futuras;
- acompanha seu progresso.

---

### 4. Executa as tarefas

Durante o dia ela conclui atividades e marca tarefas como finalizadas.

O Dashboard é atualizado automaticamente.

---

### 5. Finaliza o dia

Antes de dormir ela:

- registra como foi seu dia;
- acompanha seus hábitos;
- cria um template para uma anamnese relaxante;
- verifica se atingiu sua meta diária.

---

## Resultado esperado

Ana mantém uma rotina organizada e consegue visualizar claramente sua evolução ao longo do tempo.

---

# Jornada 2 — Estudante de Concurso

## Persona

**Lucas Henrique** — 28 anos

Objetivo: equilibrar trabalho, estudos e vida pessoal.

---

## Cenário

Lucas chega do trabalho às 19h e possui apenas três horas para estudar.

---

## Jornada

### 1. Consulta a agenda

Visualiza:

- compromissos;
- horários disponíveis;
- tarefas prioritárias.

---

### 2. Inicia sessão de estudos

Seleciona:

- disciplina;
- conteúdo;
- tempo planejado;
- realiza resumos de matéria, conceitos ou anotações.

O Journal registra a sessão.

---

### 3. Atualiza progresso

Ao terminar os estudos ele registra:

- horas estudadas;
- conteúdo concluído;
- dificuldades encontradas.

---

### 4. Consulta indicadores

Visualiza:

- horas estudadas na semana;
- disciplinas mais estudadas;
- metas alcançadas.

---

### 5. Organiza o dia seguinte

Antes de encerrar:

- revisa anotações;
- agenda novas revisões;
- organiza tarefas;
- registra despesas do dia.

---

## Resultado esperado

Lucas consegue manter consistência na preparação para o concurso mesmo possuindo pouco tempo disponível.

---

# Jornada 3 — Universitária

## Persona

**Mariana Costa** — 22 anos

Objetivo: administrar a rotina universitária.

---

## Cenário

Mariana recebe novas atividades de três disciplinas diferentes durante a semana.

---

## Jornada

### 1. Registra atividades

Adiciona:

- trabalhos;
- provas;
- apresentações;
- prazos.

---

### 2. Organiza prioridades

Distribui as tarefas conforme:

- prazo;
- dificuldade;
- carga horária disponível.

---

### 3. Acompanha a rotina

Consulta diariamente:

- agenda;
- tarefas;
- hábitos;
- anotações e resumos de matéria;
- compromissos.

---

### 4. Controla gastos

Registra despesas relacionadas à universidade.

Exemplos:

- transporte;
- alimentação;
- materiais;
- livros.

---

### 5. Fecha a semana

Analisa:

- tarefas concluídas;
- metas atingidas;
- evolução acadêmica.

---

## Resultado esperado

Mariana consegue manter equilíbrio entre vida acadêmica, pessoal e financeira.

---

# Jornada Geral do Usuário

```text
Cadastro
      │
      ▼
Personalização Inicial
      │
      ▼
Dashboard
      │
      ├──────────────┐
      ▼              ▼
Agenda         Planejamento de Estudos
      │              │
      ├──────┐       │
      ▼      ▼       ▼
Tarefas  Hábitos  Registro de Estudos
      │      │       │
      └──────┴───────┘
             │
             ▼
      Diário / Reflexões
             │
             ▼
 Relatórios e Evolução
             │
             ▼
 Planejamento do Próximo Dia
```

---

# Pontos de Contato

Durante sua jornada, o usuário interage principalmente com:

- Dashboard
- Agenda
- Estudos
- Tarefas
- Hábitos
- Diário
- Controle Financeiro
- Relatórios

Esses módulos representam os principais pontos de contato do usuário com o Journal e concentram a maior parte das interações diárias.

---

# Oportunidades de Experiência

A análise das jornadas evidencia oportunidades importantes para o Journal:

- reduzir o número de telas necessárias para realizar tarefas frequentes;
- apresentar informações relevantes logo no Dashboard;
- minimizar a necessidade de alternar entre diferentes módulos;
- incentivar a continuidade dos hábitos por meio de indicadores visuais;
- facilitar o planejamento diário e semanal.

Essas oportunidades orientarão as decisões de UX, arquitetura da informação e evolução das funcionalidades ao longo do desenvolvimento.
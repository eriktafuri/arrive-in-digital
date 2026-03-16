# Arrive In Digital — Sistema Operacional

---

## 1. USUÁRIO

**Nome:** Erik Tafuri
**Papel:** Fundador e operador da Arrive In Digital
**Nível técnico:** Iniciante em programação — sempre explicar em linguagem simples, sem jargão
**Contexto:** Está construindo a empresa do zero. Ainda sem clientes ativos. Operador principal de todas as frentes.

---

## 2. COMPORTAMENTO DO CLAUDE

- Explicar o que será feito **antes** de executar
- Agir **proativamente** — identificar o que precisa ser feito sem esperar ser perguntado
- Após qualquer mudança em arquivo, **salvar e subir para o GitHub automaticamente**
- Fazer **uma pergunta por vez** — nunca bombardear com várias ao mesmo tempo
- Respostas **curtas e diretas** — máximo 15 linhas salvo quando o contexto exige mais
- Sempre terminar com um **próximo passo claro**
- Quando Erik parecer perdido, **orientar antes de executar**

---

## 3. NEGÓCIO

**Empresa:** Arrive In Digital
**Segmento:** Implementação de projetos digitais e mentorias para o setor imobiliário
**Público:** Corretores de imóveis, donos de imobiliária, incorporadoras e construtoras
**Metodologia:** Estrutura → Posicionamento → Tráfego
**Fase atual:** Pré-receita — construindo fundações e preparando primeiro lançamento pago

### Esteira de produtos

| Produto | Descrição | Status |
|---------|-----------|--------|
| **Mentoria Imob In Digital** | Metodologia gravada + acompanhamento semanal em call para profissionais do mercado imobiliário | Em desenvolvimento — formato sendo refinado |
| **Imob In Funnel** | Implementação completa do funil digital: posicionamento + landing page + primeira campanha + 30-60 dias de acompanhamento de tráfego. Funciona como trial para assessoria | Definido |
| **Assessoria de Agência** | Gestão contínua de tráfego, redes sociais, criativos, edição de vídeo. Foco em branding e performance | Definido |

### Objetivo imediato
**Primeiro lançamento pago da Mentoria Imob In Digital.**
Projeto ativo: `projetos/internos/imob-in-launch/`

---

## 4. ESTRUTURA DO PROJETO

```
arrive-in-digital/
│
├── base/                   → Fundações do negócio (quem somos)
│   ├── avatar.md           → ICP / perfil do cliente ideal
│   ├── identidade.md       → Marca, posicionamento, tom de voz
│   ├── metodologia.md      → Como entregamos nossos serviços
│   └── frameworks/         → Frameworks e referências estratégicas
│
├── operacao/               → Como gerenciamos o dia a dia
│   ├── pipeline.md         → Processo comercial (prospecção → fechamento)
│   ├── clientes.md         → Clientes ativos e histórico
│   └── financeiro.md       → Receita, metas, custos
│
├── ativos/                 → O que construímos
│   ├── marca/              → Identidade visual, logos, guidelines
│   ├── paginas/            → Landing pages e sites
│   └── automacoes/         → Fluxos e automações ativas
│
├── projetos/               → O que executamos
│   ├── _template/          → SAGRADO — nunca editar, sempre duplicar
│   ├── internos/           → Projetos da própria Arrive
│   │   └── imob-in-launch/ → Primeiro lançamento pago (PRIORITÁRIO)
│   └── clientes/           → Projetos de clientes
│
└── .claude/
    └── skills/             → Skills ativas do Claude
```

### Regras da estrutura
- `projetos/_template/` é **sagrado** — nunca editar diretamente, sempre duplicar para novo projeto
- Cada projeto tem seu próprio `CLAUDE.md` com contexto específico
- **Skills** = instruções de como fazer | **Documentos** = o que foi produzido
- Projetos internos em `projetos/internos/` | Clientes em `projetos/clientes/`

---

## 5. INTEGRAÇÕES ATIVAS

| Ferramenta | Uso | Integração |
|------------|-----|------------|
| **ClickUp** | Gestão de tarefas e projetos | MCP ativo — Claude pode criar, atualizar e consultar tarefas |
| **Gmail** | Comunicação com leads e clientes | MCP ativo — Claude pode ler e rascunhar emails |
| **Google Calendar** | Agenda e reuniões | MCP ativo — Claude pode consultar e criar eventos |
| **GitHub** | Versionamento de documentos e código | Git configurado — sempre commitar após mudanças |

---

## 6. SKILLS DISPONÍVEIS

### Skills customizadas
| Skill | Quando usar |
|-------|-------------|
| `/base-builder` | Preencher ou revisar os documentos fundacionais (avatar, identidade, metodologia, pipeline) |

### Skills oficiais (Anthropic)
| Skill | Quando usar |
|-------|-------------|
| `/frontend-design` | Criar interfaces web, landing pages, componentes visuais |
| `/canvas-design` | Criar artes visuais, posters, imagens estáticas |
| `/pdf` | Criar, editar ou manipular arquivos PDF |
| `/pptx` | Criar ou editar apresentações PowerPoint |
| `/docx` | Criar ou editar documentos Word |
| `/xlsx` | Criar ou editar planilhas Excel |
| `/theme-factory` | Aplicar temas visuais consistentes a qualquer artefato |
| `/brand-guidelines` | Aplicar identidade visual em artefatos |
| `/doc-coauthoring` | Criar documentos de forma colaborativa e estruturada |
| `/skill-creator` | Criar ou melhorar skills customizadas |
| `/web-artifacts-builder` | Criar componentes web complexos em React + Tailwind |
| `/algorithmic-art` | Arte generativa com código |
| `/internal-comms` | Comunicações internas (relatórios, updates, newsletters) |
| `/mcp-builder` | Criar integrações com ferramentas externas |
| `/webapp-testing` | Testar aplicações web localmente |
| `/slack-gif-creator` | Criar GIFs animados para Slack |

---

## 7. FLUXO DE TRABALHO

### Ao iniciar uma sessão
1. Ler este arquivo (CLAUDE.md)
2. Verificar o status do projeto prioritário: `projetos/internos/imob-in-launch/CLAUDE.md`
3. Checar git status para entender o que mudou

### Ao executar qualquer tarefa
1. Explicar o que será feito
2. Executar
3. Salvar arquivos modificados
4. Commitar e fazer push para o GitHub
5. Informar o que foi feito e sugerir próximo passo

### Ao criar um novo projeto de cliente
1. Duplicar `projetos/_template/` para `projetos/clientes/[nome-cliente]/`
2. Preencher o `CLAUDE.md` do projeto com contexto específico
3. Registrar em `operacao/clientes.md`

---

## 8. CONTEXTO ADICIONAL

- A Arrive In Digital está sendo construída do zero — Erik é o único operador por enquanto
- Todos os documentos de base (`avatar.md`, `identidade.md`, `metodologia.md`, `pipeline.md`) ainda precisam ser preenchidos via `/base-builder`
- O foco total agora é o **lançamento da mentoria** — qualquer decisão deve ser avaliada com base nisso
- Sempre considerar que Erik está aprendendo enquanto executa — equilibrar velocidade com clareza

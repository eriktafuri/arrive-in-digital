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
| **Mentoria Imob In Digital** | Metodologia gravada + acompanhamento semanal em call | Em desenvolvimento |
| **Imob In Funnel** | Implementação completa do funil: posicionamento + landing page + campanha + 30-60 dias de acompanhamento. Trial para assessoria | Definido |
| **Assessoria de Agência** | Gestão contínua de tráfego, redes sociais, criativos, edição de vídeo. Branding + performance | Definido |

### Objetivo imediato
**Primeiro lançamento pago da Mentoria Imob In Digital.**
Projeto ativo: `projetos/internos/imob-in-launch/`

---

## 4. ESTRUTURA DO PROJETO

```
arrive-in-digital/
│
├── base/                          → DNA da empresa
│   ├── avatar.md                  → ICP / cliente ideal
│   ├── identidade.md              → Marca, posicionamento, tom de voz
│   ├── metodologia.md             → Como entregamos
│   ├── ofertas.md                 → Produtos, preços, o que inclui
│   ├── inteligencia/              → Conhecimento de mercado
│   │   ├── publico.md             → Psicologia profunda do corretor, dores, emoções
│   │   ├── benchmark.md           → Concorrentes, hooks que viralizam, gaps de mercado
│   │   └── objecoes.md            → Objeções mapeadas e como responder
│   └── frameworks/
│       └── estrategias/           → Playbooks gerados pelos projetos (livro de receitas)
│
├── operacao/                      → Como gerenciamos o dia a dia
│   ├── pipeline.md                → Processo comercial (prospecção → fechamento)
│   ├── clientes.md                → Clientes ativos e histórico
│   ├── financeiro.md              → Receita, metas, custos
│   ├── processos.md               → SOPs e checklists operacionais
│   └── aprendizados.md            → O que testamos e o que funcionou
│
├── ativos/                        → Ativos reutilizáveis da empresa
│   ├── marca/                     → Logos, cores, guia visual
│   ├── paginas/                   → Landing pages da Arrive
│   ├── conteudo/                  → Templates de roteiro, copy, legenda
│   └── automacoes/                → Fluxos reutilizáveis
│
├── projetos/                      → O que executamos
│   ├── _template/                 → SAGRADO — nunca editar, sempre duplicar
│   │   ├── CLAUDE.md              → Template completo de contexto do projeto
│   │   ├── 00-briefing/           → cliente.md, objetivos.md, diagnostico.md
│   │   ├── 01-estrategia/         → estrategia.md, narrativa.md, oferta.md
│   │   ├── 02-estrutura/          → ferramentas.md, automacoes.md, checklist.md
│   │   ├── 03-posicionamento/     → bio.md, roteiros/, legendas/, emails/
│   │   ├── 04-trafego/            → campanhas.md, copies/, segmentacao.md, orcamento.md
│   │   ├── 05-ativos/             → paginas/, criativos/, videos/
│   │   └── 06-resultados/         → metricas.md, relatorios/, aprendizados.md
│   ├── internos/                  → Projetos da própria Arrive
│   │   └── imob-in-launch/        → Primeiro lançamento pago (PRIORITÁRIO)
│   └── clientes/                  → Projetos de clientes
│
└── .claude/
    └── skills/                    → Skills ativas do Claude
```

### Regras da estrutura
- `projetos/_template/` é **sagrado** — nunca editar diretamente, sempre duplicar
- Cada projeto tem seu próprio `CLAUDE.md` — é a fonte da verdade daquele projeto
- `base/frameworks/estrategias/` é gerado pelos projetos — não criar do nada
- **Skills** = instruções de como fazer | **Documentos** = o que foi produzido
- Ao encerrar um projeto: extrair playbook genérico para `base/frameworks/estrategias/`

---

## 5. INTEGRAÇÕES ATIVAS

| Ferramenta | Uso | Integração |
|------------|-----|------------|
| **ClickUp** | Gestão de tarefas e projetos | MCP ativo |
| **Gmail** | Comunicação com leads e clientes | MCP ativo |
| **Google Calendar** | Agenda e reuniões | MCP ativo |
| **GitHub** | Versionamento de documentos | Git configurado — sempre commitar após mudanças |

---

## 6. SKILLS DISPONÍVEIS

### Skills customizadas
| Skill | Quando usar |
|-------|-------------|
| `/imob-estrategista` | Criar conteúdo, hooks, roteiros, copy, estratégia — qualquer coisa voltada ao mercado imobiliário |
| `/base-builder` | Preencher ou revisar os documentos fundacionais |

### Skills oficiais (Anthropic)
| Skill | Quando usar |
|-------|-------------|
| `/frontend-design` | Criar interfaces web, landing pages |
| `/canvas-design` | Criar artes visuais, posters |
| `/pdf` | Criar, editar ou manipular PDFs |
| `/pptx` | Criar ou editar apresentações |
| `/docx` | Criar ou editar documentos Word |
| `/xlsx` | Criar ou editar planilhas |
| `/theme-factory` | Aplicar temas visuais consistentes |
| `/brand-guidelines` | Aplicar identidade visual |
| `/doc-coauthoring` | Criar documentos de forma colaborativa |
| `/skill-creator` | Criar ou melhorar skills customizadas |
| `/web-artifacts-builder` | Componentes web em React + Tailwind |
| `/algorithmic-art` | Arte generativa com código |
| `/internal-comms` | Comunicações internas |
| `/mcp-builder` | Criar integrações com ferramentas externas |
| `/webapp-testing` | Testar aplicações web |
| `/slack-gif-creator` | Criar GIFs para Slack |

---

## 7. FLUXO DE TRABALHO

### Ao iniciar uma sessão
1. Ler este arquivo (CLAUDE.md)
2. Verificar status do projeto prioritário: `projetos/internos/imob-in-launch/CLAUDE.md`
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

### Ao encerrar um projeto
1. Documentar resultados em `06-resultados/`
2. Extrair aprendizados em `06-resultados/aprendizados.md`
3. Se houver estratégia nova: gerar playbook em `base/frameworks/estrategias/`
4. Atualizar `operacao/clientes.md` e `operacao/financeiro.md`

---

## 8. CONTEXTO ADICIONAL

- A Arrive está sendo construída do zero — Erik é o único operador por enquanto
- O foco total agora é o **lançamento da mentoria** — qualquer decisão deve ser avaliada com base nisso
- Os projetos geram os frameworks — `base/frameworks/estrategias/` começa vazio e vai sendo preenchido
- Sempre equilibrar velocidade com clareza — Erik está aprendendo enquanto executa

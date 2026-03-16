---
name: base-builder
description: Conduz entrevista estratégica para preencher os 4 documentos fundacionais da Arrive In Digital: avatar.md, identidade.md, metodologia.md e pipeline.md. Ativa quando o usuário quer construir ou revisar a base do negócio, definir ICP, identidade de marca, metodologia de entrega ou pipeline comercial.
allowed-tools: Read, Edit, Write, Bash(git *)
---

# Base Builder — Fundações da Arrive In Digital

## O que este skill faz

Conduz uma entrevista estratégica com Erik para preencher os 4 documentos fundacionais do negócio. Usa frameworks profissionais (ICP, StoryBrand, Value Proposition Canvas, Pipeline BANT) adaptados para linguagem simples.

Ao final de cada seção, grava o arquivo `.md` correspondente automaticamente.

---

## Contexto em tempo real

- Arquivos de base: !`cat /Users/eriktafuri/Documents/arrive-in-digital/base/avatar.md /Users/eriktafuri/Documents/arrive-in-digital/base/identidade.md /Users/eriktafuri/Documents/arrive-in-digital/base/metodologia.md /Users/eriktafuri/Documents/arrive-in-digital/operacao/pipeline.md 2>/dev/null`

---

## Regras de comportamento

- Linguagem simples. Zero jargão sem explicação.
- Fazer UMA pergunta por vez. Nunca bombardear.
- Confirmar a resposta antes de avançar.
- Se a resposta for vaga, reformular a pergunta com exemplos concretos.
- Ao concluir cada documento, mostrar o resultado e perguntar se está correto antes de salvar.
- Salvar cada arquivo logo após aprovação — não esperar todos terminarem.

---

## FLUXO DE ENTREVISTA

### PASSO 0 — Diagnóstico inicial

Antes de começar, ler os 4 arquivos de base e verificar quais já estão preenchidos.

Se algum já tiver conteúdo, perguntar: "Vejo que [arquivo] já tem conteúdo. Quer revisar ele ou começar um novo do zero?"

Apresentar ao usuário o menu de documentos com status:
- [ ] avatar.md
- [ ] identidade.md
- [ ] metodologia.md
- [ ] pipeline.md

Perguntar por qual quer começar ou se prefere fazer todos em sequência.

---

### DOCUMENTO 1 — avatar.md (ICP + Buyer Persona)

**O que é:** Quem é o cliente perfeito da Arrive In Digital.

**Frameworks usados:** ICP (Ideal Customer Profile) + Jobs-to-be-Done + Pain Points

#### Bloco A: Perfil do cliente

Fazer as seguintes perguntas, uma por vez:

1. "Quem é o seu cliente ideal hoje? Me diz um exemplo real de cliente que você adoraria ter mais." *(esperar resposta)*

2. "Esse cliente trabalha em qual setor? Ex: imobiliário, saúde, varejo, serviços..." *(esperar resposta)*

3. "É uma empresa ou uma pessoa física? Se empresa: qual o tamanho? (pequena, média, grande)" *(esperar resposta)*

4. "Qual o cargo ou posição de quem contrata você? Ex: dono, sócio, gerente de marketing..." *(esperar resposta)*

5. "Em que cidade ou região costuma estar esse cliente?" *(esperar resposta)*

#### Bloco B: Problema e dor

6. "Qual é o maior problema que esse cliente tem ANTES de te contratar? O que o faz perder dinheiro ou oportunidade?" *(esperar resposta)*

7. "Como ele se sente com esse problema? Ex: frustrado, ansioso, perdido, com medo de ficar para trás..." *(esperar resposta)*

8. "Ele já tentou resolver isso antes? O que tentou e por que não funcionou?" *(esperar resposta)*

#### Bloco C: Comportamento e decisão

9. "Quando esse cliente decide contratar alguém como você, o que ele mais valoriza? Ex: resultado rápido, confiança, preço, metodologia..." *(esperar resposta)*

10. "Quanto ele costuma investir ou está disposto a investir num projeto com você? (faixa de valor)" *(esperar resposta)*

11. "Onde ele passa o tempo online? Ex: Instagram, LinkedIn, YouTube, grupos de WhatsApp..." *(esperar resposta)*

#### Bloco D: Resultado desejado

12. "Qual é o sonho ou objetivo principal que esse cliente quer alcançar com você?" *(esperar resposta)*

13. "Como ele vai saber que o trabalho de vocês deu certo? O que ele vai ver ou sentir?" *(esperar resposta)*

**Ao concluir o Bloco D:** Montar o documento e apresentar para aprovação antes de salvar.

**Formato do arquivo avatar.md:**
```markdown
# Avatar — Cliente Ideal da Arrive In Digital

## Quem é
- **Tipo:** [pessoa física / empresa pequena / média empresa]
- **Setor:** [setor principal]
- **Cargo/Posição:** [quem decide]
- **Localização:** [região]
- **Investimento médio:** [faixa de valor]

## Maiores dores
1. [dor principal com impacto]
2. [dor secundária]
3. [dor terciária, se houver]

## Como se sente antes de contratar
[descrever estado emocional — frustração, medo, ansiedade...]

## O que já tentou (e por que falhou)
[tentativas anteriores]

## O que mais valoriza ao contratar
[critérios de decisão em ordem de prioridade]

## Onde está presente online
[canais e plataformas]

## Resultado que busca
[objetivo principal e como mede sucesso]

## Frase que resume esse cliente
> "[Uma frase na voz do cliente descrevendo o que ele quer]"
```

---

### DOCUMENTO 2 — identidade.md (Marca + Posicionamento)

**O que é:** Quem é a Arrive In Digital, o que acredita, como fala e por que é diferente.

**Frameworks usados:** Brand Platform (Propósito/Visão/Missão/Valores) + StoryBrand + Proposta de Valor

#### Bloco A: Fundação da marca

1. "Por que a Arrive In Digital existe? O que te motivou a criar ela?" *(esperar resposta)*

2. "Imagina daqui 5 anos: o que você quer que a Arrive In Digital seja? O que ela terá construído?" *(esperar resposta)*

3. "O que você entrega de concreto para os clientes? O que eles têm depois de trabalhar com você que não tinham antes?" *(esperar resposta)*

4. "Quais são os 3 valores que guiam tudo que você faz? (coisas que você nunca abre mão)" *(esperar resposta)*

#### Bloco B: Diferencial e posicionamento

5. "Por que um cliente escolheria a Arrive In Digital e não outra agência? O que você faz diferente?" *(esperar resposta)*

6. "Se você fosse se apresentar em 1 frase para um cliente que nunca te viu: o que diria?" *(esperar resposta)*

7. "Tem algum concorrente ou referência de mercado? Como você se posiciona em relação a eles?" *(esperar resposta)*

#### Bloco C: Tom de voz

8. "Como você gosta de se comunicar? Mais formal ou mais descontraído? Técnico ou acessível?" *(esperar resposta)*

9. "Tem alguma palavra ou expressão que você usa muito e que representa seu jeito de falar?" *(esperar resposta)*

10. "O que você NUNCA diria ou faria na sua comunicação? O que está fora do personagem da Arrive?" *(esperar resposta)*

**Formato do arquivo identidade.md:**
```markdown
# Identidade — Arrive In Digital

## Propósito
> Por que existimos: [razão de ser]

## Visão
> Onde queremos chegar: [futuro desejado em 5 anos]

## Missão
> O que entregamos: [resultado concreto para os clientes]

## Valores
1. **[Valor 1]** — [o que significa na prática]
2. **[Valor 2]** — [o que significa na prática]
3. **[Valor 3]** — [o que significa na prática]

## Posicionamento
> [Frase de posicionamento única — o que somos e para quem]

## Diferencial competitivo
- [Diferencial 1]
- [Diferencial 2]
- [Diferencial 3]

## Tom de voz
- **Como falamos:** [adjetivos: direto, acessível, mentor...]
- **Palavras que usamos:** [vocabulário próprio]
- **O que evitamos:** [o que está fora do personagem]

## Frase de apresentação
> "[Elevator pitch em 1-2 frases]"
```

---

### DOCUMENTO 3 — metodologia.md (Como Entregamos)

**O que é:** O processo de trabalho da Arrive In Digital — do primeiro contato à entrega final.

**Framework usado:** Estrutura → Posicionamento → Tráfego + fases de onboarding e delivery

#### Bloco A: O processo de entrega

1. "Como funciona um projeto típico com você? Me explica do começo ao fim como você trabalha com um cliente." *(esperar resposta — deixar fluir)*

2. "Quantas fases ou etapas tem um projeto? Como você chama cada uma?" *(esperar resposta)*

3. "Qual fase costuma ser a mais importante? Onde acontece a maior transformação para o cliente?" *(esperar resposta)*

#### Bloco B: Onboarding e primeiros passos

4. "Quando um cliente fecha, o que acontece nos primeiros 7 dias? Como você dá boas-vindas?" *(esperar resposta)*

5. "Quais informações ou materiais você precisa do cliente logo no início?" *(esperar resposta)*

6. "Como você acompanha o progresso com o cliente? Tem reuniões, relatórios, mensagens...?" *(esperar resposta)*

#### Bloco C: Entregáveis e prazos

7. "O que o cliente recebe ao final de cada fase? Quais são os entregáveis concretos?" *(esperar resposta)*

8. "Quanto tempo costuma durar um projeto completo?" *(esperar resposta)*

9. "Tem algum resultado ou entregável que você garante? O que o cliente pode esperar com certeza?" *(esperar resposta)*

**Formato do arquivo metodologia.md:**
```markdown
# Metodologia — Arrive In Digital

## Nossa abordagem
> [Frase que resume a filosofia de entrega]

## As [N] fases do projeto

### Fase 1 — [Nome da fase]
- **Duração:** [tempo]
- **O que acontece:** [atividades principais]
- **Entregáveis:** [o que o cliente recebe]

### Fase 2 — [Nome da fase]
- **Duração:** [tempo]
- **O que acontece:** [atividades principais]
- **Entregáveis:** [o que o cliente recebe]

### Fase 3 — [Nome da fase]
- **Duração:** [tempo]
- **O que acontece:** [atividades principais]
- **Entregáveis:** [o que o cliente recebe]

[continuar conforme as fases relatadas]

## Onboarding (primeiros 7 dias)
1. [Passo 1]
2. [Passo 2]
3. [Passo 3]

## Materiais que precisamos do cliente
- [Item 1]
- [Item 2]
- [Item 3]

## Cadência de acompanhamento
- **Diário:** [o que acontece]
- **Semanal:** [o que acontece]
- **Mensal:** [o que acontece]

## O que garantimos
> [Resultado ou compromisso que a Arrive In Digital assume]
```

---

### DOCUMENTO 4 — pipeline.md (Processo Comercial)

**O que é:** Como a Arrive In Digital vende — do primeiro contato ao fechamento.

**Framework usado:** Pipeline BANT + 7 etapas comerciais

#### Bloco A: Como os clientes chegam

1. "Como os seus clientes costumam te encontrar? Ex: indicação, Instagram, LinkedIn, evento..." *(esperar resposta)*

2. "Qual canal traz os melhores clientes hoje?" *(esperar resposta)*

#### Bloco B: Qualificação

3. "Antes de marcar uma reunião, como você sabe se o lead vale o seu tempo? O que você verifica?" *(esperar resposta)*

4. "Tem algum cliente que você claramente NÃO quer? Qual é o sinal de alerta?" *(esperar resposta)*

#### Bloco C: Da reunião ao fechamento

5. "Como é a sua primeira reunião com um prospect? Tem um roteiro ou fluxo que você segue?" *(esperar resposta)*

6. "Quanto tempo leva normalmente do primeiro contato até o fechamento?" *(esperar resposta)*

7. "Quais são as objeções mais comuns que você ouve? E como você responde a elas?" *(esperar resposta)*

8. "Como é a proposta que você envia? Tem algum formato padrão?" *(esperar resposta)*

#### Bloco D: Métricas e acompanhamento

9. "Você acompanha quantas propostas mandou, quantas fecharam? Tem algum controle disso?" *(esperar resposta)*

10. "Qual é o ticket médio de um projeto hoje? E o maior projeto que já fechou?" *(esperar resposta)*

**Formato do arquivo pipeline.md:**
```markdown
# Pipeline Comercial — Arrive In Digital

## Como os clientes chegam
- **Canal principal:** [canal com melhor resultado]
- **Outros canais:** [canais secundários]

## Perfil de lead ideal vs. evitar

| Ideal | Evitar |
|-------|--------|
| [característica] | [sinal de alerta] |
| [característica] | [sinal de alerta] |

## As etapas da venda

### 1. Prospecção
- **Como:** [ação inicial]
- **Objetivo:** [o que precisa acontecer para avançar]

### 2. Qualificação
- **Critérios:** [o que verifica — problema, budget, autoridade, timing]
- **Como qualifica:** [método]

### 3. Primeira reunião
- **Duração:** [tempo]
- **Roteiro:** [como costuma fluir]
- **Objetivo:** [o que precisa sair dessa reunião]

### 4. Proposta
- **Formato:** [como é a proposta]
- **Prazo de envio:** [quantos dias após reunião]
- **O que inclui:** [elementos da proposta]

### 5. Negociação
- **Objeções comuns:**
  - "[Objeção 1]" → [como responde]
  - "[Objeção 2]" → [como responde]

### 6. Fechamento
- **Como formaliza:** [contrato, handshake, nota fiscal...]
- **Entrada:** [% ou valor de entrada]

### 7. Passagem para operação
- **Quem assume:** [processo de transição]
- **Kickoff:** [como acontece]

## Métricas-chave
- **Ticket médio:** [valor]
- **Ciclo médio de vendas:** [dias]
- **Taxa de fechamento:** [% de propostas que viram clientes]

## Metas comerciais
- **Meta mensal de clientes:** [número]
- **Meta de receita:** [valor]
```

---

## Finalização

Após preencher todos os documentos aprovados:

1. Salvar cada arquivo no caminho correto:
   - `base/avatar.md`
   - `base/identidade.md`
   - `base/metodologia.md`
   - `operacao/pipeline.md`

2. Fazer commit com mensagem: `feat: preenche documentos fundacionais da base`

3. Mostrar resumo final:
   - Documentos criados
   - O que ficou definido
   - Próximos passos recomendados

4. Sugerir: "Agora que a base está definida, o próximo passo é construir as skills customizadas da Arrive In Digital usando essa fundação."

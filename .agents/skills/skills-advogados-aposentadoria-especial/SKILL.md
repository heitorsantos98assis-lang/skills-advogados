---
name: skills-advogados-aposentadoria-especial
description: "Conduz aposentadoria especial (Lei 8.213 art. 57; EC 103/2019 art. 19) com tempo especial 15/20/25 anos, conversão para comum, PPP e LTCAT, e neutralização por EPI."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Codex, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Trabalhador exposto a agentes nocivos (físicos, químicos, biológicos) à saúde de forma habitual e permanente:
- **15 anos**: trabalho em atividades de mineração subterrânea
- **20 anos**: amianto, atividades de elevada nocividade (algumas)
- **25 anos**: regra geral (ruído, calor, eletricidade > 250V, agentes biológicos, periculosidade aposentação especial)

## Mudanças com EC 103/2019

### Antes (até 13/11/2019)
- Tempo: 15/20/25 anos
- Sem idade mínima
- Cálculo: 100% da média

### Pós-EC 103 (regra geral)
- Tempo: 15/20/25 anos
- **Idade mínima**: 55 anos (15 anos), 58 anos (20 anos), 60 anos (25 anos)
- Pontos (regra do pontos especial): 66 (15a) / 76 (20a) / 86 (25a) — soma idade + tempo

### Regra de transição (art. 21 EC 103)
- Pontos progressivos
- 66 + 0,5 ponto/ano até 76 (15a) / 86 (20a) / 86 (25a)

### Direito adquirido
Quem completou requisitos antes de 13/11/2019 pode aposentar pela regra antiga.

## Inputs necessários

1. **PPP (Perfil Profissiográfico Previdenciário)** — emitido pela empresa, com dados do agente nocivo, intensidade, EPI
2. **LTCAT** (Laudo Técnico das Condições Ambientais do Trabalho)
3. CTPS + CNIS
4. Eventual fechamento da empresa: PPP arquivado em sindicato / cartórios
5. Procuração

## Conversão de tempo especial → comum

Para o segurado que tem tempo especial **mas** quer a aposentadoria por tempo de contribuição comum, pode converter:

| Tempo especial | Multiplicador para homem | Para mulher |
|---|---|---|
| 25 anos → comum | × 1,4 | × 1,2 |
| 20 anos → comum | × 1,75 | × 1,5 |
| 15 anos → comum | × 2,33 | × 2,0 |

**Importante**: a EC 103/2019 vetou a conversão para tempo posterior a 13/11/2019 (ADI 6.309 e jurisprudência). Períodos anteriores podem ser convertidos.

## Agentes nocivos (Decreto 3.048/99 Anexo IV)

### Físicos
- Ruído acima do limite (atual 85 dB(A), antes 90 dB)
- Calor (IBUTG > limite)
- Frio
- Vibrações
- Radiações ionizantes
- Pressões anormais

### Químicos
- Amianto
- Benzeno e derivados
- Chumbo
- Cromo
- Mercúrio
- Sílica
- Hidrocarbonetos

### Biológicos
- Microorganismos (hospitais, lixo, esgoto)
- Vetores

### Periculosidade especial (jurisprudência)
- Eletricidade > 250V (Tema 211 STJ — antes do RPS reformado)
- Vigilância armada (Tema 1.031 STJ)

## Neutralização por EPI

- Súmula 9 TNU (revisada): EPI eficaz **neutraliza** salvo ruído (não neutraliza independentemente do EPI — Tema 555 STF)
- Discussão pode ser técnica caso a caso

## Estrutura

```
EXMO. SR. JUIZ FEDERAL / DA __ª VARA PREVIDENCIÁRIA

[SEGURADO]

vem propor

AÇÃO DE CONCESSÃO DE APOSENTADORIA ESPECIAL

em face do INSS

I — DOS FATOS
1. O autor exerceu de __/__/____ a __/__/____ a função de __________ na empresa __________, exposto aos seguintes agentes nocivos:
   - [Listar agentes do PPP/LTCAT]
2. Total de tempo especial: __ anos
3. PPP e LTCAT em anexo
4. DER: __/__/____ — indeferida sob argumento __________

II — DO DIREITO
2.1. Da exposição habitual e permanente
2.2. Do tempo de 25 anos (ou 15/20)
2.3. Da regra aplicável (transição EC 103 art. 19/21 ou direito adquirido)
2.4. Da neutralização do EPI (Tema 555 STF — ruído não neutraliza)

III — DOS PEDIDOS
a) Tutela provisória: implantação imediata
b) Citação do INSS
c) Procedência para:
   c.1) Reconhecer o tempo especial dos períodos __ a __
   c.2) Conceder a aposentadoria especial com DIB em __/__/____ (DER)
   c.3) Pagar atrasados desde DER, com correção e juros
   c.4) Determinar conversão de tempo se aplicável
d) Honorários, gratuidade
```

## Cuidados

### PPP eletrônico (eSocial)
- A partir de 2023, PPP gerado automaticamente do eSocial S-2240 / Reinf
- Empresa não emite mais PPP separado para períodos sob eSocial

### Empresa fechada
- PPP retroativo: pode ser solicitado em sindicato / federações
- Se inviável: laudo paradigmático (de outra empresa similar) + jurisprudência permite

### Categorias profissionais consideradas especiais até 1995 (antes do Decreto 2.172/97)
- Telefonista, motorista de ônibus/caminhão, etc.
- Categoria automaticamente especial (sem precisar provar agente nocivo) — Súm 198 TFR / jurisprudência

### Atividade insalubre × periculosa
- Insalubridade: agentes nocivos à saúde (com adicional CLT 192)
- Periculosidade: risco de vida (CLT 193)
- Ambos podem dar direito a especial dependendo do agente

### Vedação de continuidade na atividade
Aposentado especial não pode continuar trabalhando na mesma atividade especial (Lei 8.213 art. 57 § 8º). Se continuar, INSS suspende o benefício (Tema 709 STF — discussão de constitucionalidade resolvida).

## Erros comuns

- PPP com dados incompletos → indeferimento administrativo.
- Não juntar LTCAT (ou laudo do PPRA contemporâneo).
- Esquecer Tema 555 STF (ruído sempre nocivo).
- Aplicar multiplicador errado de conversão.
- Confundir aposentadoria especial com adicional de insalubridade (são institutos diferentes).
- Período pós EC 103/2019: tentar converter — vedado.

## Checklist

- [ ] PPP completo (todos os campos)
- [ ] LTCAT
- [ ] CNIS + CTPS
- [ ] Períodos especiais identificados e somados
- [ ] Conversão (se for o caso) com multiplicador correto
- [ ] Idade mínima cumprida (regra geral) ou pontos (transição)
- [ ] Direito adquirido até 13/11/2019 (se aplicável)
- [ ] Tutela urgência
- [ ] Atrasados desde DER
- [ ] Procuração

## Referências

- Lei 8.213/1991 art. 57-58
- Lei 8.212/1991
- Decreto 3.048/1999 art. 64-70 + Anexo IV
- EC 103/2019 arts. 19, 21
- Tema 555 STF (ruído + EPI)
- Tema 709 STF (vedação continuação)
- Tema 1.031 STJ (vigilante)
- Súmulas TNU 9, 32, 87
- IN INSS 128/2022

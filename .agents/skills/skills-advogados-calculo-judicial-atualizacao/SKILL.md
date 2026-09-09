---
name: skills-advogados-calculo-judicial-atualizacao
description: "Atualiza valores judiciais (cíveis, trabalhistas, previdenciários, tributários) com índices corretos, juros, multas e honorários, considerando CC 406, Lei 8.177/91, Tema 905 STJ, Selic."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Claude, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Para atualizar quantia em qualquer ação. Skill operacional. Cálculos errados = peças rejeitadas, devoluções, retrabalho.

## Inputs necessários

1. Valor histórico
2. Data inicial (vencimento, evento, citação)
3. Data final (sentença, hoje, pagamento)
4. Tipo de obrigação (contratual, extracontratual, tributária, trabalhista, previdenciária)
5. Existência de multa contratual / sucumbenciais

## Índices de correção monetária (visão geral)

| Origem | Período | Índice típico |
|---|---|---|
| Tributária federal | Sempre | Selic (Lei 9.430 art. 39) |
| Tributária estadual | Conforme estado | TR + Selic ou TR + 1% (verificar lei estadual) |
| Civil contratual | 1991+ | TR (BACEN), depois IPCA conforme jurisprudência |
| Civil extracontratual | 1996+ | INPC (Tema 905 STJ) ou IPCA-E |
| Trabalhista | até 2017 | TR + 1% a.m. |
| Trabalhista pós Reforma | 2017+ | TR (mas STF ADI 5.867 declarou inconstitucional) → IPCA + Selic |
| Previdenciária (atrasados) | Sempre | INPC (Tema 810 STF) e juros pela poupança até 2021 + Selic |
| FGTS | Conta vinculada | TR + 3% a.a. |

## Atualização — civil cível

### Tema 905 STJ (REsp 1.495.146)

| Tipo | Correção | Juros |
|---|---|---|
| Contratual | INPC (Tema 905) ou previsto contratualmente | 1% a.m. da citação ou conforme contrato |
| Extracontratual | INPC | 1% a.m. desde o evento (Súm 54 STJ) |
| Dano moral | INPC desde arbitramento (Súm 362 STJ) | 1% a.m. desde evento (extra) ou citação (contratual) |
| Repetição indébito CDC | INPC | 1% a.m. desde cada cobrança |

## Atualização — trabalhista

### Antes da Reforma (até 11/11/2017)
- Correção: TR + 1% a.m. (Súm 200 TST)

### Pós Reforma (Lei 13.467/17 alterou CLT 879)
- TR como índice → STF ADI 5.867 declarou inconstitucional
- Atualmente: **IPCA-E** (Súm STJ não específica) na fase pré-judicial e **Selic** na fase processual (a partir da citação)

### Tema 1.191 STF (ADCs 58 e 59)
- IPCA-E (pré-judicial) + Selic (judicial)
- Reforma de 2024 trouxe ajustes específicos (acompanhar)

## Atualização — previdenciária

### Tema 810 STF + Tema 905 STJ
- Correção: **INPC** (Súm 9 TNU)
- Juros: poupança (TR + 0,5% a.m.) até 12/2021, **Selic** depois (Lei 9.494)
- Atrasos do INSS: cuidado com a data de cada benefício

## Atualização — tributária

### Selic (Lei 9.430/96 art. 39)
- Aplicada a partir do 1º dia do mês seguinte ao do pagamento indevido (ou ao do recolhimento) até o pagamento
- Selic mensal acumulada
- Em janeiro do mês de pagamento: + 1%

### ICMS / ISS / outros
- Conforme legislação estadual / municipal
- Em São Paulo: TR + 1% a.m. (LE 6.374/89)

## Multa contratual

```
Multa = % × Principal atualizado
Aplicação: na data do vencimento ou conforme contrato
```

## Honorários (CPC 85)

### Cumprimento de sentença
- 10% sobre o valor (CPC 523 § 1º)

### Sucumbência (sentença)
- 10-20% sobre valor da condenação (CPC 85 § 2º)
- Fazenda: escala progressiva (§ 3º)
- Recursais (§ 11): adicional de 1-5% até teto

## Cálculo passo a passo (exemplo civil contratual)

```
Dado:
- Principal: R$ 10.000
- Vencimento: 01/04/2024
- Citação: 15/06/2024
- Sentença: 01/03/2026
- Pagamento: 01/05/2026

CORREÇÃO MONETÁRIA (INPC):
INPC acumulado de 04/2024 a 05/2026 = (verificar IBGE)
Suponhamos: 8% (ilustrativo)
R$ 10.000 × 1,08 = R$ 10.800

JUROS DE MORA:
Desde a citação (15/06/2024 a 01/05/2026 = ~22,5 meses)
1% a.m. × 22,5 = 22,5% sobre principal corrigido
R$ 10.800 × 22,5% = R$ 2.430

MULTA CONTRATUAL (10% no contrato):
R$ 10.800 × 10% = R$ 1.080

HONORÁRIOS SUCUMBENCIAIS (15% sobre condenação):
(10.800 + 2.430 + 1.080) × 15% = R$ 2.146,50

TOTAL: R$ 10.800 + R$ 2.430 + R$ 1.080 + R$ 2.146,50 = R$ 16.456,50
```

## Atualização para cumprimento (CPC 523)

Após sentença não paga em 15 dias:
- Multa de 10% sobre o valor (CPC 523 § 1º)
- Honorários adicionais de 10%

## Ferramentas

- Calculadora do CNJ
- Calculadora da Justiça Federal (PJe)
- DRCALC (calculadora previdenciária)
- Calculadora do CJF/AGU
- IBGE — IPCA, IPCA-E, INPC
- BACEN — Selic
- Fixed income data — IGP-M, INCC, CDI

## Erros comuns

- Aplicar índice contratual quando há tese de não cumulatividade.
- Esquecer Súm 54 / Súm 362 STJ (juros em data diferente da correção).
- Calcular a TR puramente (declarada inconstitucional para trabalhista).
- Aplicar Selic em todas as fases sem distinguir antes / depois da modulação.
- Esquecer Lei 14.905/2024 — alterou índices civis (Selic + IPCA conforme novo regime?). Verificar atualizações.
- Repetição em dobro: dobrar a totalidade quando deveria ser apenas o indevido.

## Checklist

- [ ] Tipo de obrigação (contratual / extracontratual / tributária / trabalhista / previdenciária)
- [ ] Índice de correção correto e período aplicável
- [ ] Juros: percentual + data de início
- [ ] Multa contratual (se prevista)
- [ ] Honorários sucumbenciais (CPC 85)
- [ ] Cálculo passo a passo demonstrado
- [ ] Atualização até a data da peça/audiência
- [ ] Calculadora oficial usada (CNJ / JF)

## Referências

- CC arts. 389, 397, 405, 406
- Lei 9.430/1996 art. 39 (Selic tributária)
- Lei 8.177/1991 (TR)
- Lei 14.905/2024 (alterações em juros civis)
- CPC art. 85, 523
- Súmulas STJ 54, 362
- Tema 905 STJ
- Tema 810 STF
- Tema 1.191 STF
- ADIs 5.867 / 6.021 STF

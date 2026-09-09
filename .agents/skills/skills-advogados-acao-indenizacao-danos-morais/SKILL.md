---
name: skills-advogados-acao-indenizacao-danos-morais
description: "Estrutura ação de indenização por danos morais com responsabilidade contratual ou extracontratual, valor sugerido, jurisprudência por tipo (negativação indevida, falha bancária, extravio bagagem, perda objeto), e juros pela Súmula 54/362 STJ."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Claude, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Quando o cliente sofreu lesão a direitos da personalidade (honra, imagem, intimidade) ou ofensa significativa em relação contratual / extracontratual. Não cabe **mero aborrecimento** (Súmula 35 TJSP, jurisprudência consolidada STJ).

## Inputs necessários

1. Cliente (qualificação)
2. Réu (qualificação — empresa, banco, plano de saúde, comerciante)
3. Documentos comprobatórios do dano (extratos, prints, contratos, e-mails, testemunhas)
4. Comprovação da relação (contratual ou extracontratual)
5. Tentativas de solução extrajudicial (PROCON, ouvidoria, e-mails) — fortalece o pedido
6. Valor pretendido (com base em jurisprudência similar)

## Tipo de responsabilidade

### Contratual (CC 389-405)
- Há contrato entre as partes
- Mora desde o vencimento (mora ex re) ou desde a interpelação (mora ex persona)
- Juros: a partir da citação (Súmula sem número, mas Súmula 54 STJ se aplica em extracontratual)

### Extracontratual / Aquiliana (CC 186-188, 927)
- Sem relação contratual
- Juros: desde o evento danoso (**Súmula 54 STJ**)

### Consumerista (CDC arts. 12, 14)
- Defeito de produto (12) ou serviço (14): responsabilidade objetiva
- Vício (18, 20): repara ou indeniza
- Inversão do ônus da prova (CDC 6º VIII)

## Súmulas relevantes

| Súmula | Conteúdo |
|---|---|
| 326 STJ | Procedência parcial não enseja sucumbência recíproca quando o pedido é arbitrado pelo juiz |
| 362 STJ | Correção monetária a partir do **arbitramento** |
| 54 STJ | Juros de mora desde o **evento** (extracontratual) |
| 388 STJ | Mero aborrecimento ≠ dano moral (em regra) |
| 385 STJ | Negativação anterior subsistente afasta dano moral |
| 479 STJ | Banco responde objetivamente por fraude |

## Valor da indenização (parâmetros 2024-2026)

> Valores são referência, ajustar caso a caso. Tribunais usam dupla finalidade (compensatória + pedagógica).

| Hipótese | Faixa típica STJ |
|---|---|
| Negativação indevida (sem prejuízo extra) | R$ 5.000 a R$ 15.000 |
| Negativação indevida + recusa crédito comprovada | R$ 10.000 a R$ 25.000 |
| Falha bancária (saque indevido, fraude) | R$ 5.000 a R$ 30.000 |
| Plano de saúde — recusa de procedimento | R$ 10.000 a R$ 50.000 |
| Extravio de bagagem (vôo internacional) | R$ 5.000 a R$ 15.000 (sem CV de Montreal) ou limitado pela CV |
| Atraso de voo > 4h | R$ 3.000 a R$ 10.000 |
| Cancelamento de voo + pernoite | R$ 10.000 a R$ 20.000 |
| Falecimento (filho/cônjuge) | R$ 100.000 a R$ 500.000+ |
| Acidente do trabalho com sequela | Variado, função do grau de invalidez |
| Inscrição cadastral (CADIN, SPC) por dívida quitada | R$ 8.000 a R$ 15.000 |
| Erro médico com sequela | R$ 50.000 a R$ 300.000 |

## Estrutura

```
[Cabeçalho — Vara Cível competente]

I — DOS FATOS
1. [Narrar cronologia do evento]
2. [O comportamento do réu que gerou o dano]
3. [O dano à pessoa do autor — sentimentos, repercussões]
4. [Tentativas de solução extrajudicial]

II — DO DIREITO
2.1. Da relação [contratual/consumerista/extracontratual]
2.2. Da conduta ilícita do réu (CC 186, 187 / CDC 12, 14)
2.3. Do nexo causal
2.4. Do dano moral configurado
   [Argumentar que ultrapassa o mero aborrecimento, atinge direito da personalidade — CC 11-21]

III — DA QUANTIFICAÇÃO
3.1. Critérios (gravidade, repercussão, capacidade econômica do ofensor, pedagogia)
3.2. Jurisprudência similar (citar 2-3 acórdãos do TJ ou STJ)
3.3. Valor sugerido: R$ __________ (ou conforme arbitramento — Súm 326 STJ)

IV — DOS PEDIDOS
a) Citação do réu;
b) Procedência para condenar o réu ao pagamento de:
   b.1) Indenização por danos morais no valor de R$ __________, com correção monetária a partir do arbitramento (Súm 362 STJ) e juros de mora de 1% a.m. a partir [do evento — Súm 54 STJ / da citação — contratual];
   b.2) Custas processuais e honorários sucumbenciais (CPC 85);
c) Inversão do ônus da prova (CDC 6º VIII), se aplicável;
d) Concessão dos benefícios da gratuidade de justiça (Lei 1.060/50 + CPC 98);
e) Produção de prova testemunhal e documental complementar.

V — DO VALOR DA CAUSA
R$ __________ (valor pretendido).
```

## Tutela de urgência (CPC 300)

Comum em casos de:
- Negativação indevida → liminar para retirar do SPC/Serasa
- Plano de saúde → autorização de procedimento
- Bloqueio judicial de cartão clonado

```
III.A — DA TUTELA DE URGÊNCIA
Há probabilidade do direito (anexo prova) e perigo de dano (autor depende da retirada da negativação para conseguir crédito). Requer:
a) Em sede liminar, a retirada do nome do autor dos cadastros restritivos no prazo de 5 dias, sob pena de multa diária de R$ 500.
```

## Erros comuns

- Pedir valor exorbitante sem comparativo jurisprudencial → arbitrado a menor + sucumbência recíproca eventual.
- Mero aborrecimento (Súmula 388 STJ — desconsiderar atendimento ruim, demora razoável, fila bancária etc.).
- Súmula 385 STJ: se já havia negativação anterior subsistente, dano moral é afastado.
- Não juntar prova do prejuízo concreto (extrato de Serasa, comprovante de recusa de crédito).
- Esquecer Súm 54/362 nos juros e correção.
- PJ pleiteando dano moral por evento que não atinge sua imagem (Súm 227 STJ — PJ pode ter dano moral, mas o critério é restrito).

## Checklist

- [ ] Conduta ilícita do réu documentada
- [ ] Nexo causal claro
- [ ] Dano comprovado (não basta afirmar)
- [ ] Pedido na faixa jurisprudencial razoável
- [ ] Súmula 54/362 nos juros e correção
- [ ] Inversão de ônus (CDC) requerida
- [ ] Tutela de urgência (se cabível)
- [ ] Gratuidade requerida (se cabível)
- [ ] Documentos juntados
- [ ] Provas indicadas (testemunhas, perícia)

## Referências

- CC arts. 11-21, 186-188, 389-405, 927
- CDC (Lei 8.078/90) arts. 6º VIII, 12, 14, 17, 18, 20, 51 IV
- Súmulas STJ 54, 326, 362, 388, 385, 479
- Convenção de Montreal (transporte aéreo internacional)

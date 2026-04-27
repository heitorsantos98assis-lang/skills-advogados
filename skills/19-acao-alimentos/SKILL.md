---
name: acao-alimentos
description: Estrutura ação de alimentos (Lei 5.478/68 + CPC 693-699 + CC 1.694-1.710), com fixação provisória, definitiva, exoneração e revisão, ajustada ao binômio necessidade × possibilidade.
allowed-tools: Read Grep Bash Edit Write
user-invocable: true
---

## Quando usar

Pleitear pensão alimentícia para filhos menores, filhos universitários (Súm 358 STJ), cônjuge transitoriamente, idosos (CC 1.696), e dependentes em geral. Skill cobre fixação, revisão, exoneração e execução.

## Inputs necessários

1. Identificação do alimentando (filho menor, ex-cônjuge, idoso) e alimentante
2. Comprovação do parentesco/vínculo (certidão de nascimento, casamento)
3. Comprovação da necessidade (despesas: escola, saúde, alimentação, moradia, lazer)
4. Comprovação da possibilidade (CTPS, contracheques, IRPF do réu, padrão de vida, bens)
5. Padrão de vida anterior do beneficiário (se relevante)
6. Documentos de paternidade (se contestada — necessidade de DNA)
7. Procuração

## Modalidades

### 1. Provisórios (Lei 5.478/68 art. 4º)
- Concedidos liminarmente na inicial
- Sem necessidade de instrução completa
- Se o juiz entender presentes os pressupostos

### 2. Provisionais (acessórios à ação principal)
- Em ação de divórcio, investigação de paternidade, etc.
- Mantidos durante o processo

### 3. Definitivos
- Após instrução completa e sentença
- Substituem os provisórios/provisionais

### 4. Revisional (CPC 1.069 + CC 1.699)
- Quando há mudança da situação financeira do alimentante ou da necessidade do alimentando
- Pedido de minoração, majoração, exoneração

### 5. Exoneração (CC 1.708-1.709)
- Filho atingiu maioridade + autonomia financeira
- Necessária ação **com contraditório** (Súm 358 STJ — não exonera automaticamente em 18 ou 24 anos)

## Binômio CC 1.694 § 1º

```
Necessidade do alimentando × Possibilidade do alimentante = Quantum
```

### Necessidade
- Despesas reais demonstráveis: escola, saúde, alimentação, moradia, transporte, lazer, vestuário
- Padrão de vida anterior (se cônjuge: padrão era do casamento)
- Idade, saúde, estudos

### Possibilidade
- Renda comprovada (não só CTPS — incluir variáveis: PLR, comissões, pró-labore, autônomo, retiradas de empresa)
- Sinais externos de riqueza
- Patrimônio
- Outras dependências (outros filhos, pais)

## Cálculo e fixação

| Padrão | Quantum típico |
|---|---|
| 1 filho menor com mãe guardiã, pai assalariado | 25-30% rendimentos líquidos do pai |
| 2 filhos | 33-40% |
| 3 filhos | 40-50% |
| Cônjuge transitório (geralmente até reabilitação econômica) | 10-25% por prazo definido |
| Cliente autônomo / sem CTPS | Múltiplo do salário-mínimo (ex.: 2x SM) ou valor fixo |

**Atenção**: descontos sobre **rendimentos líquidos** (após INSS e IRRF) — Súm 358 STJ + CC 1.694 § 1º.

## Estrutura

```
EXMO. SR. JUIZ DA __ª VARA DA FAMÍLIA E SUCESSÕES DA COMARCA DE __________

[Filho menor representado pela mãe ___, ou direto, etc.]

vem propor

AÇÃO DE ALIMENTOS [com pedido de tutela de urgência]

em face de __________ [pai/responsável/devedor], pelos motivos a seguir.

I — DOS FATOS
1. O autor é filho do réu, conforme certidão de nascimento (doc. ___).
2. Atualmente com __ anos, frequenta a [escola] e tem despesas mensais de R$ __________ (planilha doc. ___).
3. O réu, profissional [...], aufere rendimentos mensais estimados em R$ __________ (CTPS doc. ___ ou indicadores doc. ___).
4. As tentativas extrajudiciais foram infrutíferas (doc. ___).

II — DO DIREITO
2.1. Do dever de prestar alimentos (CC 1.694 e seguintes; CF 229)
2.2. Do binômio necessidade × possibilidade
2.3. Da fixação provisória (Lei 5.478/68 art. 4º)
2.4. Da fixação por percentual sobre rendimentos líquidos (jurisprudência consolidada)

III — DA TUTELA DE URGÊNCIA
A urgência decorre da própria natureza alimentar — dependem de pronta intervenção. Requer:
   - Alimentos provisórios em R$ __________ ou __% dos rendimentos líquidos do alimentante, depositados até o dia __ de cada mês na conta __________

IV — DOS PEDIDOS
a) Concessão da tutela de urgência;
b) Citação do réu;
c) Ao final, procedência para fixar alimentos definitivos em R$ __________ ou __% dos rendimentos líquidos do alimentante, com as seguintes obrigações adicionais:
   - Plano de saúde (manter o filho como dependente)
   - Despesas extraordinárias (médicas, escolares de matrícula/uniforme): rateio __ %
   - Atualização anual pelo IPCA / INPC (vinculação salarial é alternativa);
d) Inversão do ônus quanto à comprovação de rendimentos (Súmula 277 e CC 1.694 § 2º — é dever do alimentante demonstrar);
e) Custas e honorários sucumbenciais;
f) Gratuidade (se cabível).

V — DO VALOR DA CAUSA
R$ __________ (12 prestações pretendidas — CPC 292 III)
```

## Detalhes processuais

### Audiência (CPC 695)
- Audiência de mediação obrigatória em ações de família.
- Possibilidade de acordo desde a primeira oportunidade.

### Citação
- Pessoal do alimentante (CPC 247).
- Pode ser por hora certa, edital se difícil.

### Prova
- Documental: contracheques, IRPF, escola, médico
- Pericial: investigação patrimonial, contábil
- Testemunhal

## Execução de alimentos (CPC 528-533)

### Rito da prisão (CPC 528 § 3º)
- 3 prestações **vencidas + as que vencerem** durante a execução
- Citação para pagar em 3 dias, justificar ou pagar
- Não pagamento: prisão civil de 1-3 meses (regime fechado, separado dos demais — Súmula 309 STJ)

### Rito da expropriação (CPC 528 § 8º + 824-825)
- Execução de prestações antigas (> 3 últimas)
- Penhora de bens, salário (até 50% — CPC 833 § 2º), bloqueio SISBAJUD

### Desconto em folha (CPC 529)
- Alimentos atuais: ofício direto ao empregador (50% rendimento líquido máx)

## Erros comuns

- Pedir 50% do bruto (correto: líquido).
- Não pedir provisórios → criança fica meses sem pensão.
- Esquecer despesas extraordinárias e plano de saúde.
- Vincular alimentos ao salário-mínimo direto sem indexação alternativa (CF veda em alguns casos — Súm 490 STJ aceita SM como referencial em alimentos).
- Maioridade automática → exoneração precisa de ação (Súm 358 STJ).
- Alimentos para idoso (CC 1.696) sem alegar incapacidade econômica.

## Checklist

- [ ] Vínculo provado (certidão nascimento, casamento)
- [ ] Necessidade documentada (planilha de despesas)
- [ ] Possibilidade demonstrada (rendimentos do réu)
- [ ] Provisórios pedidos
- [ ] Cláusulas adicionais (saúde, extraordinárias)
- [ ] Indexação anual
- [ ] Foro: domicílio do alimentando (CPC 53 II)
- [ ] Mediação (CPC 695) prevista
- [ ] Custas / gratuidade

## Referências

- CC arts. 1.694-1.710
- CF art. 229
- CPC arts. 528-533, 693-699
- Lei 5.478/1968 (Alimentos)
- ECA arts. 22, 24
- Súmulas STJ 309 (prisão civil), 358 (exoneração), 277 (CDC inverso), 384 (alimentos avoengos)
- Súmula 490 STJ (SM como indexador)

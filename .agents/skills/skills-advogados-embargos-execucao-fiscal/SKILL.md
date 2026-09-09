---
name: skills-advogados-embargos-execucao-fiscal
description: "Estrutura embargos à execução fiscal (Lei 6.830/80 art. 16) com penhora válida prévia, alegação de matérias defensivas, prescrição/decadência, excesso de execução e nulidades."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Codex, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Após a Fazenda Pública ajuizar **execução fiscal** (LEF — Lei 6.830/80) com inscrição em dívida ativa, e o devedor ser citado e ter bens penhorados ou seguro-garantia / fiança bancária. Prazo: **30 dias** da intimação da penhora (LEF art. 16).

## Pressupostos

1. Ação executiva fiscal em curso
2. **Garantia do juízo** (LEF art. 16):
   - Penhora válida (incluindo SISBAJUD bloqueio com indisponibilidade — atenção a posterior penhora formal)
   - Depósito integral
   - Fiança bancária
   - Seguro-garantia
3. Prazo de 30 dias (em dobro para Fazenda Pública)

## Inputs necessários

1. Cópia integral da execução fiscal (CDA, despacho citatório, AR/citação, auto de penhora)
2. Memória de cálculo do executado (se há excesso)
3. Provas das alegações defensivas
4. Procuração

## Estrutura

```
EXMO. SR. JUIZ DA __ª VARA DE EXECUÇÕES FISCAIS / FEDERAL DE __________

[Embargante — Devedor]

Processo de Execução Fiscal nº __________
Exequente: [União / Estado / Município]

Vem, com fulcro no art. 16 da Lei 6.830/80, opor

EMBARGOS À EXECUÇÃO FISCAL

I — DA TEMPESTIVIDADE
Penhora realizada em __/__/____ sobre [bem]. Intimação em __/__/____. 30 dias úteis. Termo final em __/__/____. Tempestivos.

II — DA GARANTIA DO JUÍZO
[Comprovar: penhora R$ ___ / depósito R$ ___ / fiança / seguro]

III — DAS MATÉRIAS DEFENSIVAS

3.1. Preliminares
   3.1.1. Prescrição (CTN 174) ou decadência (CTN 173)
   3.1.2. Nulidade da CDA (CTN 202; LEF art. 2º § 5º — requisitos formais)
   3.1.3. Inexistência ou ilegitimidade passiva
   3.1.4. Bem impenhorável
   3.1.5. Excesso de execução (CPC 917 III)

3.2. Mérito
   3.2.1. Pagamento, parcelamento, compensação, transação
   3.2.2. Decadência do lançamento
   3.2.3. Imunidade ou isenção
   3.2.4. Inconstitucionalidade do tributo
   3.2.5. Erros de cálculo (atualização, multa, juros)
   3.2.6. Recuperação de créditos (Tema 69 Aplicado, etc.)

IV — DOS PEDIDOS
a) Recebimento dos embargos com efeito suspensivo (CPC 919 § 1º + Súm 387 STJ — havendo garantia + relevância da fundamentação + risco);
b) Citação da Fazenda Pública para impugnação (LEF art. 17 — 30 dias);
c) Acolhimento das preliminares para extinção da execução;
d) No mérito, procedência para:
   d.1) Declarar prescrição/decadência
   d.2) Excluir multa abusiva
   d.3) Reconhecer pagamento/compensação
   d.4) Reduzir o quantum em razão de excesso
   d.5) Decretar nulidade da CDA
e) Custas e honorários sucumbenciais à Fazenda (CPC 85 § 3º — escala progressiva);
f) Liberação da garantia em caso de procedência total.

V — DAS PROVAS
- Documental
- Pericial contábil (cálculos)
- Testemunhal (em casos específicos)

VI — DO VALOR DA CAUSA: R$ __________ (proveito econômico — valor que pretende excluir)
```

## Matérias defensivas frequentes

### 1. Prescrição quinquenal (CTN 174)
- 5 anos da constituição definitiva para a Fazenda ajuizar execução
- Interrupções: citação válida (LEF art. 8º § 2º — interpretação STJ Tema 1.073: a CDA + despacho do juiz = interrupção)
- Tema 1.073 STJ: prescrição intercorrente (CTN 40) — ajuizada execução, não localizado devedor, prazo de 5 anos para pleitear extinção

### 2. Prescrição intercorrente (LEF art. 40)
- Suspensão por 1 ano + 5 anos = 6 anos sem movimentação útil → extingue (Tema 568 STJ)

### 3. Nulidade da CDA (CTN 202; LEF art. 2º § 5º)
Requisitos formais:
- Nome do devedor
- Quantia + data de inscrição
- Origem da dívida com fundamentação legal
- Termo inicial e modo de calcular juros e multa
- Número do processo administrativo
Falta = vício → nulidade total ou substituição (LEF art. 2º § 8º)

### 4. Excesso de execução
- Cálculo refeito na contadoria judicial
- Pagamento parcial não considerado
- Inclusão de tributo prescrito

### 5. Bem impenhorável (CPC 833)
- Salário (até teto), bem de família, ferramentas de trabalho, etc.

### 6. Pagamento, parcelamento, transação
- Comprovar com guias e adesões

## Efeito suspensivo (CPC 919)

Embargos não suspendem automaticamente. Para suspender:
- Garantia integral (penhora, depósito, fiança, seguro)
- Demonstrar relevância da fundamentação
- Risco de dano grave

## Citação Fazenda

- 30 dias para impugnação (LEF 17)
- Vista dos autos

## Honorários — escala progressiva CPC 85 § 3º (Fazenda)

Faixas reduzidas (10% para até 200 SM, decrescentes em valores maiores).

## Erros comuns

- Embargar sem garantia → não recebido (Súm 213 STJ).
- Não pedir efeito suspensivo + garantia.
- Esquecer prescrição intercorrente quando aplicável.
- Não impugnar especificamente a CDA quando há vício formal.
- Reapresentar matéria já decidida no contencioso administrativo (eficácia limitada).
- Não pleitear honorários da Fazenda (escala progressiva).
- Excesso sem perícia contábil — fragilidade na demonstração.

## Checklist

- [ ] Garantia do juízo (penhora/depósito/seguro/fiança)
- [ ] Prazo de 30 dias respeitado
- [ ] CDA analisada (vícios formais)
- [ ] Prescrição/decadência verificada
- [ ] Cálculo refeito (excesso)
- [ ] Pedido de efeito suspensivo
- [ ] Pericial requerida
- [ ] Honorários sucumbenciais com escala
- [ ] Procuração

## Referências

- Lei 6.830/1980 (LEF) arts. 1º-42
- CTN arts. 142, 173, 174, 202
- CPC arts. 833, 917, 919
- Súmulas STJ 112, 213, 314, 387, 409, 449, 496
- Tema 568 STJ (prescrição intercorrente)
- Tema 1.073 STJ

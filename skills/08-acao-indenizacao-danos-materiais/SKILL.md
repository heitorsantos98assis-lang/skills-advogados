---
name: acao-indenizacao-danos-materiais
description: Estrutura ação de indenização por danos materiais (emergentes + lucros cessantes), com prova do prejuízo, nexo causal, atualização e cumulação com danos morais quando cabível.
allowed-tools: Read Grep Bash Edit Write
user-invocable: true
---

## Quando usar

Quando há prejuízo patrimonial verificável: dano em veículo, gastos médicos, honorários de outro profissional contratado por culpa do réu, lucros não auferidos, despesas com locação de outro veículo, etc.

Pode ser cumulado com danos morais (Súmula 387 STJ).

## Componentes (CC 402)

### 1. Dano emergente (CC 402, parte 1)
Aquilo que efetivamente diminuiu o patrimônio:
- Reparo de veículo
- Despesas médicas
- Salário perdido durante afastamento (se atribuível ao evento)
- Gastos com locação substituta

### 2. Lucros cessantes (CC 402, parte 2)
Aquilo que **deixou de ganhar**:
- Lucro do faturamento durante paralisação
- Salário enquanto incapacitado

**Atenção**: lucros cessantes precisam ser **comprovados** — não basta alegar. Súmula 41/STJ: "no caso de transporte aéreo, em transporte de mercadoria, presumem-se os lucros cessantes" (exceção que confirma a regra).

## Inputs necessários

1. Cliente (qualificação)
2. Réu (qualificação)
3. Documentos: orçamentos, NFs de reparo, recibos médicos, declarações de empregador, IRPF, contratos
4. Comprovação do nexo causal (BO, perícia técnica, fotos, vídeos)
5. Cálculo do prejuízo (com método: 3 orçamentos / cálculo lucro mensal)
6. Período de afastamento ou indisponibilidade

## Exemplos típicos

### Acidente de trânsito
- Reparo do veículo (3 orçamentos)
- Diária de locadora ou Uber durante o reparo
- Despesas médicas
- Salário não pago se afastamento
- Lucros cessantes (motorista de aplicativo: comprovar média diária)

### Falha de serviço (entrega quebrada, instalação ruim)
- Custo do bem
- Despesas para nova contratação
- Lucros perdidos

### Cobrança indevida / debito a maior
- Repetição do indébito (CDC 42 § ún — em dobro se houver cobrança em má-fé)
- Tema 929 STJ: repetição em dobro pelo dobro do que foi cobrado a maior

## Cálculo

```
DANO EMERGENTE
  Item 1: R$ _________ (NF/recibo doc ___)
  Item 2: R$ _________
  ...
SUBTOTAL: R$ _________

LUCROS CESSANTES
  Cálculo: receita média mensal R$ ___ / 30 = R$ ___ por dia
  Período: ___ dias = R$ _________

CORREÇÃO (desde data de cada gasto): IPCA / INPC / tabela TJ
JUROS DE MORA: 1% a.m. (CC 406)
   - Extracontratual: desde o evento (Súm 54 STJ)
   - Contratual: desde a citação ou vencimento (se contratado)
TOTAL ATUALIZADO: R$ _________
```

## Estrutura

```
[Cabeçalho — Vara Cível competente — geralmente foro do domicílio do autor consumidor (CDC 101 I) ou foro do domicílio do réu (CPC 46)]

I — DOS FATOS
1. [O evento que gerou o dano — data, local, circunstâncias]
2. [A conduta do réu que causou]
3. [Os prejuízos materiais: cada item documentado]
4. [Tentativas de solução extrajudicial]

II — DO DIREITO
2.1. Da responsabilidade civil (CC 186, 187, 927 / CDC 12, 14)
2.2. Do nexo causal (provado por __________)
2.3. Do dano material (CC 402)
   2.3.1. Dano emergente
   2.3.2. Lucros cessantes

III — DA QUANTIFICAÇÃO
[Detalhamento do cálculo + indexação]

IV — DOS PEDIDOS
a) Citação do réu;
b) Procedência para:
   b.1) Condenação ao pagamento de R$ __________ a título de danos materiais (emergentes + cessantes), com correção monetária desde a data do efetivo prejuízo (cada gasto) e juros legais de 1% a.m. a partir do evento (Súm 54 STJ) ou da citação;
   b.2) Eventualmente, cumulação com danos morais no valor de R$ __________ (Súm 387 STJ);
c) Custas e honorários (CPC 85);
d) Inversão do ônus da prova (CDC 6º VIII), se aplicável;
e) Gratuidade (se aplicável);
f) Provas: documental, pericial (mecânica, contábil), testemunhal.

V — DO VALOR DA CAUSA
R$ __________ (soma do material + moral pretendidos)
```

## Cumulação com dano moral (Súm 387 STJ)

```
III — DA INDENIZAÇÃO MORAL CONCOMITANTE
Além do dano material, o autor sofreu abalo psíquico em razão de [descrever], a ensejar dano moral nos termos da Súmula 387 do STJ. Pleiteia-se o valor de R$ __________.
```

## Repetição do indébito (CDC 42 § ún)

Cobrança a maior em má-fé → repetição em dobro. Tema 929 STJ aplica em **má-fé presumida** quando cobrança decorre de erro injustificável em fatura de consumo.

```
b.3) A repetição em dobro do valor cobrado indevidamente, totalizando R$ __________ (CDC 42 § ún + Tema 929 STJ);
```

## Erros comuns

- Lucros cessantes alegados sem prova (precisa: contracheques, IRPF, faturamento mensal, contrato).
- Não atualizar cada gasto desde a data do desembolso → arbitragem judicial vai escolher um termo único, possivelmente desfavorável.
- Dano emergente sem nota fiscal → tribunal limita o valor.
- Cumular indevidamente material + moral pelo mesmo fato gerador único de cunho exclusivamente patrimonial.
- Não pedir produção pericial em dano material que requer perícia técnica (engenharia, mecânica, contábil).

## Checklist

- [ ] Cada item de dano emergente com NF/recibo
- [ ] Lucros cessantes com prova de receita habitual
- [ ] Nexo causal documentado (BO, perícia, foto)
- [ ] Cálculo atualizado (correção + juros)
- [ ] Eventual cumulação com dano moral fundamentada
- [ ] Inversão de ônus (CDC)
- [ ] Tutela urgente quando cabível (ex.: bloqueio do veículo do causador)
- [ ] Provas testemunhais/periciais indicadas
- [ ] Foro competente (CDC 101 I para consumidor)
- [ ] Custas pagas ou gratuidade

## Referências

- CC arts. 186, 187, 389, 402, 403, 404, 406, 927
- CDC arts. 6º VIII, 14, 17, 42 § ún, 101 I
- Súmulas STJ 41 (transporte aéreo), 54, 362, 387 (cumulação), Tema 929 (repetição)

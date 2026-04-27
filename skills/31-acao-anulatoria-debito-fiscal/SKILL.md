---
name: acao-anulatoria-debito-fiscal
description: Estrutura ação anulatória de débito fiscal (Lei 6.830/80 art. 38 + CTN) com depósito integral, prova, perícia, suspensão da exigibilidade e recurso ao tribunal.
allowed-tools: Read Grep Bash Edit Write
user-invocable: true
---

## Quando usar

Após **constituição definitiva do crédito** (auto de infração mantido em última instância administrativa OU prazo de defesa esgotado), para discutir o lançamento. Diferentemente do MS (skill 30), aqui há dilação probatória ampla.

Comum quando:
- Tese exige perícia contábil/técnica
- Já se passaram os 120 dias do MS
- Empresa não optou pela esfera administrativa

## Inputs necessários

1. Auto de infração / decisão administrativa final
2. Documentos do contribuinte (SPEDs, NFs, balancetes)
3. Análise técnica / parecer
4. Capacidade de depósito do crédito (para suspender exigibilidade) ou alternativas
5. Procuração

## Suspensão da exigibilidade — alternativas (CTN 151)

| Modalidade | Necessidade |
|---|---|
| Depósito integral em dinheiro | CTN 151 II — Súm 112 STJ |
| Liminar em MS | Lei 12.016 |
| Liminar em ação anulatória/cautelar | Súm 112 STJ — só com depósito |
| Parcelamento | Excludente em si |
| Reclamação/Recurso administrativo | Suspende durante administrativo |

Sem depósito, ação prossegue mas tributo permanece exigível, com cobrança em paralelo (execução fiscal).

## Estrutura

```
EXMO. SR. JUIZ FEDERAL / DA __ª VARA DE FAZENDA PÚBLICA DA COMARCA DE __________

[QUALIFICAÇÃO DO AUTOR — contribuinte]

vem propor

AÇÃO ANULATÓRIA DE DÉBITO FISCAL [com pedido de tutela de urgência]

em face de __________ [União / Estado / Município], pelas razões a seguir.

I — DOS FATOS
1. O autor é contribuinte do tributo __________, regime __________.
2. Em __/__/____ foi lavrado o Auto de Infração nº __________ no valor de R$ __________ (cópia anexa).
3. O autor apresentou impugnação administrativa que foi mantida pelo DRJ / TIT / TJM em __/__/____ (cópia anexa).
4. O crédito está constituído definitivamente, mas é manifestamente ilegal.

II — DO DEPÓSITO INTEGRAL [se for o caso]
2.1. Para suspender a exigibilidade (CTN 151 II + Súm 112 STJ), efetua-se o depósito integral do crédito atualizado, conforme guia anexa: R$ __________
2.2. [Alternativamente: pleitear liminar com base em outra modalidade]

III — DO DIREITO
3.1. [Tese principal — vício no lançamento, cobrança indevida, prescrição/decadência, inconstitucionalidade]
3.2. [Súmulas e jurisprudência consolidada]

IV — DOS PEDIDOS
a) Concessão de tutela de urgência para suspender a exigibilidade do crédito tributário (com base no depósito integral);
b) Citação da Fazenda Pública;
c) Procedência para anular o auto de infração nº __________ e a inscrição em dívida ativa eventualmente decorrente;
d) Restituição do depósito ao final, em caso de procedência;
e) Custas e honorários sucumbenciais (CPC 85);
f) Oficiar à PGFN/Procuradoria do Estado/Município para baixa do débito após trânsito.

V — DAS PROVAS
- Documental anexa
- Pericial contábil (CPC 369-484; necessária para __________)
- Eventualmente testemunhal

VI — DO VALOR DA CAUSA: R$ __________ (valor do auto)
```

## Teses comuns

### 1. Decadência (CTN 173)
- Auto após 5 anos do 1º dia do exercício seguinte ao fato gerador
- Lançamento por homologação (CTN 150 § 4º): 5 anos do fato gerador

### 2. Prescrição (CTN 174)
- Após constituição definitiva, 5 anos para ajuizar execução fiscal
- Suspensa por parcelamento, recurso administrativo, ações judiciais

### 3. Bitributação / cobrança em duplicidade

### 4. Erro de classificação (NCM, CFOP, Anexo do Simples)

### 5. Multa qualificada de 150% sem dolo demonstrado
- Reduzir para 75% (regular) ou 20% (homologação tácita)

### 6. Inconstitucionalidade de tributo / aplicação retroativa de lei

### 7. Crédito presumido glosado indevidamente

### 8. Imunidade ou isenção não reconhecida

## Cuidados

### Conexão com execução fiscal
Se já há execução fiscal (skill 32), embargos podem ser melhores. Se não há, anulatória previne.

### Prejudicialidade
Se o tema já é objeto de RE/REsp repetitivo, o tribunal pode sobrestar.

### Tutela de evidência (CPC 311)
Em casos de tese firmada em precedente vinculante, não precisa de depósito.

## Erros comuns

- Ajuizar sem depósito quando há urgência → cobrança paralela.
- Discutir matéria já preclusa em sede administrativa.
- Provar excesso de execução em ação principal (correto: nos embargos).
- Esquecer prescrição.
- Não pleitear restituição do depósito ao final.
- Pedir condenação em PJ que não é parte (devedor solidário sem regime).

## Checklist

- [ ] Auto / decisão administrativa final juntada
- [ ] Tese com fundamentação legal + jurisprudencial
- [ ] Estratégia de suspensão (depósito, liminar)
- [ ] Pericial requerida (se necessário)
- [ ] Decadência / prescrição alegadas se cabíveis
- [ ] Pedido principal e secundários
- [ ] Procuração e custas
- [ ] Foro competente (federal vs estadual)

## Referências

- Lei 6.830/1980 (LEF — Execução Fiscal)
- CTN arts. 142-150, 151, 156, 173-174
- CPC arts. 300-311 (tutela), 369-484 (provas)
- Súmulas STJ 112, 213; STF 70, 323
- Lei 12.016/2009 (MS — comparação)

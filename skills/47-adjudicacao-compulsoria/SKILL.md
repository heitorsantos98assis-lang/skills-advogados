---
name: adjudicacao-compulsoria
description: Estrutura ação de adjudicação compulsória (Lei 6.766/79 art. 16; CC 1.418) para promitente comprador receber escritura definitiva quando o vendedor recusa, com base em compromisso registrado.
allowed-tools: Read Grep Bash Edit Write
user-invocable: true
---

## Quando usar

Promitente comprador pagou integralmente o imóvel mas o vendedor (ou seu espólio, ou empresa em RJ) **recusa-se a outorgar a escritura definitiva**. A ação obriga o vendedor a fornecer a escritura, ou a sentença substitui sua manifestação de vontade.

## Inputs necessários

1. Promessa de compra e venda (com firma reconhecida)
2. Comprovação de quitação total do preço
3. Matrícula do imóvel
4. Notificação extrajudicial do vendedor exigindo a escritura
5. Procuração

## Requisitos (Lei 6.766/79 art. 16; CC 1.418)

1. Promessa de compra e venda devidamente firmada
2. Pagamento integral do preço
3. Recusa ou inadimplência do promitente vendedor em outorgar a escritura
4. Compromisso registrado (preferível, mas não obrigatório — Súm 239 STJ)

## Súmula 239 STJ

"O direito à adjudicação compulsória **não se condiciona ao registro** do compromisso de compra e venda."

— Mesmo sem registro, o promissário pode ajuizar a ação. Mas atenção: terceiros de boa-fé que adquirem do mesmo vendedor com registro prévio podem ter prioridade.

## Estrutura

```
EXMO. SR. JUIZ DA __ª VARA CÍVEL DA COMARCA DE __________

[PROMISSÁRIO COMPRADOR]

vem propor

AÇÃO DE ADJUDICAÇÃO COMPULSÓRIA

em face de [PROMITENTE VENDEDOR / espólio / sucessores], pelos motivos a seguir.

I — DOS FATOS
1. Em __/__/____ o autor celebrou com o réu PROMESSA DE COMPRA E VENDA do imóvel localizado em __________, matrícula __ do __º CRI (cópia anexa), pelo preço total de R$ __________
2. O autor pagou integralmente o preço:
   - Sinal: R$ __________ em __/__/____
   - Parcelas: 1ª __ R$ __ ... última __/__/____ (recibos anexos)
3. Não obstante a quitação, o réu se recusa a outorgar a escritura definitiva, apesar de notificado em __/__/____ (doc. ___).

II — DO DIREITO
2.1. Da promessa de compra e venda quitada
2.2. Da obrigação de fazer (outorgar escritura) — CC 1.418
2.3. Do direito à adjudicação (Lei 6.766 art. 16; CC 1.418; Súm 239 STJ)
2.4. Da execução específica (CPC 501 — sentença substitui declaração de vontade)

III — DOS PEDIDOS
a) Citação do(s) réu(s);
b) Procedência para:
   b.1) Determinar a outorga, pelo réu, de escritura definitiva de compra e venda do imóvel matrícula __, em prazo de 15 dias;
   b.2) Em caso de descumprimento, fazer as vezes da declaração de vontade do réu (CPC 501 — sentença adjudica diretamente, com força registral no CRI);
   b.3) Determinar a expedição de mandado para registro no CRI em nome do autor;
   b.4) Custas e honorários sucumbenciais;
c) Tutela de urgência (se houver risco de venda a terceiro): averbação na matrícula da existência da ação;
d) Intimação dos credores, se imóvel garante dívida.

IV — DO VALOR DA CAUSA
R$ __________ (valor do imóvel — ITBI / IPTU / valor venal)
```

## Pontos práticos

### Registro do compromisso
- Não obrigatório (Súm 239)
- Mas registro = oponibilidade erga omnes
- Sem registro: ação de fraude / oposição de terceiro de boa-fé pode complicar

### Notificação extrajudicial
- Obrigatória para constituir em mora (CC 397 § ún)
- Prazo razoável para outorgar (geralmente 30 dias)

### ITBI
- Devido pelo comprador (pode ser pago antes ou após sentença)
- Município pode exigir como condição para registro

### Imóvel financiado pelo SFH
- Promitente vendedor com financiamento ativo: necessária quitação ou sub-rogação
- Banco interessado no processo

### Imóvel em inventário (vendedor falecido)
- Espólio é sucessor — citar inventariante
- Adjudicação pode ser cumprida no inventário

### Promessa não registrada e venda a terceiro
- Pode caber rescisão da venda + indenização
- Tema mais complexo

## Tutela de urgência (CPC 300)

Quando há risco de venda a terceiro:

```
III.A — DA TUTELA DE URGÊNCIA
Há risco de o promitente vendedor alienar o imóvel a terceiro de boa-fé, frustrando o direito do autor. Pleiteia-se:
   a) Averbação da existência da presente ação na matrícula do imóvel (CPC 301 + Lei 6.015 art. 167 II 5)
   b) Indisponibilidade do imóvel
```

## Sentença e seus efeitos (CPC 501)

A sentença que julga procedente a adjudicação **produz os efeitos da declaração de vontade não emitida**. Substitui a escritura. Levada ao CRI: registro direto.

## Honorários e custas

- Sucumbência ao réu vencido (CPC 85)
- Custas: 1-2% conforme tabela TJ
- ITBI pago pelo autor (em geral)

## Erros comuns

- Promessa sem comprovação de quitação total — não cabe ainda.
- Réu erroneamente identificado (ex.: ainda em nome do espólio).
- Não pedir tutela de averbação → risco de venda a terceiro.
- Imóvel com hipoteca/penhora não comunicado.
- Foro errado (deve ser do imóvel — CPC 47).
- Esquecer pedido de adjudicação direta (CPC 501) — defesa subsidiária.

## Checklist

- [ ] Compromisso de compra e venda
- [ ] Comprovação de quitação total
- [ ] Notificação extrajudicial do vendedor
- [ ] Matrícula atualizada
- [ ] Pedido de tutela (averbação)
- [ ] Pedido de adjudicação compulsória
- [ ] CPC 501: sentença substitui vontade
- [ ] Custas / gratuidade
- [ ] Procuração

## Referências

- CC arts. 1.417-1.418, 397
- Lei 6.766/1979 art. 16, 23
- CPC arts. 47, 300, 501
- Lei 6.015/1973 art. 167 II
- Súmulas STJ 76 (recibos provam pagamento), 239 (registro)

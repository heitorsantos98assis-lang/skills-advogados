---
name: 15-recurso-ordinario-trt
description: "Estrutura recurso ordinário ao TRT contra sentença trabalhista, com tempestividade de 8 dias úteis, depósito recursal, custas, fundamentação articulada e contrarrazões."
allowed-tools: Read Grep Bash Edit Write
---

## Quando usar

Para impugnar **sentença** da Vara do Trabalho. Equivalente trabalhista da apelação cível. Prazo: **8 dias úteis** (CLT 6º Lei 5.584 + Lei 13.467 manteve em 8 dias após início do processo eletrônico).

## Inputs necessários

1. Sentença trabalhista (data de publicação/intimação)
2. Memória de cálculo da liquidação (se sentença líquida)
3. Depósito recursal — quando recorrer **empregador** (CLT 899 § 4º)
4. Custas processuais (CLT 789-A) — autor sucumbente paga; empregador sempre paga
5. Procuração e contrato de honorários

## Depósito recursal e custas

### Depósito recursal (CLT 899)
- Apenas para **recorrente empregador** (parte vencida com obrigação de pagar)
- Valor do depósito limitado ao valor da condenação
- Tetos atualizados anualmente pelo TST (em 2026, ~R$ 12.665 para RO; ~R$ 25.330 para RR — confirmar)
- Microempresa, empresa em RJ, beneficiária da gratuidade: dispensadas (Lei 13.467/17)
- Empregador insolvente: pode pedir gratuidade

### Custas (CLT 789)
- 2% sobre valor da condenação OU valor da causa, conforme o que se aplica
- Mínimo R$ 10,64 / máximo varia
- Reclamante vencido: paga (Lei 13.467 — mesmo com gratuidade pode haver custas a pagar com créditos do processo)
- Recurso sem custas → deserção (Súm 245 TST)

## Estrutura

```
EXMO. SR. JUIZ DA __ª VARA DO TRABALHO DE __________

Processo nº __________

Recorrente: __________
Recorrido: __________

__________ vem, com fulcro no art. 895 da CLT, interpor

RECURSO ORDINÁRIO

contra a r. sentença de fls. __, requerendo o processamento e a remessa ao TRT da __ª Região, conforme razões em anexo.

Depósito recursal: guia GFIP/FGTS Digital nº __________ R$ __________ (limite legal/limite condenação)
Custas: guia DARJ nº __________ R$ __________

[Local, data]
________________________
[Advogado] OAB/__ ______

==========================================================
RAZÕES DE RECURSO ORDINÁRIO

EGRÉGIO TRT — __ª REGIÃO

I — TEMPESTIVIDADE
Sentença publicada em __/__/____. Intimação em __/__/____. 8 dias úteis. Termo final: __/__/____. Tempestivo.

II — DA ADMISSIBILIDADE
[Confirmar depósito + custas. Se gratuidade, fundamentar.]

III — DOS FATOS
[Resumo do processo até a sentença]

IV — DAS RAZÕES PARA REFORMA

4.1. Da preliminar de [se houver]: nulidade por cerceamento, julgamento extra petita, etc.

4.2. Quanto ao mérito (item a item da sentença a reformar):
   4.2.1. Quanto às horas extras: [argumento]
       - Sentença concluiu __ porque __
       - Equivocadamente, pois __ (citar lei, súmula, jurisprudência)
       - Pleiteia-se a reforma para __
   4.2.2. Quanto ao adicional de insalubridade: [...]
   4.2.3. Quanto ao dano moral: [...]
   4.2.4. Quanto à equiparação salarial: [...]
   4.2.5. Quanto aos honorários sucumbenciais: [...]

4.3. Da quantificação / liquidação
[Discutir cálculos, índices, fórmula]

V — DOS PEDIDOS
Diante do exposto, requer:
a) O recebimento e processamento do presente recurso, com efeito apenas devolutivo (CLT 899);
b) O conhecimento e provimento, para reformar a sentença e [pedido específico];
c) Subsidiariamente, a redução / minoração da condenação;
d) Honorários sucumbenciais à parte adversa (CLT 791-A);
e) Efeito suspensivo, se cabível.

[Local, data]
________________________
[Advogado] OAB/__ ______
```

## Princípios trabalhistas no recurso

### Princípio da delimitação recursal
Cada matéria reformada deve ser **especificamente** atacada. Súmula 422 TST: razões devem combater os fundamentos da decisão recorrida.

### Princípio do non reformatio in pejus
Recorrente não pode ter sua situação piorada (salvo em recurso da parte adversa).

### Efeito devolutivo trabalhista (Súmula 393 TST)
Devolve toda a matéria impugnada e seus consectários (DSR, juros, correção, FGTS).

## Honorários sucumbenciais (CLT 791-A)

- 5-15% sobre valor liquidado da sentença
- Sucumbência recíproca: cada parte responde pelos honorários da outra
- Beneficiário da gratuidade: paga com créditos havidos no próprio processo OU em outro (Lei 13.467/17 — STF declarou parcialmente inconstitucional na ADI 5.766: a parte beneficiária só paga se houver capacidade)

## Erros comuns

- Não impugnar todos os fundamentos da sentença — Súmula 422 TST.
- Esquecer depósito recursal → deserção (Súm 245 TST).
- Custas atrasadas → deserção.
- Recurso copiado da defesa, sem confronto com a sentença.
- Microempresa sem comprovação do enquadramento → não isenta de depósito.
- Empresa em RJ sem documento → não isenta.
- Ofensa à coisa julgada parcial (não recorrer de itens torna-os imutáveis para o recorrente).

## Checklist

- [ ] 8 dias úteis confirmado e respeitado
- [ ] Depósito recursal (empregador) ou gratuidade
- [ ] Custas pagas
- [ ] Razões impugnam cada item da sentença
- [ ] Fundamentação legal + jurisprudencial (TST)
- [ ] Efeito suspensivo requerido se cabível (CLT 899)
- [ ] Honorários recursais
- [ ] Procuração ativa
- [ ] Protocolo OK no PJe-JT

## Referências

- CLT arts. 893-902, 789, 791-A, 899
- Lei 13.467/2017
- Súmulas TST 245, 422, 393
- ADI 5.766 STF (gratuidade trabalhista)
- Resoluções CSJT (gratuidade, formato eletrônico)

---
name: skills-advogados-falencia-pedido
description: "Estrutura pedido de falência por credor (Lei 11.101 art. 94 — impontualidade, execução frustrada, atos de falência), defesa do devedor e auto-falência (art. 105)."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Claude, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

### Pelo credor (Lei 11.101 art. 94)
1. **Impontualidade**: dívida líquida > 40 SM, vencida e não paga, comprovada por título(s) executivo(s)
2. **Execução frustrada**: empresa executada não paga, não deposita e não nomeia bens à penhora em 3 dias da citação
3. **Atos de falência**: prática de atos previstos no art. 94 III (procede ao patrimônio sem causa, abandona o estabelecimento, simula transferência etc.)

### Pelo próprio devedor (autofalência — art. 105)
- Quando reconhecer impossibilidade de continuar
- Pode ser estratégica em algumas hipóteses

## Inputs necessários (pedido por credor)

1. Título executivo (cheque, NP, contrato com 2 testemunhas, sentença) ou conjunto
2. Valor da dívida > 40 SM
3. Comprovação da impontualidade (protesto especial para fins de falência — art. 94 § 3º)
4. Identificação do devedor

## Estrutura — pedido de falência por credor

```
EXMO. SR. JUIZ DA __ª VARA DE FALÊNCIAS E RECUPERAÇÕES JUDICIAIS DA COMARCA DE __________

[CREDOR — qualificação completa]

vem propor

PEDIDO DE FALÊNCIA

em face de __________ [devedor — empresa], com fundamento no art. 94, I, II ou III da Lei 11.101/2005, pelos motivos a seguir.

I — DOS REQUISITOS

1.1. Tradicionalidade: o credor é titular de [título executivo] no valor de R$ __________ (acima de 40 SM = R$ __________ atualizado).

1.2. Impontualidade: vencimento em __/__/____. Não pago. Protesto especial para fins falimentares anexo (art. 94 § 3º).

1.3. [Demais hipóteses se cabíveis]

II — DOS FATOS
[Síntese da relação comercial e da inadimplência]

III — DO DIREITO
3.1. Lei 11.101/2005, art. 94 I (ou II / III)
3.2. Exigência do protesto especial (art. 94 § 3º)
3.3. Súmula 248 STJ: comprovação documental da insolvência

IV — DOS PEDIDOS
a) Citação do devedor no prazo legal de 10 dias para depositar a quantia, contestar ou apresentar pedido de recuperação judicial (art. 95-98);
b) Caso não cumprido, decreto de falência;
c) Nomeação de administrador judicial;
d) Determinações inerentes ao processo falimentar (arrecadação, lacre, suspensão de protestos, comunicações).

V — DO VALOR DA CAUSA: R$ __________ (valor do crédito)
```

## Defesa do devedor — depósito elisivo (art. 98 § ún)

Em 10 dias da citação, o devedor pode:

### a) Depositar a quantia (depósito elisivo)
- Suspende o processo
- Discute em embargos / contestação
- Não há decreto de falência

### b) Contestar a falência
- Negar requisitos
- Alegar legitimidade, prescrição, pagamento

### c) Apresentar pedido de recuperação judicial
- Se cumprir requisitos do art. 48
- Suspende o pedido de falência

## Decreto de falência — efeitos

- Declaração: art. 99 da Lei
- Lacre dos estabelecimentos
- Suspensão das obrigações do devedor
- Exigência de habilitação de créditos pelos credores (15 dias do edital)
- Administrador judicial assume
- Dirigentes podem ser afastados

## Massa falida

- Bens arrecadados constituem a massa
- Realização do ativo (venda de bens)
- Pagamento conforme ordem (Lei 11.101 art. 83):
  1. Trabalhistas até 150 SM por credor (excedente quirografário)
  2. Garantia real até o valor do bem gravado
  3. Tributários (não as multas)
  4. Privilégio especial
  5. Privilégio geral
  6. Quirografários
  7. Multas
  8. Subordinados

## Atos atentatórios (Lei 11.101 art. 129-131) — ineficácia

Atos do devedor nos 90 dias anteriores ao decreto (termo legal):
- Pagamento de dívidas não vencidas
- Pagamento por meios não usuais
- Doações
- Contratos onerosos

## Falência fraudulenta — crimes (Lei 11.101 art. 168 ss)

- Fraude a credores
- Crime de natureza falimentar
- Pena de 3 a 6 anos + multa

## Estrutura — autofalência (art. 105)

```
[CABEÇALHO — Vara de Falências]

[EMPRESA — qualificação] vem requerer

AUTOFALÊNCIA

com fundamento no art. 105 da Lei 11.101/2005.

I — DA SITUAÇÃO
1. A empresa não consegue cumprir suas obrigações pecuniárias.
2. Não há viabilidade de recuperação.
3. Patrimônio insuficiente para atender aos credores.

II — DOS DOCUMENTOS (art. 105)
   I. Demonstrações contábeis
   II. Relação nominal de credores
   III. Relação de bens
   IV. Relação de ações em curso
   V. Quadro societário

III — DOS PEDIDOS
a) Decretação da falência;
b) Nomeação de administrador judicial;
c) Atos de arrecadação e lacre;
d) Demais providências de praxe.
```

## Erros comuns

- Pedir falência sem protesto especial (art. 94 § 3º) — exigência formal.
- Crédito abaixo de 40 SM — não cabe pedido isolado.
- Cumular pedidos em desacordo com o procedimento.
- Esquecer prazo de 10 dias para depósito elisivo.
- Cliente devedor: deixar passar prazo para apresentar RJ (estratégia comum).
- Não pleitear nomeação de administrador na inicial.

## Checklist

- [ ] Crédito > 40 SM
- [ ] Protesto especial (art. 94 § 3º)
- [ ] Título executivo
- [ ] Citação para depósito ou defesa em 10 dias
- [ ] Pedido de nomeação de administrador
- [ ] Procuração com poderes específicos
- [ ] Custas

## Referências

- Lei 11.101/2005, especialmente arts. 94-105, 129-131, 168
- Lei 14.112/2020 (alterações)
- Súmula 248 STJ
- Tema STJ sobre protesto especial

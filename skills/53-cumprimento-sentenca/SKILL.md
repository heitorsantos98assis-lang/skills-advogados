---
name: cumprimento-sentenca
description: Estrutura cumprimento de sentença (CPC 513-538) com intimação para pagamento, multa de 10%, honorários de 10%, penhora SISBAJUD/RENAJUD/INFOJUD, expropriação e cumprimento de obrigação de fazer.
allowed-tools: Read Grep Bash Edit Write
user-invocable: true
---

## Quando usar

Após sentença transitada em julgado (ou liquidada), credor inicia a fase de cumprimento. Substitui a antiga "execução de título judicial". Aplica-se a:
- Pagar quantia (CPC 523-527)
- Obrigação de fazer/não fazer (CPC 536-537)
- Entregar coisa (CPC 538)
- Alimentos (CPC 528-533) — skill 19

## Inputs necessários

1. Sentença transitada em julgado
2. Memória de cálculo atualizada (quando há quantificação)
3. Endereços e dados do executado (para citação)
4. Procuração

## Cálculo (cumprimento de obrigação de pagar)

```
Principal (sentença)................ R$ __________
+ Correção monetária (TR/IPCA/Selic) R$ __________
+ Juros (1% a.m. ou Selic conforme) R$ __________
+ Honorários sucumbenciais (sentença) R$ __________
= Total atualizado.................. R$ __________

(Pós CPC 523:
+ Multa de 10% se não pagar em 15 dias
+ Honorários de 10% no cumprimento)
```

## Estrutura — petição inicial de cumprimento (CPC 524-525)

```
EXMO. SR. JUIZ DA __ª VARA __ DA COMARCA DE __________

Processo originário nº __________

[CREDOR — exequente]

vem requerer

CUMPRIMENTO DE SENTENÇA

I — DOS FATOS
1. A sentença transitou em julgado em __/__/____ (cópia + certidão de trânsito anexa).
2. A obrigação consiste em [pagar R$ __________ / fazer __ / entregar __].
3. Memória de cálculo atualizada (anexa).

II — DA OBRIGAÇÃO E DO DEVEDOR
2.1. Devedor: __________ CPF/CNPJ __________
2.2. Endereço atual: __________
2.3. Valor atualizado: R$ __________

III — DOS PEDIDOS
a) Intimação do executado para pagar em 15 dias (CPC 523), sob pena de:
   - Multa de 10% sobre o saldo (CPC 523 § 1º)
   - Honorários de 10% no cumprimento (CPC 523 § 1º — STJ EAREsp 1.229.797)
b) Não pago, o prosseguimento com:
   - Penhora online via SISBAJUD
   - Bloqueio de veículos via RENAJUD
   - Consulta INFOJUD (Receita) para imóveis e patrimônio
   - Penhora de outros bens
c) Eventuais protestos da sentença (Lei 9.492/97 art. 1º + § 5º)
d) Negativação no SPC/Serasa
e) Custas e honorários do cumprimento

IV — DOS DOCUMENTOS
1. Sentença + acórdão (se houver) + certidão de trânsito
2. Memória de cálculo
3. Procuração

[Local, data]
[Advogado] OAB
```

## Atos de constrição

### SISBAJUD (Sistema de Busca de Ativos do Judiciário)
- Bloqueio em todos os bancos do executado
- Resposta em ~3 dias
- Limite: salário (CPC 833 IV — protege salário até teto, com exceções)

### RENAJUD
- Bloqueio de veículos
- Restringe transferência

### INFOJUD
- Acesso à RFB para identificar bens, IRPF, declarações
- Restrito (necessário fundamentar)

### CCS-BACEN (Cadastro de Clientes do Sistema Financeiro)
- Identifica relações bancárias

### CNIB (Central Nacional de Indisponibilidade)
- Indisponibilidade de imóveis em todos os cartórios do país

## Penhora e expropriação

1. Penhora dos bens
2. Avaliação
3. Manifestação do executado
4. Adjudicação (CPC 876) — credor toma para si
5. Alienação por iniciativa particular (CPC 880)
6. Leilão eletrônico (CPC 881-903)

## Impugnação ao cumprimento (CPC 525)

Executado tem 15 dias após o pagamento (ou penhora — discussão) para opor:
- Falta ou nulidade de citação no processo originário
- Ilegitimidade de parte
- Inexigibilidade ou inexequibilidade do título
- Penhora incorreta ou avaliação errônea
- Excesso de execução / cumulação indevida
- Incompetência absoluta ou relativa
- Qualquer causa modificativa ou extintiva da obrigação posterior à sentença
- Defesa específica (skill 54)

## Cumprimento de obrigação de fazer/não fazer (CPC 536-537)

```
Pedido:
a) Intimação do executado para cumprir em prazo razoável
b) Astreinte de R$ __________ por dia de descumprimento (proporcional ao valor da obrigação)
c) Em caso de impossibilidade material, conversão em perdas e danos
```

CPC 537: o juiz pode modificar a multa diária se exorbitante (Súm 410 STJ — astreinte sem prejuízo de outras medidas).

## Cumprimento de entregar coisa (CPC 538)

```
Pedido: mandado de busca e apreensão / imissão na posse, conforme natureza
```

## Erros comuns

- Pedir cumprimento sem trânsito em julgado.
- Cálculo desatualizado → executado paga e o credor descobre que falta valor.
- Não pedir SISBAJUD na primeira oportunidade — executado movimenta dinheiro.
- Esquecer multa de 10% e honorários (CPC 523 § 1º).
- Astreinte abusiva (proporcional ao valor da obrigação).
- Penhorar bem impenhorável (CPC 833) — discussão posterior.

## Checklist

- [ ] Sentença + trânsito em julgado
- [ ] Memória de cálculo atualizada
- [ ] Pedido de intimação CPC 523
- [ ] Multa 10% + honorários 10%
- [ ] SISBAJUD / RENAJUD / INFOJUD
- [ ] Astreinte (obrigação de fazer)
- [ ] Custas (em geral suportadas pelo executado)
- [ ] Procuração

## Referências

- CPC arts. 513-538
- Lei 9.492/1997 (Protesto de Títulos)
- Súmulas STJ 410, 519
- Tema 547 STJ (cumprimento e penhora)
- Resolução CNJ 314/2020 (CNIB)

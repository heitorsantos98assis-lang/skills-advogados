---
name: 40-acao-consumidor-procon
description: "Conduz reclamação no Procon e ação no Juizado Especial Cível (Lei 9.099/95) ou rito comum, com inversão do ônus da prova, valor da condenação e cumprimento."
allowed-tools: Read Grep Bash Edit Write
---

## Quando usar

Consumidor lesado em relação de consumo (CDC art. 2º + 3º). Estratégia escalonada:

1. **Reclamação interna** (SAC, ouvidoria) — Decreto 11.034/2022 obriga prazo de resposta
2. **Procon municipal/estadual ou consumidor.gov.br** — administrativa
3. **Juizado Especial Cível** (Lei 9.099/95) — até 40 SM, sem advogado obrigatório nas primeiras 20 SM
4. **Rito comum cível** — quando valor superior ou complexidade exige

## Inputs necessários

1. Identificação do consumidor (PF — Súm 297 STJ aplica CDC a bancos; Súm 363 admite PJ consumidora em condições)
2. Identificação do fornecedor (CNPJ, endereço, ramo)
3. Documentos da relação de consumo (NFs, contratos, prints, e-mails)
4. Histórico de tentativas de solução
5. Valor pretendido (com base jurisprudencial — skill 07)

## Reclamação no consumidor.gov.br

Plataforma da SENACON para mediação digital:
- Cadastro do consumidor
- Reclamação descritiva com docs
- Empresa cadastrada responde em 10 dias
- Não substitui Procon nem JEC, mas é rápido e gratuito

## Reclamação no Procon

- Procon municipal ou estadual
- Prazo da empresa para resposta: 10 dias úteis
- Audiência conciliatória eventual
- Multa administrativa (não substitui indenização ao consumidor)

## Estrutura — petição inicial JEC

```
EXMO. SR. JUIZ DO __ JUIZADO ESPECIAL CÍVEL DA COMARCA DE __________

[CONSUMIDOR] (qualificação) vem propor

AÇÃO DE INDENIZAÇÃO POR DANOS [MATERIAIS / MORAIS] C/ [PEDIDO DE TUTELA]

em face de [FORNECEDOR] (CNPJ, endereço completo)

I — DOS FATOS
1. Em __/__/____ o autor adquiriu da ré [produto/serviço] pelo valor de R$ __________ (cupom/contrato anexo).
2. [Defeito / vício / falha].
3. [Tentativas de solução: SAC nº __, Procon nº __, e-mails].
4. A ré [não respondeu / negou / propôs quantia insuficiente].

II — DO DIREITO
2.1. Da relação de consumo (CDC arts. 2º e 3º)
2.2. Da responsabilidade objetiva (CDC 12, 14)
2.3. Da inversão do ônus da prova (CDC 6º VIII)
2.4. Dos danos morais [se houver]
2.5. Da repetição em dobro [se cobrança a maior — CDC 42 § ún]

III — DOS PEDIDOS
a) Citação da ré;
b) Inversão do ônus da prova;
c) Procedência para:
   c.1) Restituição em dobro de R$ __________ (CDC 42 § ún)
   c.2) Indenização por danos materiais de R$ __________
   c.3) Indenização por danos morais de R$ __________
   c.4) Obrigação de fazer: __________ (ex.: cancelar negativação, retirar do SPC, executar serviço, devolver bem)
   c.5) Astreinte (multa diária) em caso de descumprimento
d) Tutela de urgência: [retirada do SPC / abstenção de cobrança] em 5 dias sob pena de multa diária
e) Gratuidade de justiça (se cabível)
f) Custas suportadas pela ré em caso de procedência

IV — VALOR DA CAUSA: R$ __________ (até 40 SM no JEC)

V — DOCUMENTOS
1. Cupom/contrato
2. Comprovante de pagamento
3. Tentativas de solução
4. Print SPC/Serasa (se houver negativação)
5. Comprovação do dano

[Local, data]
[Nome] — sem assinatura de advogado se até 20 SM
```

## Princípios CDC fundamentais

### Vulnerabilidade (CDC 4º I)
Consumidor reconhecido como vulnerável.

### Boa-fé objetiva (CDC 4º III)
Lealdade nas relações.

### Inversão do ônus da prova (CDC 6º VIII)
Quando hipossuficiência ou verossimilhança.

### Responsabilidade objetiva (CDC 12, 14)
Independente de culpa.

### Solidariedade (CDC 7º § ún, 25 § 1º)
Toda a cadeia (fabricante, distribuidor, comerciante) responde.

## Tipos comuns

### 1. Negativação indevida
- Skill 07 — danos morais
- Tutela: retirar SPC/Serasa imediatamente

### 2. Cobrança indevida
- CDC 42 § ún: repetição em dobro (jurisprudência: comprovação de má-fé não é exigida — Tema 929 STJ)

### 3. Defeito / vício de produto
- Skill 42

### 4. Falha de serviço (banco, plano, telefonia)
- Responsabilidade objetiva CDC 14

### 5. Atraso / cancelamento de voo
- Convenção de Montreal (internacional) — limita material
- Resolução ANAC 400/2016 — direitos
- STJ Tema 1.103: dano moral por atraso > 4h em hipóteses específicas

### 6. Plano de saúde
- Recusa de cobertura
- Aumento abusivo
- Súm 302 STJ — cláusula limitativa de tempo de internação é abusiva

### 7. E-commerce
- Direito de arrependimento (CDC 49 — 7 dias)
- Entrega em desacordo / não entrega

## JEC — Lei 9.099/95

- Até 40 SM
- Sem advogado até 20 SM
- Audiência de conciliação obrigatória
- Sentença em 30 dias após audiência
- Recurso para Turma Recursal (não TJ)
- Custas isenta na 1ª instância para o autor; recursal: 1% sobre o valor da causa

## Erros comuns

- Pleitear danos morais por mero aborrecimento (Súm 388 STJ).
- Não juntar prova da relação de consumo.
- Esquecer pedido de inversão do ônus.
- Negativação anterior subsistente afasta dano moral (Súm 385 STJ) — verificar antes.
- Pedido de restituição em dobro sem fundamentar má-fé / Tema 929.
- Acionar duas vezes (Procon + JEC) sem litispendência — pode ser problema processual.
- Foro: domicílio do autor (CDC 101 I) — fórmula de proteção.

## Checklist

- [ ] Documentos da relação de consumo
- [ ] Tentativas extrajudiciais documentadas
- [ ] Pedido específico (restituição, indenização, obrigação de fazer)
- [ ] Tutela de urgência se cabível
- [ ] Inversão do ônus
- [ ] Astreinte
- [ ] Foro do domicílio do consumidor
- [ ] Valor da causa adequado ao JEC ou ordinário

## Referências

- Lei 8.078/1990 (CDC)
- Lei 9.099/1995 (JEC)
- Decreto 11.034/2022 (SAC)
- Resolução ANAC 400/2016
- Convenção de Montreal (Decreto 5.910/06)
- Súmulas STJ 297, 363, 385, 388, 302; STF 297
- Tema 929 STJ (repetição em dobro)
- Tema 1.103 STJ (atraso voo)

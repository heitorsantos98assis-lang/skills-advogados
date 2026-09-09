---
name: skills-advogados-calculo-horas-extras
description: "Calcula horas extras (50%, 100%, intervalo intra-jornada, sobreaviso) com reflexos em DSR, 13º, férias e FGTS, considerando banco de horas, regime 12x36 e jornada parcial."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Codex, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Para fundamentar pedido em reclamação trabalhista, quantificar passivo do empregador, ou auditoria de folha. Skill espelho da contadora 27 (folha) e 11 (reclamação).

## Inputs necessários

1. Salário base do mês de referência
2. Jornada contratual (40h, 44h, 36h, 12x36)
3. Cartão de ponto OU registro alternativo (testemunhas, e-mails)
4. CCT/ACT vigente (define adicional, intervalos, sobreaviso)
5. Regime: jornada padrão, banco de horas, compensação semanal, 12x36
6. Período de cálculo (mês, ano, ou todo o contrato com prescrição quinquenal)

## Conceitos-chave

### Hora normal (CLT 64)
```
Hora normal = Salário mensal / 220 (jornada 44h/sem)
```

| Jornada semanal | Divisor |
|---|---|
| 44h (8h × 5,5d ou 8h × 5d + 4h sáb) | 220 |
| 40h | 200 |
| 36h | 180 |
| 30h (parcial) | 150 |
| 25h (parcial) | 125 |
| 12h × 36h | Considera cada plantão; geralmente equivalente a 36h/sem efetivas |

### Adicional de HE
- Mínimo CF: 50% (CF 7º XVI)
- CCT pode estabelecer maior (60%, 100%)
- Domingos e feriados sem folga compensatória: 100% (CCT pode confirmar)
- Plantões noturnos: + adicional noturno (CLT 73)

## Cálculo passo a passo

### 1. Identificar HE do dia
```
Jornada efetiva (cartão) − Jornada contratual = HE do dia
```

### 2. Soma mensal por adicional
```
HE 50% = soma de horas extras de dias úteis × valor hora × 1,5
HE 100% = horas extras de domingo/feriado × valor hora × 2
```

### 3. Reflexos (Súmula 60, 172 TST e Lei 605/49)

```
Reflexo em DSR (sobre HE habituais):
  = (HE × dias úteis no mês) / dias úteis × dias DSR no mês

Reflexo em 13º:
  HE habituais somam à média do 13º

Reflexo em férias + 1/3:
  Idem na média de férias

Reflexo em FGTS:
  HE × 8% mensal

Reflexo em INSS / IRRF:
  Base ampliada
```

### 4. Intervalo intra-jornada não fruído (CLT 71 § 4º)

- Empregado que trabalha > 6h tem direito a 1h de intervalo (mín).
- Não usufruído: paga a hora **integral com adicional 50%** apenas pelo período suprimido (Lei 13.467/17 alterou — antes era a hora inteira).
- Reflexos: TST tem julgado que a parcela é indenizatória (não reflete em outras verbas) após reforma 2017. Tema controverso — verificar jurisprudência atualizada.

### 5. Sobreaviso (CLT 244 § 2º)

- Empregado fora do trabalho mas em "regime de plantão" (hoje: celular ligado, à disposição).
- Adicional de **1/3 da hora normal** por hora de sobreaviso.
- Súmula 428 TST: tempo à disposição ≠ uso ocasional do celular.

### 6. Hora reduzida noturna (CLT 73 § 1º)

- Jornada 22h-5h: 52'30" = 1 hora.
- Adicional noturno mín 20% sobre hora normal.

### 7. Banco de horas e compensação

- Compensação semanal: HE compensadas dentro da semana → não devidas (Súm 85 TST com cuidado).
- Banco de horas: compensa em até 6 meses (Lei 13.467/17 — pode ser por acordo individual; antes era só por CCT).
- Banco vencido sem compensação → todas as horas viram HE.

## Exemplo

Empregado com salário R$ 4.400, jornada 44h, fez 30 HE 50% e 8 HE 100% no mês.

```
Hora normal = 4.400 / 220 = R$ 20
HE 50% = 30 × 20 × 1,5 = R$ 900
HE 100% = 8 × 20 × 2 = R$ 320
TOTAL HE = R$ 1.220

DSR (Lei 605, ~5 domingos no mês = ~22% do mês):
DSR HE = 1.220 / 23 (dias úteis) × 5 (domingos) = R$ 265,22

Reflexos no mês:
  Em 13º (1/12 da soma anual): registrado para o final do ano
  Em férias (1/12): registrado
  FGTS 8% × (HE + DSR HE) = 8% × 1.485 = R$ 118,80

Encargos do empregador:
  INSS 20% + RAT × FAP + Terceiros sobre HE + reflexos
```

## Templates

### Planilha mensal de HE

```
EMPREGADO ____________ Mês __/____
Salário R$ ____ Jornada ___h/sem Hora normal R$ ____

Dia | Entrada | Saída | Total | Jornada contratual | HE 50% | HE 100%
___ | ___:__  | ___:__| ___h  | ___h               | ___h   | ___h
...
TOTAL HE 50%: ___h
TOTAL HE 100%: ___h

CÁLCULO:
HE 50% = ___ × ____ × 1,5 = R$ ________
HE 100% = ___ × ____ × 2 = R$ ________
DSR HE = R$ ________
TOTAL: R$ ________

Reflexos:
  13º (a apurar) | Férias (a apurar) | FGTS R$ ________
```

### Memória para reclamação

```
ITEM 1 — HORAS EXTRAS
Período: __/__/____ a __/__/____ (com prescrição quinquenal)
Cartão de ponto: doc ___ (ou Súmula 338 TST: invertido o ônus à empresa)

Mês | Salário | HE 50% | HE 100% | DSR HE | Reflexos 13º | Reflexos férias+1/3 | FGTS | TOTAL
____|________|________|_________|________|______________|____________________|______|______
...
TOTAL RECLAMADO: R$ ________

(Atualizado pela Selic / TR a partir de cada vencimento, conforme jurisprudência)
```

## Erros comuns

- Esquecer DSR sobre HE habituais (Súm 172 TST) → empregador / empregado perde valor.
- Aplicar adicional 50% sem CCT mais favorável (alguns CCT preveem 60-100%).
- Considerar todos os intervalos no banco de horas — controlar período de 6 meses (Lei 13.467).
- Tratar sobreaviso como hora normal — adicional é só 1/3 (CLT 244 § 2º).
- Calcular HE noturna sem hora reduzida (52'30" = 1h) → empregado paga a menos.
- Empregado externo (CLT 62 II) sem prova de controle de jornada → não tem direito a HE; mas a tese cai se houver controle (apps, GPS).
- Periculosidade/insalubridade na base da HE: incluir, conforme Súmula 60 e 264 TST.

## Checklist

- [ ] Salário base + adicionais habituais somados na hora normal
- [ ] Jornada contratual conferida (CTPS, contrato)
- [ ] Cartão de ponto ou prova alternativa (Súm 338 TST)
- [ ] HE 50% e 100% segregadas
- [ ] DSR sobre HE
- [ ] Reflexos em 13º, férias, FGTS
- [ ] Intervalo intra-jornada (Lei 13.467 redução)
- [ ] Sobreaviso (1/3)
- [ ] Hora noturna reduzida (52'30")
- [ ] Banco de horas validado (acordo + 6 meses)
- [ ] Atualização Selic / TR

## Referências

- CLT arts. 4º, 58, 59, 59-A, 62, 64, 66, 71, 73, 74, 244 § 2º
- CF 7º XIII, XIV, XVI
- Lei 605/1949 (DSR)
- Lei 13.467/2017
- Súmulas TST 60, 85, 172, 264, 338, 366, 428, 437
- Tema 1.046 STF (negociado sobre legislado)

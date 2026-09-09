---
name: 13-calculo-verbas-rescisorias
description: "Calcula verbas rescisórias por motivo (sem justa causa, justa causa, pedido de demissão, acordo, fim de contrato, aposentadoria, falecimento) com base em médias, FGTS, multa, IRRF e INSS."
allowed-tools: Read Grep Bash Edit Write
---

## Quando usar

Como advogado representando empregado (verificar pagamento correto / fundamentar inicial — skill 11) ou empregador (validar TRCT — skill 12). Skill espelho da contadora 29.

## Inputs necessários

1. Data de admissão e desligamento
2. Salário base + médias variáveis 12m (HE, comissões, adicionais)
3. Motivo (CLT art. 482, 483, 484, 484-A; Lei 13.467/17)
4. Saldo FGTS (extrato CAIXA / FGTS Digital)
5. Aviso prévio: trabalhado, indenizado, dispensa
6. Descontos legítimos: VT, plano, sindicato

## Tabela síntese — direitos por motivo

| Verba | Sem justa causa | Justa causa | Pedido demissão | Acordo (484-A) | Prazo determinado | Aposentadoria | Falecimento |
|---|---|---|---|---|---|---|---|
| Saldo salário | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Aviso prévio | Sim | Não | Empregado paga ou trabalha | 50% | Não (regra) | Não | Não |
| Férias vencidas + 1/3 | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Férias proporcionais + 1/3 | ✓ | Não (Súm 171 TST) | ✓ (Súm 261) | ✓ | ✓ | ✓ | ✓ |
| 13º proporcional | ✓ | Não | ✓ | ✓ | ✓ | ✓ | ✓ |
| FGTS (saque) | ✓ | Não | Não | 80% | ✓ | ✓ | ✓ (dep) |
| Multa 40% | ✓ | Não | Não | 20% | Não | Não | Não |
| Seguro-desemprego | ✓ | Não | Não | Não | Não | Não | Não |

## Cálculo padrão (sem justa causa — caso mais frequente)

```
Saldo salário = (dias trab no mês / 30) × salário
Aviso indenizado = 1 salário + Lei 12.506 (3 dias × ano completo, máx +60 dias)
Férias vencidas = 1 salário + 1/3
Férias proporcionais = (avos / 12) × salário × 1,33
13º proporcional = (avos / 12) × salário
FGTS rescisório:
  Saldo + depósito do mês corrente + sobre aviso indenizado
Multa 40% = sobre saldo + depósitos rescisórios
```

### Avos (CLT 146 e Lei 4.090)
- Cada mês com 15 ou + dias trabalhados = 1 avos.
- Aviso prévio indenizado **projeta tempo** (Súm 305 TST) — soma para avos de férias prop e 13º prop.

### Médias variáveis
- HE habituais
- Comissões
- Adicional noturno habitual
- Periculosidade / insalubridade habituais
- Calcular média 12 meses (ou desde a admissão se < 12)

## Descontos

### INSS
Sobre as verbas: **incide** em saldo, aviso, 13º. **Não incide** em férias indenizadas (proporcionais/vencidas pagas em rescisão), aviso indenizado (controvérsia, mas STJ inclina pela não incidência — REsp 1.230.957).

### IRRF
- Saldo de salário, 13º, médias: **incide** com tabela progressiva.
- Aviso indenizado: **não incide** (Súmula 463 STJ).
- Férias indenizadas: **não incide** (Tema 481 STJ; STF vem sinalizando incidência sobre 1/3 — acompanhar).
- Multa 40% FGTS: **não incide** (RE 595.838 STF).

## Exemplo numérico

Empregado: salário R$ 5.000, médias HE R$ 800, demissão 15/04/2026, admissão 15/03/2018, sem justa causa, aviso indenizado.

```
Tempo de casa: 8 anos 1 mês ≈ 8 anos (avos completos no aviso)
Aviso prévio Lei 12.506: 30 + (8 × 3) = 54 dias (cap 90)
Saldo salário (15 dias): 5.000 / 30 × 15 = R$ 2.500
Aviso indenizado: (5.000 + 800) × 54/30 = 5.800 × 1,8 = R$ 10.440
Férias vencidas (período 03/24-03/25): (5.000 + 800) × 1,33 = R$ 7.714
Férias prop: aviso projeta até 06/2026 → avos = 4/12 (abr-jun). Cálculo (5.800 × 4/12 × 1,33) = R$ 2.571
13º prop: avos = 6/12 (jan-jun com aviso). 5.800 × 6/12 = R$ 2.900
TOTAL BRUTO: R$ 26.125

INSS sobre saldo + 13º (segregar bases — saldo + 13º): conforme tabela
IRRF sobre saldo + 13º (DARF separado para 13º)

FGTS:
  Saldo CAIXA: ~R$ 38.400 (estimativa 8 anos × 8% × salário)
  Depósito rescisório (sobre aviso, 13º prop, férias prop): ___
  Multa 40%: 40% × (38.400 + dep rescis) = ___
```

## Acordo Lei 13.467/17 (CLT 484-A)

- Aviso prévio: 50% indenizado, 50% trabalhado
- Multa FGTS: 20%
- Saque FGTS: 80%
- Sem seguro-desemprego
- Demais verbas: completas (13º, férias, etc.)

## Templates

### Memória de cálculo (TRCT)

```
TRCT — Comp __/____ — Adm __/__/____ — Demissão __/__/____ — Motivo: 02 (s/ justa causa)
Salário base: R$ ____ Médias variáveis: R$ ____

VERBAS
1. Saldo salário (___ dias)................. R$ ________
2. Aviso indenizado (___ dias)............. R$ ________
3. Férias vencidas + 1/3.................... R$ ________
4. Férias proporcionais (__/12) + 1/3....... R$ ________
5. 13º proporcional (__/12)................. R$ ________
6. Adicionais (insal/peric/HE — média)..... R$ ________
SUBTOTAL.................................... R$ ________

DESCONTOS
INSS (saldo + aviso + 13º)................. R$ ________
IRRF (saldo + 13º somente).................. R$ ________
Plano de saúde / VT / sindicato............ R$ ________
SUBTOTAL.................................... R$ ________

LÍQUIDO RESCISÃO............................ R$ ________

FGTS
Saldo na CAIXA.............................. R$ ________
Depósitos rescisórios....................... R$ ________
Multa 40%................................... R$ ________
GRRF / FGTS Digital......................... R$ ________

PRAZO LEGAL DE PAGAMENTO: até 10 dias do desligamento (CLT 477 § 6º)
SOB PENA DE: multa do § 8º (1 salário em favor do empregado)
```

## Erros comuns

- IRRF aplicado em férias indenizadas e aviso indenizado → indevido (STJ Súmulas 463 e 498, Tema 481).
- INSS sobre 1/3 férias indenizado: STF declarou inconstitucional sobre **patronal** (Tema 985), mas para empregado a discussão segue.
- Acordo com multa 40% (errado: 20%).
- Não projetar aviso indenizado nos avos.
- Médias variáveis ignoradas — empregado perde dinheiro.
- Justa causa sem documentação (advertências) — invertível em juízo.

## Checklist

- [ ] Motivo do desligamento
- [ ] Tempo de casa exato (com aviso projetado)
- [ ] Médias variáveis dos últimos 12m
- [ ] Aviso prévio Lei 12.506 calculado
- [ ] FGTS: saldo + depósito do mês + dep rescisório + multa
- [ ] INSS e IRRF nas verbas tributáveis
- [ ] TRCT pronto e revisado
- [ ] Prazo de 10 dias respeitado
- [ ] eSocial S-2299 (skill contadora 24)
- [ ] GRRF / FGTS Digital (skill contadora 30)

## Referências

- CLT arts. 477-484-A
- Lei 13.467/2017
- Lei 12.506/2011 (aviso)
- Lei 8.036/1990 (FGTS)
- RE 595.838 STF (multa 40% IRRF)
- Tema 481 STJ
- Súmulas TST 171, 261, 305, 437; STJ 463, 498

---
name: apelacao-criminal
description: Estrutura apelação criminal (CPP 593) contra sentença condenatória/absolutória, em 5 dias úteis (interposição) + 8 dias (razões), com erros de fato/direito, dosimetria e regime.
allowed-tools: Read Grep Bash Edit Write
user-invocable: true
---

## Quando usar

Para impugnar:
- Sentença definitiva condenatória ou absolutória
- Sentença que julga improcedente queixa
- Sentença de pronúncia (CPP 593 II) — em ritual do júri há recurso em sentido estrito específico, mas essa é apelação
- Sentenças do Tribunal do Júri com ofensa às regras (CPP 593 III)

Prazo: **5 dias** para interposição + **8 dias** para razões (CPP 600). Para Ministério Público / querelante o prazo é o mesmo. Em rito sumário, prazos podem variar.

## Inputs necessários

1. Sentença
2. Termo de apresentação da defesa (se houver)
3. Provas produzidas no processo (autos completos)
4. Comprovação de tempestividade (intimação)
5. Manifestação se cliente quer recorrer (CPP 605)
6. Procuração

## Estrutura — interposição (em 5 dias)

```
EXMO. SR. JUIZ DA __ª VARA CRIMINAL DA COMARCA DE __________

Processo nº __________

[RÉU] vem, por seu defensor, com fulcro no art. 593 do CPP, interpor

APELAÇÃO

contra a r. sentença de fls. ___, que [resumir conclusão da sentença], requerendo sua remessa ao TJ-__ / TRF / STJ / STF.

[Local], [data]
________________________
[Defensor] OAB/__ ______
```

## Estrutura — razões (em 8 dias)

```
EGRÉGIA __ª CÂMARA / TURMA CRIMINAL DO TRIBUNAL DE __________

Apelante: __________
Apelado: __________

I — TEMPESTIVIDADE
Sentença publicada em __/__/____. Interposição em __/__/____. Razões agora em __/__/____. Tempestivo.

II — DOS FATOS E DA SENTENÇA
[Histórico do processo até a sentença]

III — DAS RAZÕES DE REFORMA

3.1. ERRO IN PROCEDENDO (vício processual)
   3.1.1. Cerceamento de defesa
   3.1.2. Nulidade absoluta (CPP 564)
   3.1.3. Sentença extra/ultra/citra petita

3.2. ERRO IN JUDICANDO (mérito)
   3.2.1. Atipicidade
   3.2.2. Excludente de ilicitude / culpabilidade
   3.2.3. Insuficiência probatória (in dubio pro reo — CPP 386 VII)
   3.2.4. Análise crítica das provas (testemunhas, perícia, reconhecimento)
   3.2.5. Negativa de autoria

3.3. DESCLASSIFICAÇÃO
   3.3.1. Roubo → furto
   3.3.2. Tráfico → uso (Lei 11.343 art. 28)
   3.3.3. Homicídio doloso → culposo
   ...

3.4. DOSIMETRIA
   3.4.1. Pena-base reduzida ao mínimo (CP 59 — circunstâncias judiciais favoráveis)
   3.4.2. Atenuantes (CP 65) não aplicadas
   3.4.3. Causas de diminuição (tentativa CP 14, art. 33 § 4º Lei 11.343, etc.)
   3.4.4. Substituição por restritivas de direitos (CP 44)
   3.4.5. Sursis (CP 77)
   3.4.6. Regime inicial menos gravoso (Súm 718-719 STF)
   3.4.7. Detração (CP 42; Lei 7.210 art. 111)

IV — DOS PEDIDOS

a) Conhecimento e provimento do recurso para:
   a.1) ABSOLVIÇÃO do apelante por uma das hipóteses do CPP 386
   a.2) Subsidiariamente, a anulação da sentença com retorno dos autos para novo julgamento
   a.3) Sucessivamente, desclassificação para __________
   a.4) Em qualquer caso, a redução da pena, aplicação de atenuantes, substituição, sursis, regime aberto/semiaberto

b) Concessão / manutenção do efeito suspensivo da pena (CPP 597 — apelação contra sentença condenatória pode ter efeito suspensivo se réu não estiver preso ou se não houver decisão que mantenha a prisão)

c) Em caso de réu preso: alvará de soltura ou conversão em regime mais brando

[Local], [data]
________________________
[Defensor] OAB/__ ______
```

## Pontos críticos

### Análise crítica de provas em apelação
- Testemunhas: contradições, impedimento, suspeição
- Reconhecimento: Tema 1.016 STJ (CPP 226)
- Cadeia de custódia (CPP 158-A)
- Confissão extrajudicial sem ratificação em juízo (Súm 545 STF)

### Dosimetria — atacar cada fase

**1ª fase (CP 59)**
- Cada circunstância judicial: motivar a alteração
- Súm 444 STJ: inquéritos e ações em andamento não podem agravar

**2ª fase**
- Súm 231 STJ: atenuante não pode reduzir abaixo do mínimo legal
- Confissão: Súm 545 STF; CP 65 III "d"

**3ª fase**
- Tentativa CP 14: ¹/³ a ²/³ (1/3 + comprometimento próximo da consumação)
- Tráfico privilegiado (Lei 11.343 art. 33 § 4º): 1/6 a 2/3 — STF Tema 1.052: hediondez excluída no privilegiado

### Regime inicial
- Súm 719 STF: pena ≤ 4 anos primário não pode ir ao fechado
- Súm 440 STJ: regime inicial vincula-se à pena, não a critério judicial
- Súm 269 STJ: reincidente em pena ≤ 4 anos pode ir ao semiaberto se circunstâncias forem favoráveis

### Substituição por restritivas (CP 44)
- Pena ≤ 4 anos
- Crime sem violência ou grave ameaça
- Não reincidente em crime doloso
- Circunstâncias judiciais favoráveis

## Apelação no Tribunal do Júri (CPP 593 III)

Especificidades:
- Ofensa às regras de procedimento → anular julgamento (a, b, c, d)
- Decisão dos jurados manifestamente contrária à prova dos autos (d) → novo julgamento (não pode ser revisto duas vezes pelo mesmo motivo — CPP 593 § 3º)

## Apelação do MP

- MP pode recorrer pela majoração ou cassação da absolvição
- Para condenado, isso significa risco de pena maior em recurso do MP

## Erros comuns

- Não impugnar todos os pontos da sentença → preclusão.
- Apelação cópia da defesa final.
- Esquecer dosimetria como pedido subsidiário.
- Não pedir efeito suspensivo / soltura quando preso.
- Atacar prova já reconhecida pelo apelado (sem confronto direto).
- Não juntar atestado de antecedentes atualizado (para regime/substituição).

## Checklist

- [ ] Tempestividade: 5 dias interposição + 8 dias razões
- [ ] Nulidades atacadas
- [ ] Análise crítica das provas
- [ ] Pedido principal de absolvição
- [ ] Pedidos subsidiários: desclassificação, dosimetria, regime, substituição
- [ ] Efeito suspensivo / soltura
- [ ] Procuração e manifestação de vontade do réu (CPP 605)
- [ ] Documentos atualizados (antecedentes, certidões)
- [ ] Protocolo OK

## Referências

- CPP arts. 564 (nulidades), 593-595, 597, 600, 605, 386, 158-A
- CP arts. 14, 23-28, 33, 42, 44, 59, 65-66, 71, 77
- Súmulas STF 718, 719, 545; STJ 231, 269, 440, 444
- Tema 1.016 STJ (reconhecimento)
- Tema 1.052 STF (tráfico privilegiado)

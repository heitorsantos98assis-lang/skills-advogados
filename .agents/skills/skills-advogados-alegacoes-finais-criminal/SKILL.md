---
name: skills-advogados-alegacoes-finais-criminal
description: "Estrutura alegações finais (memoriais escritos — CPP 403 §3º) com análise da prova produzida, teses de absolvição/desclassificação, dosimetria preventiva e pedidos."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Claude, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Após instrução criminal (audiência una de inquirição) e a oitiva das testemunhas, se o juiz determinar conversão em memoriais escritos. Prazo: **5 dias** para acusação e depois 5 dias para defesa (CPP 403 § 3º). Em rito ordinário, podem ser orais em audiência (20 minutos cada).

## Inputs necessários

1. Denúncia
2. Resposta à acusação (skill 25)
3. Termos de audiência (depoimentos)
4. Vídeo / áudio das audiências (se disponível)
5. Provas produzidas no processo
6. Antecedentes do réu (atestado de antecedentes criminais)
7. Comprovação de circunstâncias pessoais favoráveis (trabalho, residência, família)
8. Procuração

## Estrutura

```
EXMO. SR. JUIZ DA __ª VARA CRIMINAL DA COMARCA DE __________

Processo nº __________

Réu: __________

Vem, por seu defensor, apresentar

ALEGAÇÕES FINAIS / MEMORIAIS

nos termos do art. 403 § 3º do CPP, conforme análise da prova produzida.

I — DOS FATOS E DA INSTRUÇÃO
[Resumo da denúncia, do que foi colhido em juízo]

II — DA PROVA PRODUZIDA — ANÁLISE CRÍTICA

2.1. Da prova testemunhal
   2.1.1. Testemunha __________: depôs que __________
       - Contradição com __ (CPP 209)
       - Imprecisão / hesitação / alegações genéricas
       - Comprometido pelo vínculo com a vítima
   2.1.2. Testemunha __________: depôs que __________
       - Confirma a tese da defesa em [ponto]
   ...

2.2. Da prova documental
2.3. Da prova pericial
2.4. Do depoimento do réu (interrogatório)
   - Confissão? (atenuante CP 65 III "d")
   - Negativa coerente
   - Direito ao silêncio (CF 5º LXIII) preservado

III — DAS TESES DE DEFESA

3.1. Atipicidade material (insignificância — HC 84.412/STF, Tema 1.099)
3.2. Excludente de ilicitude (CP 23)
   - Legítima defesa: prova de moderação, agressão atual, meios necessários
3.3. Excludente de culpabilidade (CP 26-28)
3.4. Negativa de autoria
   - Ausência de provas robustas
   - Reconhecimento sem observância do CPP 226 (Tema 1.016 STJ)
3.5. Atipicidade (fato não é crime)
3.6. Desclassificação para crime menos grave
   - Ex.: roubo → furto (sem violência ou grave ameaça)
   - Ex.: tráfico → uso (Lei 11.343/06 art. 28 + critérios)
3.7. Dúvida razoável (in dubio pro reo — CPP 386 VII)

IV — DA DOSIMETRIA PREVENTIVA (em caso de eventual condenação)
4.1. Pena-base mínima — circunstâncias judiciais (CP 59) favoráveis
4.2. Atenuantes (CP 65) — confissão, menoridade relativa, motivo de relevante valor
4.3. Causas de diminuição (CP 14 II tentativa, CP 16 arrependimento, art. 33 § 4º Lei 11.343)
4.4. Substituição da pena por restritiva de direitos (CP 44)
4.5. Suspensão condicional (CP 77 — sursis)
4.6. Regime aberto / detração

V — DOS PEDIDOS

a) ABSOLVIÇÃO com base no art. 386 do CPP, hipótese __:
   I. estar provada a inexistência do fato
   II. não haver prova da existência do fato
   III. não constituir o fato infração penal
   IV. estar provado que o réu não concorreu
   V. não existir prova de ter o réu concorrido
   VI. existirem circunstâncias que excluam o crime
   VII. não existir prova suficiente para condenação

b) Subsidiariamente, DESCLASSIFICAÇÃO para crime menos grave;
c) Sucessivamente, em caso de condenação:
   c.1) Pena-base no mínimo
   c.2) Aplicação de todas as atenuantes
   c.3) Substituição por penas restritivas de direitos
   c.4) Sursis (CP 77)
   c.5) Regime inicial menos gravoso (Súm 718-719 STF)
d) Em qualquer caso, expedição de alvará de soltura se houver prisão preventiva.

[Local], [data]
________________________
[Defensor] OAB/__ ______
```

## Análise crítica de provas — pontos a abordar

### Testemunha
- Coerência interna do depoimento
- Coerência com outros elementos (perícia, documental)
- Vínculo com a vítima/acusado (CPP 206 — informante; CPP 207 — impedida)
- Tempo de exposição ao fato (visibilidade, distância, iluminação, agitação emocional)

### Reconhecimento de pessoas (Tema 1.016 STJ)
- Procedimento do CPP 226 deve ter sido observado
- Sem fila de comparação, sem múltiplas pessoas semelhantes → fragilidade

### Perícia
- Cadeia de custódia (CPP 158-A a 158-F)
- Quesitos respondidos
- Habilitação do perito

### Confissão
- Voluntária? Em sede policial?
- Confessou em juízo?
- Coerente com prova material?

## Dosimetria — método trifásico (CP 68)

```
1ª fase — Pena-base (CP 59):
   - Culpabilidade
   - Antecedentes
   - Conduta social
   - Personalidade
   - Motivos
   - Circunstâncias
   - Consequências
   - Comportamento da vítima
   ⇒ Fixar entre mínimo e máximo

2ª fase — Atenuantes (CP 65) e Agravantes (CP 61-62):
   ⇒ Aplicar, sem ultrapassar mínimo nem máximo (Súm 231 STJ atenuantes; Súm 718-719 STF regime)

3ª fase — Causas de diminuição/aumento:
   - Tentativa (CP 14 II): 1/3 a 2/3
   - Concurso material (CP 69)
   - Concurso formal (CP 70)
   - Continuidade delitiva (CP 71)
   - Causas específicas (art. 33 § 4º Lei 11.343/06: 1/6 a 2/3)
```

## Substituições e benefícios

### Pena restritiva de direitos (CP 44)
- Pena ≤ 4 anos
- Crime sem violência ou grave ameaça (não aplica em crimes hediondos)
- Não reincidente em crime doloso
- Modalidades: prestação serviços comunidade, perda de bens, prestação pecuniária, limitação de fim-de-semana, interdição temporária

### Sursis (CP 77)
- Pena ≤ 2 anos
- Não reincidente em crime doloso
- Período de prova 2-4 anos com condições

### Regime inicial (Súm 719-440 STF + CP 33)
- Aberto: pena ≤ 4 anos, primário
- Semiaberto: 4-8 anos OU reincidente com 4 anos
- Fechado: > 8 anos

## Erros comuns

- Repetir resposta à acusação sem analisar a prova produzida.
- Não atacar testemunha-chave ponto a ponto.
- Esquecer dosimetria preventiva — em condenação, fica sem subsídio.
- Esquecer pedidos subsidiários (substituição, sursis).
- Não pleitear absolvição quando há dúvida razoável (CPP 386 VII).
- Confissão sem pedir atenuante.
- Reconhecimento sem questionar Tema 1.016 STJ.

## Checklist

- [ ] Análise crítica de cada prova
- [ ] Tese principal de absolvição articulada
- [ ] Teses subsidiárias (desclassificação, dosimetria)
- [ ] Atenuantes, causas de diminuição
- [ ] Substituição / sursis / regime
- [ ] Soltura se preso
- [ ] Prazo de 5 dias respeitado
- [ ] Procuração ativa

## Referências

- CPP arts. 158-A a 158-F (cadeia de custódia), 226 (reconhecimento), 386 (absolvição), 403 (memoriais), 65 ss
- CP arts. 14, 23, 26-28, 44, 59, 61-62, 65, 68, 71, 77, 109
- Súmulas STF 718, 719; STJ 231, 438, 269 (reincidência)
- HC 84.412/SP (bagatela)
- Tema 1.016 STJ (reconhecimento)
- Tema 1.099 STF (insignificância)

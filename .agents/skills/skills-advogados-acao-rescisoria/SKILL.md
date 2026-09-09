---
name: skills-advogados-acao-rescisoria
description: "Estrutura ação rescisória (CPC 966-975) para desconstituir sentença transitada em julgado por dolo, prevaricação, prova falsa, documento novo, violação manifesta da norma, no prazo bienal."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Claude, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Para desconstituir decisão **transitada em julgado** com vício de:
- Prevaricação, concussão ou corrupção do juiz
- Dolo ou coação da parte vencedora ou colusão entre partes
- Ofensa à coisa julgada
- Violação manifesta de norma jurídica (com ou sem entendimento vinculante)
- Prova cuja falsidade tenha sido apurada em processo criminal ou nos próprios autos
- Documento novo, ignorado pela parte ou de que não pôde fazer uso
- Após sentença, fundada em prova cuja falsidade tenha sido apurada
- Inobservância de norma do art. 525 § 12 ou 535 § 5º (precedente vinculante)

**Prazo: 2 anos** do trânsito em julgado (CPC 975) — prazo decadencial.

## Inputs necessários

1. Sentença/acórdão rescindendo (íntegra com data do trânsito)
2. Comprovação do vício (sentença criminal, documento novo, precedente vinculante)
3. Procuração e poderes especiais (CPC 105)
4. Depósito de 5% do valor da causa (CPC 968 II) — exceto Fazenda, MP, gratuidade
5. Provas que serão produzidas

## Hipóteses (CPC 966) — detalhe

### I — Prevaricação, concussão, corrupção
Vício no juiz: precisa de sentença criminal transitada em julgado ou ação penal em curso.

### II — Dolo / coação / colusão
Comportamento da parte vencedora que enganou o juízo. Demonstrar.

### III — Ofensa à coisa julgada
Decisão posterior ignora julgamento anterior protegido pela coisa julgada material.

### IV — Violação manifesta da norma jurídica
Aplicação ou interpretação **errada e clara**. CPC 489 §1º + jurisprudência: violação não é mero erro de julgamento, e sim erro patente. Súmula 343 STF: cabe rescisória mesmo sem unanimidade jurisprudencial em divergência manifesta.

### V — Prova falsa
Confirmada em ação penal ou nos autos da rescisória.

### VI — Documento novo
Documento existente à época, mas a parte não conhecia ou não pôde usar — capaz de mudar o resultado.

### VII — (revogado pela Lei 13.105/15)

### VIII — Inobservância de precedente vinculante (CPC 525 §12, 535 §5º)
Decisão que descumpre súmula vinculante, precedente do STF/STJ em RE/REsp repetitivos, IRDR.

## Inadmissibilidade

- Decisões interlocutórias (em regra) — exceção: aquelas que decidem o mérito.
- Decisão sem trânsito em julgado.
- Decisão que aplique entendimento posteriormente alterado pela jurisprudência (Súm 343 STF — não cabe se a divergência era razoável à época).

## Estrutura

```
EXMO. SR. DESEMBARGADOR PRESIDENTE DO TRIBUNAL DE JUSTIÇA / TRF / TST / STJ / STF

Ação Rescisória — CPC 966 a 975

Autor: __________
Réu: __________
(Foro: tribunal que julgou a decisão rescindenda)

I — DA COMPETÊNCIA
A presente ação compete ao [TJ-__ / TRF-__ / STJ / STF], pois a decisão rescindenda foi proferida em última instância no respectivo tribunal.

II — DA TEMPESTIVIDADE
Decisão transitada em julgado em __/__/____. Prazo bienal terminando em __/__/____. Esta ação é interposta tempestivamente.

III — DO DEPÓSITO PRÉVIO (CPC 968 II)
Junta-se guia de depósito no valor de 5% do valor da causa (R$ __________) à disposição do juízo, nos termos do art. 968, II do CPC.

IV — DOS FATOS
[Narrar o processo originário, a sentença/acórdão impugnado e o vício]

V — DO VÍCIO RESCISÓRIO (CPC 966, INCISO __)
[Detalhar o vício específico — descrever a violação, provar com documentos]

5.1. Da [hipótese específica do art. 966]
5.2. Da prova do vício
5.3. Do impacto no julgamento (sem o vício, o resultado seria outro)

VI — DO PEDIDO RESCISÓRIO E DO IUDICIUM RESCINDENS / RESCISSORIUM
6.1. Iudicium rescindens: desconstituir a sentença/acórdão por padecer de [vício].
6.2. Iudicium rescissorium: rejulgar o mérito do processo originário, decidindo-se pelo seguinte:
   [exposição da nova solução pretendida]

VII — DOS PEDIDOS
Diante do exposto, requer:
a) Recebimento e processamento da rescisória;
b) Citação do réu para contestar em 15 a 30 dias (a depender do regimento);
c) Procedência para:
   c.1) Desconstituir a sentença/acórdão rescindendo;
   c.2) Em juízo rescisório, julgar [novo resultado];
d) Honorários recursais;
e) Custas e honorários.

VIII — DO VALOR DA CAUSA: R$ __________ (proveito econômico)
```

## Procedimento (CPC 968-975)

1. Distribuição no tribunal competente.
2. Relator decide sobre admissibilidade.
3. Citação do réu (prazo varia por tribunal — usualmente 15-30 dias).
4. Instrução probatória.
5. Voto do relator + julgamento colegiado.

### Tutela de urgência
CPC 969: o autor pode requerer suspensão dos efeitos da decisão rescindenda — risco de execução em curso.

## Casos comuns

### Recém-julgado pelo STF/STJ em sentido oposto
- Súm 343 STF e Tema 736 STF: se à época da decisão a divergência era razoável, não cabe rescisória.
- Se decisão era manifestamente contra súmula vinculante ou precedente repetitivo prévio, cabe.

### Documento novo (CPC 966 VII)
- Documento existente no momento da decisão, mas oculto ou desconhecido.
- Não vale documento produzido depois (laudo posterior, prova nova).

## Erros comuns

- Confundir rescisória com recurso (rescisória é ação autônoma, sob condição de coisa julgada).
- Perder prazo de 2 anos (decadencial — não admite suspensão / interrupção, salvo Súm 401 STJ — partilha em separado).
- Não depositar 5% — extinção sem mérito, salvo gratuidade.
- Fundamentar em "injustiça" — não basta; precisa hipótese do art. 966.
- Querer rediscutir prova — Súmula 343 STF / Súm 7 STJ: rescisória não é via para reanálise probatória.

## Checklist

- [ ] Decisão transitada em julgado
- [ ] Hipótese do art. 966 mapeada com prova
- [ ] Prazo de 2 anos não expirado
- [ ] Procuração com poderes especiais
- [ ] Depósito de 5% (ou gratuidade)
- [ ] Documentos do processo originário juntados
- [ ] Pedido rescisório + rescissório explícitos
- [ ] Valor da causa correto (proveito econômico)
- [ ] Tutela de suspensão (se houver execução em curso)

## Referências

- CPC arts. 966-975
- Súmula 343 STF (divergência razoável)
- Súmula 7 STJ (reexame probatório)
- Tema 736 STF
- Súmula 401 STJ (partilha em fase própria)

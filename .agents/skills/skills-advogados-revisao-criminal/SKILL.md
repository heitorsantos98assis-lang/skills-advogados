---
name: skills-advogados-revisao-criminal
description: "Estrutura revisão criminal (CPP 621-631) para desconstituir condenação transitada em julgado por contrariedade ao texto expresso, prova nova, sentença em prova falsa, sem prazo decadencial."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Codex, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Para impugnar **condenação criminal transitada em julgado** quando há:
- Sentença contrária ao texto expresso de lei ou à evidência dos autos (CPP 621 I)
- Sentença fundada em depoimentos, exames ou documentos comprovadamente falsos (CPP 621 II)
- Descoberta de novas provas de inocência ou de circunstância que autorize diminuição de pena (CPP 621 III)

**Sem prazo** — pode ser proposta a qualquer tempo, inclusive após cumprimento de pena (CPP 622).

Pode ser proposta:
- Pelo próprio condenado
- Por procurador legalmente habilitado
- Pelo MP
- Pelo cônjuge, ascendente, descendente ou irmão (em caso de morte do condenado — CPP 623)

## Inputs necessários

1. Sentença condenatória + acórdão confirmatório
2. Comprovação do trânsito em julgado
3. Prova nova (documento, perícia, testemunha)
4. Análise da contradição ao texto expresso de lei
5. Antecedentes do condenado e situação atual

## Hipóteses (CPP 621)

### I — Contrariedade ao texto expresso de lei OU à evidência dos autos

**Texto expresso de lei**:
- Tribunal aplicou pena fora do mínimo/máximo legal
- Aplicou regime mais grave do que o cabível
- Não aplicou causa de diminuição obrigatória

**Evidência dos autos**:
- Decisão claramente contraditória com o que está nos autos
- Não confunda com reanálise probatória — precisa ser **manifesta**

### II — Prova falsa

- Testemunha falsa, perícia falsa, documento falso
- Falsidade reconhecida em ação penal autônoma OU na própria revisão (excepcionalmente)

### III — Prova nova

- Documento, depoimento, perícia que não existia ou era desconhecida
- Capaz de **modificar o resultado**: absolver, atenuar, reduzir pena, alterar regime
- Cuidado: prova nova ≠ prova revalorada (Súm 7 STJ inaplicável aqui, mas há limites)

## Competência

| Decisão revisanda | Tribunal competente |
|---|---|
| Tribunal de Justiça | TJ (composição plena ou Seção Criminal) |
| TRF | TRF |
| STF (matéria criminal) | STF |
| STJ | STJ |

## Estrutura

```
EXMO. SR. DESEMBARGADOR PRESIDENTE DO __ ª SEÇÃO CRIMINAL DO TJ-__ / DOUTO MINISTRO DO STJ

REVISÃO CRIMINAL
Revisado: __________ (réu condenado)
Decisão revisanda: Acórdão de __/__/____ no Processo nº __________

[REQUERENTE] (qualificação completa) vem, com fulcro nos arts. 621 a 631 do CPP, propor

REVISÃO CRIMINAL

contra a r. condenação proferida no [TJ / TRF / vara] em __/__/____ (cópia anexa), pelas razões a seguir.

I — DA TEMPESTIVIDADE
A revisão criminal não tem prazo (CPP 622), podendo ser proposta a qualquer tempo, mesmo após cumprimento da pena.

II — DOS FATOS E DA CONDENAÇÃO
[Resumo do processo originário e da decisão]

III — DA HIPÓTESE DA REVISÃO (CPP 621)

3.1. [Inciso I — contrariedade ao texto expresso de lei]
   - A sentença/acórdão violou o dispositivo __ ao __________
   - O entendimento aplicado contraria o art. __ do CP
   - [Demonstrar com clareza]

3.2. [Inciso II — prova falsa]
   - O depoimento da testemunha __, base da condenação, é comprovadamente falso (sentença criminal anexa, ou prova produzida nesta revisão)
   - A perícia __ foi desautorizada por nova perícia [nova prova]

3.3. [Inciso III — prova nova]
   - Documento __ produzido em __/__/____ ou descoberto em __/__/____
   - Capacidade de alterar o resultado: [absolvição / desclassificação / pena atenuada]
   - Não disponível à época do processo originário porque __________

IV — DOS FUNDAMENTOS — IMPACTO NO RESULTADO
[Demonstrar como, sem o vício/com a prova nova, a decisão seria diferente]

V — DOS PEDIDOS
a) Recebimento e processamento da revisão;
b) Vista ao Ministério Público (CPP 625);
c) Procedência para:
   c.1) Iudicium rescindens: desconstituir o acórdão / sentença condenatória;
   c.2) Iudicium rescissorium: absolver o requerente OU desclassificar para __ OU reduzir a pena para __ OU alterar o regime para __;
d) Eventual indenização do estado (CPP 630) por erro judiciário, comprovados os pressupostos;
e) Comunicação para fins de averbação no registro criminal (CPP 800) e exclusão de antecedentes;
f) Soltura imediata se o requerente está preso e a prova é robusta.

VI — DAS PROVAS
- Documental anexa
- Eventual oitiva de testemunhas em revisão (incomum)
- Eventual perícia nova (anexa laudo)

[Local], [data]
________________________
[Advogado] OAB/__ ______
```

## Indenização do estado por erro judiciário (CPP 630)

Se a revisão **absolver** ou modificar a pena, com prova manifesta de que a condenação foi resultado de erro grave do estado, possível pleitear indenização.

- Não automática
- Requerimento separado em sede de execução

## Aspectos práticos

### Documentação da prova nova
- Como foi produzida
- Por que não estava disponível
- Robustez para alterar o julgamento

### Não cabimento
- Recurso ainda pendente → use apelação/HC
- Mero inconformismo → não basta
- Reanálise de prova já valorada → não cabe (precisa de prova efetivamente nova ou contrariedade ao texto expresso)

### Súmula 393 do STF
"Para requerer revisão criminal, o condenado **não é obrigado a recolher-se à prisão**" — útil para fugitivos / sentenciados em regime aberto.

## Erros comuns

- Confundir revisão com nova apelação.
- Apresentar como prova nova algo já discutido nos autos.
- Falta de demonstração de impacto: ainda que houvesse a prova, condenação seria a mesma.
- Não solicitar indenização (CPP 630) quando absolvido em revisão.
- Esquecer averbação no registro criminal.
- Apresentar revisão sem o trânsito em julgado.

## Checklist

- [ ] Trânsito em julgado da condenação
- [ ] Hipótese do CPP 621 mapeada
- [ ] Prova nova (se for o caso) com clareza
- [ ] Demonstração de impacto no resultado
- [ ] Pedido rescindens + rescissorium
- [ ] Indenização por erro (se cabível)
- [ ] Procuração com poderes específicos
- [ ] Provas juntadas e bem identificadas
- [ ] Comunicação para averbação posterior

## Referências

- CPP arts. 621-631
- Súmula 393 STF (não recolhimento)
- Súmula 152 TFR (revisão e prova)
- Convenção Americana de Direitos Humanos art. 8.4

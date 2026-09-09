---
name: skills-advogados-embargos-declaracao
description: "Estrutura embargos de declaração (CPC 1.022-1.026) para sanar omissão, contradição, obscuridade ou erro material em decisão, sentença ou acórdão, em 5 dias úteis, com efeitos infringentes quando cabível."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Codex, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Para apontar:
- **Omissão** (CPC 489 § 1º — vícios da motivação)
- **Contradição** entre fundamentos ou entre fundamento e dispositivo
- **Obscuridade** que dificulta a execução / cumprimento
- **Erro material** (CPC 1.022, parágrafo único III — incluído pela Lei 13.105/2015)

Prazo: **5 dias úteis** (CPC 1.023). Pode ser interposto contra qualquer decisão (interlocutória, sentença, acórdão).

Embargos **interrompem** o prazo dos demais recursos (CPC 1.026).

## Inputs necessários

1. Decisão/sentença/acórdão objeto
2. Comprovação de tempestividade (intimação)
3. Identificação clara do vício (omissão, contradição, obscuridade, erro material)
4. Argumento do prequestionamento (se objetivo é levar tema para STJ/STF)

## Estrutura

```
EXMO. SR. JUIZ / DESEMBARGADOR / MIN. RELATOR

Processo nº __________

__________ [embargante], por seu procurador, nos autos do processo em epígrafe, com fulcro no art. 1.022 do CPC, vem opor

EMBARGOS DE DECLARAÇÃO

contra a r. [decisão/sentença/acórdão] de fls. __, pelos motivos a seguir.

I — TEMPESTIVIDADE
[Decisão proferida em __/__/____. Intimação em __/__/____. 5 dias úteis. Termo final __/__/____. Embargos opostos nesta data.]

II — DO VÍCIO IDENTIFICADO

2.1. Da omissão / contradição / obscuridade / erro material
[Apontar especificamente: "A r. sentença é omissa quanto à __, pois deixou de se manifestar sobre __, ponto controvertido a que se referem os arts. __ do CPC..."]

III — DOS FUNDAMENTOS QUE DEVERIAM TER SIDO APRECIADOS
[Reproduzir o ponto da defesa/inicial que não foi enfrentado, com referência aos autos]

IV — DO PEQUESTIONAMENTO [se aplicável]
Os presentes embargos têm também finalidade de prequestionar a matéria constitucional/federal para fins de futuro recurso ao STF/STJ:
   - Art. __ da CF, sob alegação de __________
   - Art. __ da Lei __, sob alegação de __________
(CPC 1.025 — prequestionamento ficto: matérias examinadas no acórdão recorrido se consideram prequestionadas, mesmo se rejeitados os embargos)

V — DOS PEDIDOS
Diante do exposto, requer:
a) O conhecimento dos embargos;
b) O acolhimento para sanar o vício apontado, [especificar como deve ser sanado];
c) Subsidiariamente, com efeitos infringentes, a alteração da [decisão] para [pedido];
d) O prequestionamento das matérias acima (CPC 1.025);
e) [Se aplicável] A determinação de novo prazo para outros recursos (CPC 1.026 — interrupção).

[Local, data]
________________________
[Advogado] OAB/__ ______
```

## Vícios — diferença prática

| Vício | Como apontar |
|---|---|
| Omissão | "A decisão deixou de apreciar [tese/argumento/prova]." Citar onde está nos autos. |
| Contradição | Mostrar duas afirmações inconsistentes na mesma decisão. |
| Obscuridade | Indicar frase ou parte cuja interpretação é dúbia. |
| Erro material | Erro de cálculo, nome, número, data — corrigível sem alteração do mérito. |

**CPC 489 § 1º — não fundamentação**: hipóteses específicas em que decisão é considerada não fundamentada (limita-se a transcrever lei, súmula, ou se contradiz com seus fundamentos). Pode-se opor embargos por esses vícios.

## Efeitos infringentes

Em regra, embargos **não modificam** o resultado, apenas integram. Mas quando o vício é tamanho que o resultado precisa mudar (acolhimento da omissão sobre prova essencial, por exemplo), há efeitos infringentes.

Exemplo: sentença omissa sobre quem é a parte ré → embargos esclarecem e mudam quem é condenado.

Quando se postula efeitos infringentes, deve-se intimar a outra parte para contrarrazões em 5 dias (CPC 1.023 § 2º).

## Multa por procrastinação (CPC 1.026 § 2º)

- Embargos manifestamente protelatórios → multa de até 2% sobre valor atualizado da causa.
- Reincidência → até 10%.
- Boa fé processual: opor com fundamento.

## Prequestionamento ficto (CPC 1.025)

Mesmo com embargos rejeitados pelo tribunal, considera-se prequestionada a matéria, podendo subir para STJ/STF.

## Erros comuns

- Embargos puramente protelatórios → multa.
- Tentar rediscutir mérito sem apontar vício específico (omissão, contradição, etc.).
- Perder prazo de 5 dias úteis.
- Não interpor para fins de prequestionamento e perder a oportunidade no STJ/STF.
- Embargos contra decisão sem motivação que precisaria de outro recurso (não use embargos para o que cabe agravo).
- Reclamar de "fundamento equivocado" — isso é mérito de apelação, não de embargos.

## Checklist

- [ ] Vício específico identificado (omissão / contradição / obscuridade / erro material)
- [ ] Tempestividade: 5 dias úteis
- [ ] Pedido claro de sanar o vício
- [ ] Eventuais efeitos infringentes solicitados
- [ ] Prequestionamento (se for o caso)
- [ ] Não há intuito protelatório (proteger contra multa)
- [ ] Protocolo OK

## Referências

- CPC arts. 1.022-1.026
- CPC art. 489 § 1º (fundamentação)
- Súmula 98 STJ — embargos para prequestionamento não são protelatórios
- Súmula 33 STJ — prequestionamento implícito é admitido em certas hipóteses

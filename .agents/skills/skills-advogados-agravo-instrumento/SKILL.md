---
name: skills-advogados-agravo-instrumento
description: "Estrutura agravo de instrumento (CPC 1.015-1.020) contra decisões interlocutórias da lista taxativa (com flexibilização do Tema 988 STJ), com peças obrigatórias e pedido de efeito suspensivo."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Claude, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Para impugnar **decisão interlocutória** (não sentença) em uma das hipóteses do art. 1.015 do CPC ou nas hipóteses por interpretação extensiva do **Tema 988 STJ** (REsp 1.704.520) — quando a decisão pode causar prejuízo de difícil ou impossível reparação.

Prazo: **15 dias úteis** (CPC 1.003 § 5º) da intimação da decisão.

## Hipóteses do art. 1.015 (rol)

I — Tutelas provisórias
II — Mérito do processo
III — Rejeição da alegação de convenção de arbitragem
IV — Incidente de desconsideração da personalidade jurídica
V — Rejeição do pedido de gratuidade ou acolhimento da impugnação
VI — Exibição/posse de documento ou coisa
VII — Exclusão de litisconsorte
VIII — Rejeição do pedido de limitação do litisconsórcio
IX — Admissão/inadmissão de intervenção de terceiros
X — Concessão/modificação/revogação do efeito suspensivo aos embargos à execução
XI — Redistribuição do ônus da prova
XII — (vetado)
XIII — Outras hipóteses expressamente referidas em lei

**Tema 988 STJ**: hipóteses do 1.015 são taxativas, mas admite-se mitigação em decisões que causem **prejuízo iminente ou irreparável**, fora do rol — caso a caso (taxatividade mitigada).

## Inputs necessários

1. Decisão interlocutória (com data de publicação)
2. Petição inicial e contestação (cópias)
3. Documentos relevantes para o ponto recorrido
4. Procuração e contrato de honorários
5. Custas (preparo)
6. Demonstração da urgência (para pedido de efeito suspensivo / antecipado)

## Estrutura

```
EXMO. SR. DESEMBARGADOR PRESIDENTE DO TRIBUNAL DE JUSTIÇA DE __________

Agravante: __________
Agravado: __________
Origem: __ª Vara __ da Comarca de __________ — Processo nº __________

__________ [agravante], por seu procurador, com fulcro nos arts. 1.015 e 1.016 do CPC, vem interpor

AGRAVO DE INSTRUMENTO

contra a decisão interlocutória proferida em __/__/____ pelo MM. Juiz __________ que [resumir o que foi decidido], pelas razões a seguir.

I — TEMPESTIVIDADE
Decisão proferida em __/__/____, intimação em __/__/____. 15 dias úteis. Termo final: __/__/____. Recurso interposto nesta data.

II — PREPARO
Guia DARJ/DJE/DARE nº __________ R$ __________ + porte R$ __________.

III — DAS PEÇAS OBRIGATÓRIAS (CPC 1.017)
Conforme art. 1.017, instruem o presente:
   1. Cópia da petição inicial
   2. Cópia da contestação
   3. Cópia do despacho/decisão agravada
   4. Cópia da certidão de intimação
   5. Cópia da procuração outorgada ao(s) advogado(s) das partes

(Em PJe, juntada automática ou opcional — confirmar regimento)

IV — DOS FATOS
[Síntese: o que o autor pediu, o que o réu opôs, qual decisão atacada e por qual motivo]

V — DA HIPÓTESE DO ART. 1.015 [ou Tema 988]
A decisão se enquadra no inciso ___ do art. 1.015 do CPC, pois __________.
[Se taxatividade mitigada: demonstrar prejuízo iminente, urgência irreparável]

VI — DAS RAZÕES DO AGRAVO
[Tese de fato e de direito]

VII — DO EFEITO SUSPENSIVO ATIVO / SUSPENSIVO (CPC 1.019, I)
Há urgência justificada para que o relator, em decisão monocrática, atribua efeito suspensivo / antecipe os efeitos da tutela recursal, pois __________ (demonstrar risco).

VIII — DOS PEDIDOS
Diante do exposto, requer:
a) A atribuição de efeito suspensivo / antecipado da tutela recursal (CPC 1.019, I);
b) A intimação do agravado para apresentar resposta no prazo de 15 dias (CPC 1.019, II);
c) A oitiva do MP, se cabível (CPC 1.019, III);
d) Ao final, o conhecimento e provimento do agravo, para reformar a decisão e __________;
e) A condenação do agravado em honorários recursais (CPC 85 § 11).

[Local, data]
________________________
[Advogado] OAB/__ ______
```

## Comunicação ao juiz de 1ª instância

CPC 1.018 — em **3 dias** após interposição, juntar nos autos do processo de origem cópia da petição do agravo + comprovante de protocolo + relação dos documentos. **Pena**: inadmissibilidade do agravo se o agravado alegar.

(Em PJe a comunicação é automática em vários tribunais. Verificar regimento.)

## Efeito suspensivo / antecipado da tutela (CPC 1.019, I)

- **Suspensivo**: paralisa os efeitos da decisão agravada.
- **Antecipado**: o que a decisão negou, o relator concede.

Requisitos: probabilidade do direito + risco de dano grave.

## Honorários recursais (CPC 85 § 11)

- Sempre quando recurso desprovido em decisão final do agravo.

## Erros comuns

- Atacar decisão interlocutória **fora** do rol do art. 1.015 sem fundamentar Tema 988 STJ → não conhecimento.
- Não juntar peças obrigatórias do art. 1.017 → não conhecimento.
- Esquecer a comunicação em 3 dias ao juiz de origem (CPC 1.018) → inadmissibilidade.
- Não comprovar tempestividade — guia datada errada.
- Pedir efeito suspensivo sem demonstrar urgência.
- Confundir agravo de instrumento com agravo interno (CPC 1.021 — é contra decisão monocrática do relator) ou agravo em recurso especial/extraordinário (CPC 1.042).
- Apelar de decisão que cabia agravo (CPC 1.009 § 1º — recurso adesivo na apelação contra interlocutória sem agravo é admissível).

## Checklist

- [ ] Decisão interlocutória dentro do rol 1.015 ou Tema 988
- [ ] Tempestividade (15 dias úteis)
- [ ] Preparo recolhido
- [ ] Peças obrigatórias do CPC 1.017 juntadas
- [ ] Demonstração da urgência (se efeito suspensivo)
- [ ] Pedido específico (suspensivo, antecipado, mérito)
- [ ] Comunicação em 3 dias ao juiz de 1ª (CPC 1.018) — verificar PJe
- [ ] Razões fundamentadas (lei + jurisprudência)
- [ ] Honorários recursais
- [ ] Protocolo eletrônico no tribunal

## Referências

- CPC arts. 1.015-1.020 (agravo)
- CPC art. 1.017 (peças obrigatórias)
- CPC art. 1.018 (comunicação ao juízo)
- CPC art. 1.019 (poderes do relator)
- Tema 988 STJ — REsp 1.704.520 (taxatividade mitigada)
- Súmula 622 STJ — descabimento de agravo de instrumento contra decisão saneadora não enumerada (com mitigação Tema 988)
- Regimento Interno do TJ

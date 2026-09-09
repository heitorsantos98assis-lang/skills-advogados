---
name: skills-advogados-peticao-inicial-civel
description: "Estrutura petição inicial cível seguindo o art. 319 do CPC, com qualificação, fatos, fundamentos, pedido, valor da causa, provas e protocolização eletrônica (PJe, e-SAJ, Projudi)."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Claude, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Toda demanda cível (rito comum ou procedimentos especiais) ajuizada como autor. Esta skill é o esqueleto base — para tipos específicos use as skills correlatas (06 cobrança, 07 danos morais, 08 danos materiais, 09 revisional, 19 alimentos, etc.).

## Inputs necessários

1. Cliente (nome completo, CPF/CNPJ, RG, endereço, e-mail, profissão, estado civil)
2. Réu (mesmo nível de qualificação — investigar bem para citação)
3. Procuração assinada (CPC art. 105) — preferencialmente eletrônica (Lei 11.419/2006)
4. Documentos comprobatórios (contrato, NF, comprovantes, prints, laudos)
5. Pretensão concreta + valor estimado
6. Competência (territorial, material, funcional — CPC arts. 42-66)
7. Justiça gratuita (Lei 1.060/50 + CPC arts. 98-102) ou custas

## Estrutura (CPC art. 319)

```
EXMO. SR. JUIZ DE DIREITO DA __ª VARA CÍVEL DA COMARCA DE __________

[QUALIFICAÇÃO DAS PARTES]
__________ [autor], [nacionalidade], [estado civil], [profissão], inscrito no CPF/MF sob nº __________, RG nº __________, domiciliado em __________, e-mail __________, vem, por seu procurador signatário (procuração anexa), com fulcro nos arts. 318 e 319 do CPC, propor

AÇÃO __________ [tipo] [com pedido de tutela provisória, se for o caso]

em face de __________ [réu], CPF/CNPJ nº __________, com sede em __________, pelos fatos e fundamentos a seguir.

I — DOS FATOS
[Narrativa cronológica e clara dos fatos relevantes, com referência a documentos. Cada parágrafo deve trazer um ponto.]

II — DO DIREITO
2.1. [Tema/tese 1] — fundamentar com lei, doutrina, jurisprudência
2.2. [Tema 2]
2.3. [Tema 3]

III — DA TUTELA PROVISÓRIA [se houver]
3.1. Probabilidade do direito (CPC art. 300)
3.2. Perigo de dano ou risco ao resultado útil do processo
3.3. Pedido específico

IV — DOS PEDIDOS
Diante do exposto, requer:
a) A citação da parte ré, no endereço acima, para apresentar contestação no prazo legal sob pena de revelia;
b) [Pedido principal — descrever objetivamente]
c) [Pedidos secundários se houver]
d) A condenação da parte ré ao pagamento de custas, despesas processuais e honorários sucumbenciais (CPC art. 85);
e) A produção de todas as provas em direito admitidas, especialmente __________;
f) Os benefícios da gratuidade de justiça [se for o caso] ou o pagamento de custas iniciais conforme guia anexa.

V — DO VALOR DA CAUSA
Atribui-se à causa o valor de R$ __________ (CPC art. 291).

[Local], [data]

________________________
[Advogado] OAB/__ nº ______
[E-mail / contato]
```

## Requisitos materiais (CPC 319) — checklist

| Item | Onde |
|---|---|
| Juízo competente (foro) | Cabeçalho |
| Qualificação completa autor/réu | I |
| Fato + fundamentos jurídicos | I e II |
| Pedido com suas especificações | IV |
| Valor da causa | V |
| Provas com que pretende demonstrar | IV (e) |
| Opção pela audiência conciliatória (CPC 334) | IV (a) — pedir realização ou desinteresse |

## Tutela provisória (CPC arts. 294-311)

### Tutela de urgência (cautelar ou antecipada)
- **Probabilidade do direito** (fumus boni iuris)
- **Perigo de dano ou risco ao resultado útil** (periculum in mora)
- Pode ser concedida liminarmente, antes da contestação

### Tutela de evidência (CPC 311)
- Independe de urgência
- Quando: abuso processual, prova documental e tese firmada em recurso repetitivo, contrato de depósito, prova suficiente.

### Cuidados
- Caução pode ser exigida (CPC 300 §1º)
- Reversibilidade (CPC 300 §3º) — se concedida e depois revertida, autor responde pelos danos

## Valor da causa (CPC art. 292)

| Tipo de pedido | Valor |
|---|---|
| Cobrança | Soma do principal + juros vencidos + multa |
| Dano material/moral | Valor pretendido |
| Anulação | Valor do contrato/título |
| Despejo | 12 vezes o aluguel |
| Alimentos | 12 prestações pretendidas |
| Reintegração de posse | Valor do bem |
| Declaração de inexigibilidade | Valor do título contestado |

## Custas

- TJ varia por estado (1-2% do valor da causa, com piso e teto)
- Justiça gratuita: requerer no CPC art. 98 + declaração de hipossuficiência (Súmula 481 STJ — PJ pode também)

## Templates de pedidos típicos

### Cobrança (skill 06 detalha)

```
b) A condenação do réu ao pagamento da quantia de R$ __________, atualizada pela tabela do TJ desde __/__/____, acrescida de juros legais de 1% ao mês contados da citação, e multa contratual de __% prevista na cláusula __ do contrato anexo;
```

### Indenização por danos morais (skill 07)

```
b) A condenação do réu ao pagamento de indenização por danos morais no valor de R$ __________, ou conforme o prudente arbítrio do juízo (Súmula 326 STJ), com correção desde o arbitramento (Súmula 362 STJ) e juros de mora de 1% ao mês a partir do evento (Súmula 54 STJ — responsabilidade extracontratual) ou citação (responsabilidade contratual);
```

### Obrigação de fazer

```
b) A condenação do réu na obrigação de [descrever] no prazo de ___ dias, sob pena de multa diária de R$ __________ (astreinte — CPC art. 537), com determinação direta ao bloqueio em caso de descumprimento;
```

## Protocolização

| Tribunal | Sistema |
|---|---|
| TJSP, TJRJ, TJES | e-SAJ |
| TJMG, TJBA, TJPR (parte), STJ, STF | PJe |
| TJPR, TJTO, TJAM | Projudi |
| Federal | PJe |
| Trabalhista | PJe (TST/TRTs) |

Cada sistema tem requisitos: petição em PDF, documentos em PDF (max 10MB ou conforme o tribunal), assinatura digital com certificado ICP-Brasil.

## Erros comuns

- Endereço do réu desatualizado → cita por edital (atrasa o processo).
- Pedidos genéricos ("o que for de direito") → CPC 322 § 2º exige interpretação restritiva, mas pedidos vagos podem levar a inépcia.
- Esquecer pedido de citação → inépcia da inicial.
- Valor da causa incompatível (R$ 1.000 em ação que envolve R$ 1 mi) → tribunal pode determinar adequação.
- Faltar documento essencial (contrato, comprovante) — CPC 320: indispensáveis devem instruir a inicial.
- Pedir liminar sem provar urgência → indeferida.
- Foro errado → tribunal declina ou autor é prejudicado em prazo de prescrição.
- Não juntar procuração nos autos → indeferimento.

## Checklist

- [ ] Qualificação completa autor/réu
- [ ] Fatos descritos com clareza e cronologia
- [ ] Fundamentação jurídica robusta
- [ ] Pedido específico, claro e congruente
- [ ] Valor da causa correto (CPC 292)
- [ ] Provas anunciadas
- [ ] Documentos essenciais juntados
- [ ] Procuração anexa
- [ ] Custas pagas ou gratuidade requerida
- [ ] Audiência conciliatória: opção indicada
- [ ] Tutela provisória (se houver) com fumus + periculum
- [ ] Foro competente
- [ ] Protocolo eletrônico com OK do sistema

## Referências

- CPC (Lei 13.105/2015) arts. 318-321 (inicial), 292 (valor), 98-102 (gratuidade), 294-311 (tutela), 334 (audiência), 85 (sucumbência)
- Lei 1.060/1950 (gratuidade — parcialmente vigente)
- Lei 11.419/2006 (processo eletrônico)
- Súmulas STJ pertinentes (54, 326, 362, 481)
- Resolução CNJ 185/2013 (PJe)

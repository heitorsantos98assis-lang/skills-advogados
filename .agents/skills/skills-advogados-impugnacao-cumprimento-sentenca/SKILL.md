---
name: skills-advogados-impugnacao-cumprimento-sentenca
description: "Estrutura impugnação ao cumprimento de sentença (CPC 525) com matérias defensivas (excesso, prescrição, pagamento, ilegitimidade) e pedido de efeito suspensivo, em 15 dias."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Claude, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Devedor (executado) intimado em cumprimento de sentença (CPC 523). Prazo: **15 dias** após o decurso do prazo de pagamento (ou após a intimação, conforme procedimento), para opor impugnação. Não exige garantia (diferente dos embargos à execução fiscal — skill 32).

## Inputs necessários

1. Petição inicial de cumprimento (do credor)
2. Sentença e cálculos
3. Comprovação de pagamentos (se houver)
4. Documentos das matérias defensivas

## Matérias cabíveis (CPC 525 § 1º)

I. Falta ou nulidade da citação no processo originário, processado à revelia
II. Ilegitimidade de parte
III. Inexigibilidade ou inexequibilidade do título
IV. Penhora incorreta ou avaliação errônea
V. Excesso de execução ou cumulação indevida
VI. Incompetência absoluta ou relativa
VII. Qualquer causa modificativa ou extintiva da obrigação posterior à sentença (pagamento, novação, transação, prescrição superveniente, compensação)

## Estrutura

```
EXMO. SR. JUIZ DA __ª VARA __ DA COMARCA DE __________

Processo nº __________

Impugnante (Executado): __________

Vem, com fulcro no art. 525 do CPC, opor

IMPUGNAÇÃO AO CUMPRIMENTO DE SENTENÇA

I — DA TEMPESTIVIDADE
Intimação para pagamento em __/__/____. Prazo de 15 dias após o vencimento dos 15 dias do CPC 523 (=__/__/____). Termo final: __/__/____. Tempestiva.

II — DAS MATÉRIAS DEFENSIVAS

2.1. [Excesso de execução — quando aplicável]
   - Valor cobrado: R$ __________
   - Valor correto pelo cálculo do impugnante: R$ __________
   - Memória de cálculo refeita anexa
   - Causa do excesso: [erro de índice / data / fórmula]

2.2. [Pagamento parcial / total]
   - Comprovante de DARJ/depósito de R$ __________ em __/__/____
   - Pagamento integral / parcial demonstrado

2.3. [Prescrição da pretensão executiva]
   - Súmula 150 STF: prescrição superveniente possível
   - 3 ou 5 anos conforme título (Súm 503 STJ se cheque, 5 anos para outros títulos no cumprimento)
   - Cálculo do prazo: trânsito em julgado + ___ anos

2.4. [Inexequibilidade]
   - Título não líquido / não certo / não exigível
   - Sentença sem dispositivo claro

2.5. [Inexigibilidade — STF declarou inconstitucional norma fundamento]
   - CPC 525 § 12-15: inexigibilidade quando STF declara inconstitucional o fundamento da sentença

2.6. [Compensação com crédito do executado]
   - Crédito anterior do executado contra o exequente

III — DO EFEITO SUSPENSIVO (CPC 525 § 6º)
Pleiteia-se atribuição de efeito suspensivo, pois:
   - Garantia já realizada (penhora / depósito)
   - Probabilidade do direito do impugnante
   - Risco de dano grave em prosseguir

IV — DOS PEDIDOS
a) Recebimento com efeito suspensivo;
b) Acolhimento das matérias suscitadas;
c) Procedência para:
   c.1) Reduzir o valor da execução de R$ __________ para R$ __________
   c.2) Declarar o pagamento integral / parcial e extinguir o cumprimento
   c.3) Reconhecer prescrição
   c.4) Declarar inexigibilidade
d) Custas e honorários sucumbenciais à parte adversa.

V — PROVAS
- Documental anexa
- Pericial contábil (se cálculos)

[Local, data]
[Advogado] OAB
```

## Excesso de execução — atenção (CPC 525 § 4º)

Quando alegado excesso, **deve indicar o valor correto** e **juntar o cálculo respectivo**, sob pena de:
- Rejeição liminar quanto a essa matéria
- Mantém-se o valor pleiteado pelo exequente

## Efeito suspensivo (CPC 525 § 6º)

Requer:
- Garantia (penhora, depósito, fiança bancária, seguro)
- Probabilidade do direito (fundamento relevante)
- Risco de dano

## Inexigibilidade pós-STF (CPC 525 § 12-15)

Se sentença foi fundamentada em norma posteriormente declarada inconstitucional pelo STF (em controle concentrado ou difuso com efeito vinculante), a obrigação se torna inexigível. Prazo: 2 anos da decisão do STF (mesma do art. 535 § 5º).

## Erros comuns

- Não juntar cálculo refeito ao alegar excesso → rejeição.
- Esquecer prazo (15 dias após pagamento — discussão).
- Não pedir efeito suspensivo + garantia.
- Apresentar matéria de mérito já decidida na sentença (preclusão).
- Discutir matéria que cabia em apelação.
- Compensação sem comprovar liquidez do crédito do impugnante.

## Checklist

- [ ] Tempestividade (15 dias)
- [ ] Garantia se for pleitear efeito suspensivo
- [ ] Memória de cálculo refeita (excesso)
- [ ] Comprovação documental do pagamento (se houver)
- [ ] Matéria adequada ao art. 525 § 1º
- [ ] Pedido específico (redução, extinção)
- [ ] Honorários sucumbenciais
- [ ] Procuração

## Referências

- CPC arts. 525, 535, 833 (impenhorabilidade)
- Súmulas STJ 150, 503, 519
- Tema 547 STJ
- Lei 9.494/1997 (FP)

---
name: skills-advogados-acao-renovatoria-locacao
description: "Estrutura ação renovatória de locação não residencial (Lei 8.245 arts. 51-57) com requisitos, prazo decadencial específico, perícia para valor do aluguel renovado e cláusulas de renovação."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Claude, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Empresário/locatário comercial que quer **renovar** o contrato de locação contra a vontade do locador. Direito específico do "ponto comercial".

## Requisitos (Lei 8.245 art. 51)

1. **Contrato escrito** com prazo determinado
2. **Mínimo 5 anos** de contrato (somando renovações se forem ininterruptas)
3. **3 anos** ininterruptos de exploração do mesmo ramo no imóvel pelo locatário

## Prazo decadencial (art. 51 § 5º)

A ação deve ser proposta entre o **último ano e os 6 meses anteriores** ao fim do prazo do contrato.

Fora desse prazo: decadência.

## Inputs necessários

1. Contrato em vigor + alterações
2. Comprovação da continuidade do ramo (NFs, alvará, IRPJ)
3. Comprovação dos 5 anos (contratos / aditivos)
4. Avaliação do valor justo do aluguel para a nova locação
5. Indicação de fiador idôneo
6. Procuração

## Estrutura

```
EXMO. SR. JUIZ DA __ª VARA CÍVEL DA COMARCA DE __________

[LOCATÁRIO — empresa]

vem propor

AÇÃO RENOVATÓRIA DE LOCAÇÃO NÃO RESIDENCIAL

em face de [LOCADOR], com fundamento nos arts. 51 a 57 da Lei 8.245/91, pelos motivos a seguir.

I — DOS FATOS
1. As partes celebraram em __/__/____ contrato de locação não residencial do imóvel [endereço], com prazo determinado de __ meses, vencimento em __/__/____ (cópia anexa).
2. A autora explora no imóvel a atividade de __________ desde __/__/____, totalizando __ anos de continuidade no ramo.
3. Histórico contratual:
   - Contrato 1: de __/__/____ a __/__/____ (anexo)
   - Contrato 2: de __/__/____ a __/__/____
   ... totalizando __ anos de locação.

II — DOS REQUISITOS LEGAIS (Lei 8.245 art. 51)
2.1. Contrato escrito por prazo determinado (anexo)
2.2. Soma de prazos ≥ 5 anos: total de __ anos
2.3. Exploração do mesmo ramo por 3+ anos ininterruptos: comprovado por __________
2.4. Tempestividade (art. 51 § 5º): ação proposta no período entre o último ano e os 6 meses anteriores ao fim do contrato

III — DAS CONDIÇÕES PROPOSTAS
3.1. Aluguel: R$ __________ (valor real estimado, com possibilidade de perícia)
3.2. Prazo: __ meses
3.3. Reajuste: pelo IGPM/IPCA anual
3.4. Garantia: fiador __________ (CPF/RG, qualificação) ou seguro fiança ou caução de R$ __________
3.5. Demais cláusulas: nos termos do contrato vigente, com as adaptações necessárias

IV — DA INDICAÇÃO DE FIADOR
3.1. Nome: __________
3.2. CPF: __________
3.3. Renda: R$ __________
3.4. Patrimônio comprovado: __________
3.5. Termo de aceitação anexo

V — DOS PEDIDOS
a) Citação do réu;
b) Procedência para:
   b.1) Renovar o contrato de locação pelo prazo de __ meses, com vigência a partir de __/__/____;
   b.2) Fixar o aluguel em R$ __________ (ou conforme perícia judicial);
   b.3) Manter as demais cláusulas com as adaptações necessárias;
c) Em caso de defesa do réu sobre exceção de retomada (art. 52), discussão dos motivos invocados;
d) Custas e honorários sucumbenciais.

VI — DA PROVA
- Documental (contratos, NFs, alvará, IRPJ)
- Pericial: avaliação do aluguel real do imóvel
- Testemunhal: continuidade da atividade

VII — DO VALOR DA CAUSA
R$ __________ (CPC 292 II — 12 vezes o valor do aluguel proposto)
```

## Defesa do locador (art. 72)

Locador pode opor:
- Não preenchimento dos requisitos do art. 51
- Proposta inadequada de aluguel (perícia para fixar)
- Exceção de retomada (art. 52):
  I. Necessidade do imóvel para uso próprio (ou de cônjuge/ascendente/descendente)
  II. Reforma substancial autorizada por autoridade pública (que acresçam capacidade ou modifiquem natureza)
- Sublocador ofereceu proposta melhor (art. 72 V)

## Indenização ao locatário pela retomada (art. 52 § 3º, 53)

Se locador retomar para uso próprio, indeniza fundo de comércio (lucros cessantes, etc.) na conformidade dos arts. 52 § 3º e 53.

## Cuidados

### Soma dos prazos
- Contratos sucessivos do mesmo locatário no mesmo imóvel se somam (Súm 482 STJ — só somam contratos com mesmo locatário)
- Se houver troca de empresário: começa de novo

### Atividade idêntica
- Mudança de ramo após o início do contrato → quebra continuidade
- Sublocação para terceiro: questionável, depende do caso

### Fiador idôneo
- Renda mínima 3 vezes o aluguel proposto (jurisprudência)
- Patrimônio compatível
- Sem restrições creditícias

### Acordos paralelos
- Antes de chegar a juízo, frequente é conseguir negociar diretamente
- Mediação prévia é recomendada

## Erros comuns

- Perder o prazo decadencial (fora da janela 12-6 meses do fim).
- Não ter 5 anos de contrato (ou ter contratos sucessivos com pessoas diferentes).
- Mudar de ramo na metade do contrato — quebra continuidade.
- Não indicar fiador ou indicar inadequado.
- Pedido genérico (sem especificar aluguel proposto, prazo, garantia).
- Esquecer perícia avaliatória.
- Sublocador como autor sem comprovar concordância do locador original.

## Checklist

- [ ] Prazo de propositura (12-6 meses antes do fim) respeitado
- [ ] Contrato escrito por prazo determinado
- [ ] 5 anos de contrato (somando)
- [ ] 3 anos ininterruptos no mesmo ramo
- [ ] Aluguel proposto razoável (com perícia possível)
- [ ] Fiador idôneo + termo
- [ ] Prazo proposto
- [ ] Documentos comprobatórios da atividade
- [ ] Procuração
- [ ] Valor da causa: 12 × aluguel (CPC 292 II)

## Referências

- Lei 8.245/1991 arts. 51-57, 72
- Súmula 482 STJ
- Súmula 411 STJ (legitimidade ativa)
- CPC art. 292 II
- Tema 951 STJ (decadência)

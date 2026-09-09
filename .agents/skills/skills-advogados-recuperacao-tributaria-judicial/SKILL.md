---
name: skills-advogados-recuperacao-tributaria-judicial
description: "Estrutura ações de recuperação tributária com teses consolidadas (Tema 69, 1.067, 962, 1.135), via mandado de segurança ou ação ordinária, com pedido de compensação ou repetição."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Claude, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Empresa quer recuperar tributos pagos indevidamente nos últimos 5 anos (decadência), aplicando teses já firmadas pelo STF/STJ. Skill correlata: contadora 43.

## Inputs necessários

1. Apurações dos últimos 60 meses
2. EFD-Contribuições, EFD ICMS/IPI, ECD, ECF
3. Memória de cálculo refeita
4. Análise tributária preliminar com tese identificada
5. Procuração

## Principais teses

### 1. Exclusão do ICMS da base PIS/COFINS (Tema 69 STF)
- Crédito por 5 anos retroativos
- ICMS destacado na NF (Lei 14.592/2023 confirmou)
- Modulação: efeitos a partir de 15/03/2017 para ações ajuizadas após essa data; antes para quem já tinha ação

### 2. Exclusão do ISS da base PIS/COFINS (Tema 1.067 STF)
- STF reconheceu repercussão geral; aguardando julgamento definitivo (em 2024-2026)
- Tese vencedora aplicada por analogia em vários TRFs

### 3. Exclusão do PIS/COFINS da própria base (Tema 1.048 STF)
- STF: exclusão é cabível
- Recuperação por 5 anos

### 4. Exclusão da CPRB da própria base (Tema 1.135 STF)
- Análogo

### 5. Não incidência de IRPJ/CSLL sobre Selic (Tema 962 STF)
- Restituição de IR/CSLL sobre juros Selic em repetições
- Modulação (RE 1.063.187): fatos geradores até 30/09/2021

### 6. ICMS na base do PIS/COFINS — créditos
- Lei 14.592/2023 confirmou exclusão do ICMS também nas bases dos créditos

### 7. Ampliação do conceito de insumo (Tema 779 STJ)
- Direito a créditos de PIS/COFINS sobre insumos essenciais e relevantes
- Em matéria administrativa; pode ser provocado em juízo

### 8. ICMS / Substituição tributária recolhido a maior — Tema 201 STF
- Devolução do ICMS-ST quando preço final de venda é menor que a base presumida

### 9. Compensação de créditos com tributos administrados pela RFB
- Lei 13.670/2018, IN 2.055/2021
- Possibilidade de cruzamento

### 10. PIS/COFINS sobre receita de exportação direta — Tema 1.181 STF
- Amplo, regula a manutenção de créditos

## Vias judiciais

### a) Mandado de Segurança (Lei 12.016 — preventivo ou repressivo)
- Para reconhecimento do direito + autorização de compensação
- Súmula 213 STJ: "O MS constitui ação adequada para a declaração do direito à compensação tributária"
- Súmula 460 STJ: "É incabível o MS para convalidar compensação tributária realizada pelo contribuinte" — separar reconhecimento do direito × validação

### b) Ação ordinária (declaratória + repetição)
- Quando a tese demanda dilação probatória
- Restituição em dinheiro (precatório / RPV)
- Cumulação com declaração e condenação

### c) Ação rescisória
- Quando há decisão transitada em julgado contra o contribuinte e há mudança jurisprudencial

## Estrutura — MS recuperação Tema 69

```
EXMO. SR. JUIZ FEDERAL DA __ª VARA DE __________

[QUALIFICAÇÃO DO IMPETRANTE]

vem impetrar

MANDADO DE SEGURANÇA C/ PEDIDO LIMINAR

contra ato do Sr. Delegado da Receita Federal do Brasil em __________, pelas razões a seguir.

I — DOS FATOS
1. O impetrante é PJ no regime do Lucro Real (ou Presumido), tributado pelas contribuições PIS e COFINS.
2. Tem efetuado o recolhimento incluindo o ICMS destacado em NFs na base de cálculo.
3. O STF (RE 574.706, Tema 69) reconheceu que o ICMS destacado não compõe a base dessas contribuições, o que torna o recolhimento atual ilegal.

II — DO DIREITO LÍQUIDO E CERTO
2.1. Tema 69 STF — RE 574.706 — modulação 15/03/2017
2.2. Lei 14.592/2023 — consolidou a exclusão
2.3. IN RFB 2.121/2022 — ainda restritiva, gerando o constrangimento
2.4. Direito à compensação dos últimos 5 anos (Súm 213 STJ)

III — DOS PEDIDOS
a) Liminar para autorizar a exclusão do ICMS destacado da base de PIS/COFINS imediatamente, e suspender exigibilidade caso de cobrança em apuração futura;
b) Notificação da autoridade coatora;
c) Concessão definitiva da segurança para:
   c.1) Reconhecer o direito à exclusão do ICMS destacado da base de PIS/COFINS, presente e futuro
   c.2) Reconhecer o direito à compensação administrativa dos créditos pagos a maior nos últimos 5 anos, com aplicação da Selic e nos termos da Lei 9.430/96 + IN 2.055/21
   c.3) Reconhecer o crédito não atingido pela modulação do Tema 69 (15/03/2017) — ou somente a partir dessa data, conforme caso
d) Custas pela autoridade impetrada e pessoa jurídica interessada

IV — VALOR DA CAUSA: R$ __________ (estimativa do crédito 60 meses)
```

## Compensação administrativa (após sentença)

1. Habilitação prévia do crédito (IN 2.055/21 art. 100 e seguintes — exigível para crédito > R$ X)
2. Apresentação de PER/DCOMP por competência
3. Aproveitamento do crédito até a extinção
4. Atualização Selic (Lei 9.250/95 art. 39 § 4º)

## Honorários

- MS: Súm 105 STJ — sem honorários
- Ação ordinária: aplicação do CPC 85 § 3º (Fazenda) — escala progressiva

## Erros comuns

- Pedir compensação além do prazo decadencial (5 anos).
- Não pedir Selic.
- Compensação automática sem habilitação prévia (quando exigida).
- MS sem prova pré-constituída.
- Confundir tese — Tema 69 (PIS/COFINS) com Tema 1.067 (idem ISS).
- Não retificar SPEDs após sentença.
- Cobrança paralela: empresa em fiscalização ainda recebe auto.

## Checklist

- [ ] Tese aplicável identificada e fundamentada
- [ ] Período de 5 anos retroativos
- [ ] Memória de cálculo
- [ ] Atualização Selic
- [ ] Estratégia: MS x ação ordinária
- [ ] Habilitação prévia (se PER/DCOMP > limite)
- [ ] Procuração ativa
- [ ] Acompanhamento da compensação
- [ ] Retificação de SPEDs

## Referências

- Lei 9.430/1996, art. 39 § 4º (Selic)
- Lei 14.592/2023
- CTN arts. 165-168, 168 (decadência)
- IN RFB 2.055/2021 (compensação)
- IN RFB 2.121/2022 (PIS/COFINS)
- Súmulas STJ 213, 460
- Temas STF 69, 962, 1.048, 1.067, 1.135, 1.181

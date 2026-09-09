---
name: skills-advogados-mandado-seguranca-tributario
description: "Estrutura mandado de segurança tributário (Lei 12.016/2009) preventivo ou repressivo contra ato de autoridade coatora (RFB, Sefaz, Município), com prova pré-constituída e prazo decadencial de 120 dias."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Codex, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Para impugnar **ato concreto** ilegal ou abusivo de autoridade fiscal:
- Auto de infração / lançamento ilegal
- Negativa de CND
- Glosa de PER/DCOMP
- Cobrança de tributo discutido em regime de exceção
- Recusa em emitir certidão / em receber declaração
- Bloqueio em sistemas (SISBAJUD-fiscal, etc.)

Vantagens vs. ação ordinária:
- Sem custas em alguns casos
- Sumário (julgamento rápido)
- Prova pré-constituída — sem dilação

Desvantagens:
- Decadência de **120 dias** (Lei 12.016/2009 art. 23)
- Não cabe condenação em honorários sucumbenciais (Súm 105 STJ — para o impetrante; STF reafirmou)
- Sem dilação probatória — deve ser direito líquido e certo

## Inputs necessários

1. Identificação do impetrante (PF/PJ)
2. Autoridade coatora (RFB-DRF Subdelegada, Sefaz-Diretoria, Prefeitura)
3. Ato coator (auto, despacho, decisão administrativa)
4. Prova pré-constituída (documental anexa)
5. Procuração

## Estrutura

```
EXMO. SR. JUIZ DE DIREITO DA __ª VARA [Federal — se autoridade federal / Estadual de Fazenda / Cível]

[QUALIFICAÇÃO DO IMPETRANTE]

vem, com fundamento na CF art. 5º LXIX e na Lei 12.016/2009, impetrar

MANDADO DE SEGURANÇA C/ PEDIDO LIMINAR

contra ato do MM. __________ [autoridade coatora — Delegado da RFB / Auditor-Fiscal / Secretário da Fazenda], pelas razões a seguir.

I — DA AUTORIDADE COATORA E DA PESSOA JURÍDICA INTERESSADA
Autoridade coatora: __________
Pessoa jurídica de direito público: [União / Estado / Município] (Lei 12.016 art. 6º § 3º — informa interessada)

II — DO DIREITO LÍQUIDO E CERTO
A demanda apresenta direito líquido e certo, demonstrável documentalmente, sem necessidade de dilação probatória.

III — DOS FATOS
1. O impetrante é [contribuinte do tributo X]
2. A autoridade coatora praticou o seguinte ato em __/__/____: [descrever]
3. O ato é ilegal porque __________

IV — DO DIREITO
4.1. [Tese principal — citar lei, CF, súmula, jurisprudência]
4.2. [Súmulas STJ / STF / temas vinculantes aplicáveis]
4.3. Cabimento do MS: ato administrativo concreto ofensivo a direito líquido e certo (Lei 12.016 art. 1º)

V — DOS REQUISITOS PARA A LIMINAR (Lei 12.016 art. 7º III)
5.1. Fumus boni iuris: [demonstrar a ilegalidade com prova documental]
5.2. Periculum in mora: [risco de protesto, negativação, exigibilidade indevida, etc.]

VI — DOS PEDIDOS
a) Concessão da liminar para [suspender exigibilidade do crédito tributário (CTN 151 IV); permitir emissão de certidão; abster-se de protestar];
b) Notificação da autoridade coatora para prestar informações em 10 dias (Lei 12.016 art. 7º I);
c) Ciência ao Ministério Público (Lei 12.016 art. 12);
d) Ao final, concessão definitiva da segurança para [pedido específico];
e) Custas (em geral suportadas pelo impetrante e ressarcidas se vencedor) e ônus de sucumbência reduzido.

[Local], [data]
________________________
[Advogado] OAB/__ ______
```

## Espécies

### MS preventivo
- Antes da prática do ato (justo receio)
- Ex.: empresa quer adotar tese e teme autuação

### MS repressivo
- Após o ato concreto
- Decadencial de 120 dias do conhecimento do ato

## Suspensão da exigibilidade (CTN 151)

A liminar em MS suspende a exigibilidade do crédito (CTN 151 IV):
- Empresa pode emitir CND
- Não pode ser protestada
- Discussão judicial fica resolvida sem cobrança no curso

## Teses tributárias frequentes

### 1. Exclusão do ICMS da base PIS/COFINS (Tema 69 STF)
- RE 574.706, ICMS destacado não compõe base
- Já consolidado e contado no STF

### 2. Exclusão do ISS da base PIS/COFINS
- Tese análoga, em discussão no STF (Tema 1.067 STF)

### 3. Exclusão do PIS/COFINS da própria base
- Tema 1.048 STF

### 4. Exclusão da CPRB da própria base
- Tema 1.135 STF

### 5. Limitação do salário-educação a 5% do FPM
- Tese específica de empresas

### 6. Não incidência de IRPJ/CSLL sobre Selic em repetição de indébito
- Tema 962 STF

### 7. Tributação de software como serviço (LC 116) ou produto (ICMS)
- ADI 5.659 STF — software só ISS

### 8. Equiparação tributária de bonificações em mercadoria
- Tema 144 STJ — não compõe base

### 9. Reabertura de prazo para parcelamentos especiais
- Caso a caso

## Prova pré-constituída

- NFs, faturas, GIA, EFD, DCTFWeb, atos administrativos
- Sem testemunhas, sem perícia
- Se precisa de perícia → via inadequada, ajuizar ação ordinária

## Honorários

- Súmula 105 STJ: descabe condenação em honorários no MS para o impetrante
- Para o impetrado, idem (Súm 512 STF)

## Erros comuns

- MS sem prova pré-constituída → indeferimento da liminar.
- Esquecer prazo decadencial de 120 dias.
- Identificar autoridade coatora errada (delegado x auditor; secretário x diretor) → indeferimento ou correção.
- Pedir o que não cabe em MS (perda da função, indenização — ambos têm via própria).
- Não pedir liminar quando há urgência.
- Tributo já com inscrição em dívida ativa: discussão pela via dos embargos à execução fiscal (skill 32).

## Checklist

- [ ] Autoridade coatora correta e qualificada
- [ ] Prova pré-constituída anexa
- [ ] Tese com fundamento legal + jurisprudencial
- [ ] Pedido liminar com fumus + periculum
- [ ] Prazo de 120 dias respeitado (se repressivo)
- [ ] Ciência da pessoa jurídica de direito público
- [ ] Procuração ativa
- [ ] Foro competente
- [ ] Documentos numerados

## Referências

- Lei 12.016/2009 (MS)
- CF arts. 5º LXIX, 109 (vara federal)
- CTN art. 151 IV (suspensão exigibilidade)
- Súmulas STJ 213 (compensação), 273 (admissibilidade); STF 105 (honorários)
- Tema 69, 962, 1.048, 1.067, 1.135 STF
- ADI 5.659 STF (software ISS)

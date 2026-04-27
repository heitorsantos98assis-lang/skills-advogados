---
name: dissolucao-sociedade
description: Conduz dissolução total ou parcial de sociedade (CC 1.029-1.038, 1.077-1.085 + CPC 599-609), com apuração de haveres, retirada de sócio, exclusão judicial e liquidação.
allowed-tools: Read Grep Bash Edit Write
user-invocable: true
---

## Quando usar

### Dissolução parcial (mais comum)
- **Retirada do sócio** (CC 1.029) — direito de denúncia em sociedade por prazo indeterminado, com 60 dias de antecedência
- **Exclusão de sócio** (CC 1.030, 1.085) — falta grave, inadimplência
- **Falecimento de sócio** (CC 1.028) — herdeiros podem ou não ingressar
- **Quebra de affectio societatis** (jurisprudencial)

### Dissolução total
- Vencimento do prazo
- Consenso unânime
- Quebra do quorum mínimo (sociedade simples — CC 1.033)
- Falência
- Atividade ilícita ou inalcançabilidade do objeto

## Inputs necessários

1. Contrato social atualizado e alterações
2. Quadro societário e capital
3. Balanço patrimonial recente (data próxima da retirada/dissolução)
4. Comunicação prévia (CC 1.029)
5. Documentos de eventos (faltas graves se exclusão)
6. Procuração

## Apuração de haveres (CC 1.031 + CPC 604-606)

Sócio retirante / falecido / excluído tem direito ao valor de sua participação.

### Critérios

**Padrão (CC 1.031)**: balanço patrimonial **especial** apurado na data da resolução.

**Cláusula contratual**: pode prever critério próprio (ex.: valor patrimonial contábil, valor econômico via avaliação independente).

**Sem cláusula**:
- Balanço patrimonial: ativo (a valor de mercado) − passivo
- Multiplicar pela fração do retirante

**STJ inclina** pelo valor **econômico** (justo) quando o balanço contábil não reflete a realidade — incluindo:
- Reavaliação de ativos
- Goodwill
- Intangíveis (clientela, marca)

(Skill contadora 48 — valuation PME pode complementar)

## Pagamento

- Em 90 dias após apuração (regra padrão CC 1.031 § 2º)
- Cláusula contratual pode prever parcelamento

## Estrutura — ação de dissolução parcial (retirada)

```
EXMO. SR. JUIZ DA __ª VARA EMPRESARIAL / CÍVEL DA COMARCA DE __________

[SÓCIO RETIRANTE]

vem propor

AÇÃO DE DISSOLUÇÃO PARCIAL DE SOCIEDADE C/C APURAÇÃO DE HAVERES

em face de [SOCIEDADE] e [SÓCIOS REMANESCENTES], com base nos arts. 1.029 do CC e 599 do CPC, pelos motivos a seguir.

I — DOS FATOS
1. O autor é sócio da [SOCIEDADE], com __% das cotas.
2. A sociedade tem prazo indeterminado.
3. O autor exerceu direito de retirada mediante notificação extrajudicial em __/__/____ (doc. ___), com 60 dias de antecedência.
4. Os demais sócios concordam ou recusaram a apuração / não pagaram os haveres.

II — DO DIREITO
2.1. Direito de retirada (CC 1.029)
2.2. Apuração de haveres (CC 1.031)
2.3. Procedimento (CPC 599-609)

III — DOS PEDIDOS
a) Citação dos réus;
b) Acolhimento do pedido de dissolução parcial em relação ao autor, com efeitos a partir de __/__/____ (data da denúncia + 60 dias);
c) Apuração de haveres por balanço especial, considerando o valor justo dos ativos (com perícia contábil, se necessário);
d) Pagamento dos haveres ao autor em 90 dias após a sentença, com correção e juros desde a data de retirada;
e) Anotações na Junta Comercial e no contrato social;
f) Custas e honorários.

IV — DA PERÍCIA CONTÁBIL
Pleiteia-se nomeação de perito para elaborar balanço especial e laudo de avaliação patrimonial dos ativos, intangíveis e dívidas.

V — DO VALOR DA CAUSA
R$ __________ (estimativa do valor dos haveres a apurar)
```

## Procedimento (CPC 599-609)

1. Petição inicial — comunicar a sociedade
2. Citação da sociedade e dos demais sócios (todos os interessados)
3. Manifestação dos sócios e da sociedade
4. Sentença de dissolução parcial (ou improcedência)
5. **Liquidação por arbitramento**: nomeação de perito (CPC 605)
6. Laudo pericial
7. Sentença de homologação dos haveres
8. Pagamento + averbações

## Exclusão de sócio (CC 1.085)

- Sociedade limitada
- Falta grave: descumprimento contratual, ato ruinoso à sociedade
- Pelo voto majoritário (mais da metade do capital)
- Reunião / assembleia com convocação específica
- Com possibilidade de defesa prévia

Após exclusão administrativa, sócio excluído pode contestar judicialmente. Apuração de haveres como dissolução parcial.

## Sócio falecido (CC 1.028)

- Cabe aos herdeiros ingressar (se contrato permitir + acordo da maioria)
- Não havendo: dissolução parcial, com pagamento dos haveres ao espólio

## Quebra da affectio societatis (jurisprudencial)

Mesmo sem falta grave individualizada, jurisprudência reconhece direito de retirada quando há quebra da harmonia entre sócios. Impõe a dissolução parcial em vez de "obrigar" os sócios a permanecer juntos.

## Cuidados

### Cláusula de não-concorrência
- Para sócio que sai
- Geralmente limitada no tempo (até 5 anos) e no espaço

### Pagamento parcelado
- Cláusula contratual pode definir
- Sem cláusula: 90 dias

### Tributação
- Sócio PJ recebendo haveres: ganho de capital se valor > custo de aquisição
- Sócio PF: idem (skill contadora 50)
- Empresa: redução de capital ou conta de PL conforme caso

### Empresa após retirada
- Consolidar capital remanescente
- Atualizar contrato social
- Comunicar bancos, fornecedores, clientes

## Erros comuns

- Sociedade não citada (precisa ser parte na ação).
- Retirada sem comunicação prévia (60 dias).
- Apuração apenas pelo PL contábil quando há ativos subavaliados → STJ inclina pelo valor justo.
- Esquecer ações em curso, contingências (passivo) na apuração.
- Cláusula contratual que viole limitação legal (ex.: parcelamento abusivo, pagamento sem juros).
- Sócio remanescente alegando exclusão sem provas robustas.
- Atualização monetária e juros não pleiteados.

## Checklist

- [ ] Notificação prévia (60 dias)
- [ ] Documentos do contrato social
- [ ] Balanço atualizado
- [ ] Critério de apuração (cláusula ou padrão)
- [ ] Citação de sociedade + sócios
- [ ] Perícia para liquidação
- [ ] Cláusula de não-concorrência se aplicável
- [ ] Atualização monetária e juros
- [ ] Averbações Junta Comercial
- [ ] Tributação do ganho de capital

## Referências

- CC arts. 1.028-1.038, 1.077-1.085
- CPC arts. 599-609
- Lei 11.598/2007 (REDESIM)
- Lei 14.195/2021
- Súmulas STJ — apuração de haveres a valor de mercado (REsp 1.139.593, etc.)
- Súmula 256 STJ (sociedade limitada)

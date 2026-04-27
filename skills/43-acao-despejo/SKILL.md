---
name: acao-despejo
description: Estrutura ação de despejo (Lei 8.245/91 — Lei do Inquilinato) por falta de pagamento, denúncia vazia, denúncia cheia, infração contratual, com pedido de liminar e fiel depositário.
allowed-tools: Read Grep Bash Edit Write
user-invocable: true
---

## Quando usar

Locador querendo retomar imóvel locado. Hipóteses (Lei 8.245/91):
- **Falta de pagamento** (art. 9º III, 62) — aluguel ou encargos não pagos
- **Denúncia vazia / cheia** (art. 46-47) — fim do prazo do contrato
- **Infração contratual** (art. 9º II) — descumprimento de cláusula
- **Reformas urgentes** (art. 9º IV)
- **Uso próprio** ou de ascendente/descendente (art. 47 III)
- **Desfazimento da locação por construção** (art. 47 IV)

## Inputs necessários

1. Contrato de locação (com firma reconhecida ou registrado)
2. Comprovação dos aluguéis em atraso (planilha)
3. Notificação extrajudicial (em alguns casos)
4. Identificação dos fiadores (se houver)
5. Procuração

## Tipos de locação (Lei 8.245)

### Residencial (art. 46-47)
- Prazo igual ou superior a 30 meses: vencido, denúncia vazia
- Prazo inferior a 30 meses: prorrogado por prazo indeterminado, mas denúncia exige cumprimento de motivações específicas (5 anos de locação OU motivos do art. 47)

### Não residencial (art. 51-57)
- Comercial / industrial
- Renovatória possível (art. 51) se 5 anos de contrato escrito + por prazo determinado + 3 anos no ramo

### Por temporada (art. 48-50)
- Até 90 dias

## Estrutura — despejo por falta de pagamento

```
EXMO. SR. JUIZ DA __ª VARA CÍVEL DA COMARCA DE __________

[LOCADOR] (qualificação) vem propor

AÇÃO DE DESPEJO POR FALTA DE PAGAMENTO C/C COBRANÇA DE ALUGUÉIS

em face de [LOCATÁRIO] e [FIADORES — se houver, em litisconsórcio].

I — DOS FATOS
1. Em __/__/____ foi celebrado contrato de locação do imóvel [endereço] (cópia anexa), com aluguel mensal de R$ __________ e encargos de R$ __________
2. O locatário deixou de pagar:
   - Aluguel competência __/____ — R$ __________
   - Aluguel competência __/____ — R$ __________
   - Encargos: IPTU, condomínio: R$ __________
   Total atualizado até __/__/____ = R$ __________
3. Notificação extrajudicial enviada em __/__/____ (doc. ___) sem regularização.

II — DO DIREITO
2.1. Da falta de pagamento (Lei 8.245 art. 9º III)
2.2. Da liminar de despejo (art. 59 § 1º IX) com caução
2.3. Da cobrança de aluguéis e encargos
2.4. Da responsabilidade dos fiadores (Lei 8.245 art. 39)

III — DOS PEDIDOS

a) Concessão de LIMINAR DE DESPEJO (Lei 8.245 art. 59 § 1º IX), mediante prestação de caução não inferior a 3 aluguéis;

b) Citação do(s) réu(s) para purgar a mora ou contestar (em 15 dias);
   - Caso haja contestação sem purga: prosseguimento
   - Caso haja purga: extinção do despejo, prosseguimento da cobrança

c) Procedência para:
   c.1) Decretar o despejo do locatário do imóvel [endereço];
   c.2) Condenar o locatário e os fiadores, solidariamente, ao pagamento dos aluguéis e encargos vencidos e vincendos até a efetiva desocupação;
   c.3) Multa contratual de __% (cláusula __);
   c.4) Atualização monetária e juros de 1% a.m.;
   c.5) Custas e honorários (CPC 85 + Lei 8.245 art. 75);

d) Em caso de não desocupação voluntária após sentença, expedição de mandado de desocupação com força policial, no prazo de 30 dias;

e) Provas: documental (anexada) e testemunhal.

IV — DO VALOR DA CAUSA
R$ __________ (12 aluguéis — Lei 8.245 art. 58 III + atualizado)
```

## Purga da mora (art. 62)

O locatário pode evitar o despejo pagando integralmente os atrasados + multa + juros + honorários (10% sobre o valor) **uma única vez a cada 24 meses** (Lei 8.245 art. 62 § ún).

Importante: a purga **paralisa o despejo**, mas a cobrança prossegue se o réu não pagar tudo.

## Liminar de despejo (art. 59 § 1º)

Casos com liminar de **15 dias**:
I. Mútuo acordo (escrito, vintena prévia)
II. Disposição judicial em ação de revisão
III. Despejo em prazo certo por temporada (art. 48-50)
IV. Falência da pessoa jurídica locatária
V. Permanência do sublocatário após resilição da locação
VI. Falta de pagamento aluguel ou encargos vencidos a + 3 meses
VII. Extinção do contrato de trabalho que originou a locação
VIII. Necessidade urgente de obra ordenada por autoridade pública
IX. **Falta de pagamento + caução de 3 aluguéis** (mais usado na prática)

## Despejo por denúncia vazia / cheia

### Denúncia vazia (art. 46 § 2º)
Contrato com prazo ≥ 30 meses → vencido, locador pede sem fundamentar motivo. Notificação prévia de 30 dias.

### Denúncia cheia (art. 47)
Contratos com prazo < 30 meses, prorrogados por prazo indeterminado:
- Decurso de 5 anos da locação (art. 47 V)
- Uso próprio ou de ascendente/descendente (47 III)
- Demolição/construção (47 IV)

Notificação prévia de 30 dias antes do despejo.

## Renovatória (não residencial — art. 51)

Empresa com 5 anos de contrato + 3 anos no ramo: pode renovar mesmo contra a vontade do locador. Ação proposta entre o último ano e os 6 meses anteriores ao fim do contrato.

## Erros comuns

- Não notificar previamente (denúncia vazia precisa de aviso 30 dias).
- Liminar sem caução de 3 aluguéis → indeferida.
- Esquecer fiadores na inicial — depois é difícil incluí-los.
- Aluguel sem firma reconhecida → reduzida força executiva (mas continua válido como contrato).
- Despejo de imóvel comercial sem distinguir renovatória.
- Não pedir cobrança junto com despejo → necessário ajuizar segunda ação.

## Checklist

- [ ] Contrato de locação juntado
- [ ] Planilha de débitos atualizada
- [ ] Hipótese legal definida (falta pagamento, denúncia, infração)
- [ ] Notificação prévia (denúncia)
- [ ] Pedido de liminar com caução (falta pagamento)
- [ ] Fiadores em litisconsórcio
- [ ] Pedido de cobrança junto
- [ ] Foro: do imóvel (CPC 47)
- [ ] Custas / gratuidade
- [ ] Procuração

## Referências

- Lei 8.245/1991 (Locações)
- Lei 12.112/2009 (alterações)
- CPC arts. 47 (foro), 528-533 (cumprimento)
- Súmulas STJ 268, 442
- ITQ-486/STJ (admite caução em despejo)

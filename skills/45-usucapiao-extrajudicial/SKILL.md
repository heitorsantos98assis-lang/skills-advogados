---
name: 45-usucapiao-extrajudicial
description: "Conduz usucapião extrajudicial (Lei 13.465/2017 + Provimento CNJ 65/2017) em cartório de registro de imóveis, com ata notarial, planta georreferenciada, justo título e prescrição aquisitiva."
allowed-tools: Read Grep Bash Edit Write
---

## Quando usar

Aquisição da propriedade por **posse prolongada e mansa** (CC 1.238 e ss). A via extrajudicial (Lei 13.465/2017 introduziu o art. 216-A na Lei de Registros Públicos) é mais rápida e simples quando há **consenso** entre os interessados.

## Espécies de usucapião

| Tipo | Prazo | Requisitos | Base legal |
|---|---|---|---|
| **Extraordinária** | 15 anos (10 se moradia) | Posse contínua, mansa e pacífica | CC 1.238 |
| **Ordinária** | 10 anos (5 se imóvel adquirido por instrumento + moradia) | Posse + justo título + boa-fé | CC 1.242 |
| **Especial urbana** (CF 183) | 5 anos | Imóvel ≤ 250 m² em área urbana, moradia, sem outro imóvel | CC 1.240 |
| **Especial rural** (CF 191) | 5 anos | Imóvel ≤ 50ha, produção, moradia | CC 1.239 |
| **Familiar** (CC 1.240-A) | 2 anos | Cônjuge abandonado, imóvel até 250m², coabitação interrompida pelo abandono | Lei 12.424/2011 |

## Inputs necessários

1. Ata notarial com posse documentada (Lei 13.465 art. 216-A I)
2. Planta georreferenciada do imóvel + memorial descritivo (Lei 6.015 art. 213)
3. Certidões dos titulares anteriores (matrícula)
4. Documentos do requerente
5. Anuência expressa dos confinantes e dos titulares (Lei 13.465 art. 216-A II)
6. Justo título (se ordinária) — promessa de compra e venda, escritura defeituosa
7. Comprovação de posse (IPTU, contas de luz/água, declarações de testemunhas)
8. Procuração com poderes específicos

## Fluxo extrajudicial (Provimento CNJ 65/2017)

### 1. Preparação
- Levantar matrícula atualizada
- Identificar antigos proprietários e confinantes
- Mapeamento georreferenciado por engenheiro/agrimensor

### 2. Ata notarial (em tabelionato de notas)
- Tabelião colhe declarações + entrevista testemunhas
- Documenta posse mansa, contínua, pacífica
- Anexa documentos

### 3. Petição ao Cartório de Registro de Imóveis (CRI)
- Acompanhada de:
  - Ata notarial
  - Planta + memorial
  - Justo título (se houver)
  - Anuências dos titulares anteriores e confinantes
  - Certidões pessoais
  - Certidões negativas dos imóveis na vizinhança (algumas comarcas)

### 4. Análise pelo Oficial do CRI (15 dias)
- Notifica interessados que não anuíram (15 dias para impugnar)
- Notifica Fazenda (Federal, Estadual, Municipal — para defesa de eventual interesse)
- Publica edital (em alguns estados)

### 5. Conclusão
- Sem impugnações: registro da aquisição
- Com impugnações: encerramento extrajudicial → ajuizar ação judicial

## Estrutura — petição ao CRI

```
Ao Sr. Oficial do __º Cartório de Registro de Imóveis da Comarca de __________

Requerente: __________ (qualificação completa, com cônjuge se aplicável)

Vem requerer o reconhecimento de USUCAPIÃO EXTRAJUDICIAL com fundamento no art. 216-A da Lei 6.015/73 (Lei de Registros Públicos), introduzido pela Lei 13.465/2017, e Provimento CNJ 65/2017.

I — IDENTIFICAÇÃO DO IMÓVEL
Localização: __________
Matrícula: __________ (atualmente em nome de __________)
Área: __________ m² (urbano / rural)
Confinantes: __________ (nomes)

II — DA POSSE
2.1. Posse iniciada em __/__/____ (provas anexas)
2.2. Tempo de posse: __ anos, contínua, mansa, pacífica
2.3. Animus dominil (utilizar como dono, com ânimo)
2.4. [se ordinária] Justo título: __________ (promessa de compra e venda anexa)
2.5. [se ordinária] Boa-fé objetiva: ignorância do vício do título

III — DOS DOCUMENTOS ANEXOS
   a) Ata notarial (Tabelião do __º Tabelionato, em __/__/____)
   b) Planta georreferenciada e memorial descritivo (engenheiro __________ CREA __)
   c) Justo título (se aplicável)
   d) Anuências:
      - Titular(es) anterior(es): __________ (anuência anexa)
      - Confinante norte: __________ (anuência)
      - Confinante sul: __________ (anuência)
      - Confinante leste: __________ (anuência)
      - Confinante oeste: __________ (anuência)
   e) Certidões pessoais do requerente
   f) Comprovação de posse: contas, IPTU, fotos, declarações

IV — DA ESPÉCIE DE USUCAPIÃO
[Identificar com precisão: extraordinária / ordinária / especial urbana / especial rural / familiar]

V — DO PEDIDO
Requer-se o processamento do presente, com:
   a) Notificação dos interessados que não anuíram, se houver
   b) Notificação da Fazenda Federal, Estadual e Municipal
   c) Publicação de edital, conforme provimento estadual
   d) Ao final, registro da aquisição da propriedade plena em favor do requerente
   e) Abertura de matrícula, se necessário

[Local], [data]

________________________
[Advogado] OAB/__ ______
```

## Cuidados

### Anuências
- Se algum titular ou confinante não anuir → impossível extrajudicial
- Solução: ajuizar ação judicial (skill 46)

### Imóveis públicos
- Não usucapíveis (CF 183 § 3º, 191 § ún; Súm 340 STF)

### Bens em condomínio
- Cada coproprietário pode usucapir se houve possessio domínio de fato exclusiva

### Imóvel financiado / hipotecado
- Hipoteca persiste; usucapir extingue dívida do antigo proprietário ao hipotecante? Tema 1.114 STJ (em julgamento) — verificar

### Justo título
- Promessa de compra e venda
- Escritura sem registro
- Cessão de direitos com vícios

## Erros comuns

- Apresentar planta sem georreferenciamento (obrigatório).
- Não conseguir anuência de algum confinante → migrar para judicial.
- Imóvel rural sem CCIR.
- Confundir as espécies (especial urbana exige imóvel ≤ 250m² e único).
- Descontinuar a posse (saída do imóvel por longo período) — quebra do prazo.
- Usucapir bem que tem registro em nome de PJ pública (não cabe).
- Imóvel objeto de inventário aberto (entra no espólio — usucapião pode ser arguida no inventário).

## Checklist

- [ ] Ata notarial completa
- [ ] Planta + memorial georreferenciados
- [ ] Anuências (todos os interessados)
- [ ] Documentos pessoais
- [ ] Justo título (se ordinária)
- [ ] Comprovação de posse com testemunhas
- [ ] Identificação correta da espécie
- [ ] Pedido de notificação Fazendas
- [ ] Procuração com poderes específicos
- [ ] Honorários do tabelionato e do CRI

## Referências

- CC arts. 1.238-1.244, 1.240-A
- CF arts. 183, 191
- Lei 6.015/1973 art. 216-A (Lei de Registros Públicos)
- Lei 13.465/2017
- Provimento CNJ 65/2017
- Súmulas STJ 11, 73, 391; STF 340

---
name: 20-inventario-extrajudicial
description: "Conduz inventário e partilha extrajudicial em cartório (Lei 11.441/2007), aplicável quando há consenso entre herdeiros maiores e capazes, com cálculo de ITCMD, monte-mor e formal de partilha."
allowed-tools: Read Grep Bash Edit Write
---

## Quando usar

Falecimento (causa mortis) com:
- **Todos os herdeiros maiores e capazes** (com exceção de nascituro com decisão judicial)
- **Consenso** sobre partilha
- **Sem testamento** (Resolução CNJ 35/2007 antiga; com Lei 14.382/2022, há exceções: testamento revogado, expirado, ou todos os herdeiros e legatários maiores e capazes consentirem)
- Assistência de advogado obrigatória

Se houver litígio, menor/incapaz sem decisão prévia, ou testamento contestado: **inventário judicial** (skill 21).

## Inputs necessários

1. Certidão de óbito
2. Certidão de casamento + pacto antenupcial (se houver)
3. Documentos pessoais dos herdeiros e do cônjuge
4. Testamento e certidão de inexistência de testamento (CENSEC — Central de Testamentos)
5. Lista de bens com matrículas, certidões, valores
6. Certidões negativas: federal (RFB, FGTS), estaduais (ITCMD), municipais (IPTU)
7. CCIR (imóvel rural), CTC (cooperativa)
8. Contas bancárias e investimentos (extratos)
9. Empresa: contrato social, balanço, valuation
10. Procurações com poderes específicos

## Prazo

- Abertura do inventário: **60 dias** do óbito (CPC 611) — após esse prazo, multa estadual sobre o ITCMD em vários estados.
- Conclusão: **12 meses** (CPC 611) — pode ser prorrogado.

## Tributação — ITCMD (estadual)

Imposto de Transmissão Causa Mortis e Doação. Cada estado tem alíquota e base própria.

| Estado (exemplo) | Alíquota | Base |
|---|---|---|
| SP | 4% | Valor venal de referência ou de mercado |
| RJ | progressiva 4-8% | Valor venal |
| MG | progressiva 3-6% | Valor de mercado |
| RS | progressiva 3-6% | — |
| Outros | varia | varia |

- Pago **antes** da escritura
- Isenção/redução: cônjuge meeiro, herdeiro com baixa renda, único bem residencial até teto (varia por estado)
- Verificar se há decisão STF/STJ sobre progressividade do estado

## Estrutura — escritura pública

```
ESCRITURA PÚBLICA DE INVENTÁRIO E PARTILHA

Aos __ dias do mês de __ de 20__, perante mim, Tabelião do __º Tabelionato de Notas, comparecem:

[CÔNJUGE SOBREVIVENTE / MEEIRO] (qualificação)
[HERDEIRO 1] (qualificação)
[HERDEIRO 2] (qualificação)
... assistidos por adv. Dr. ____ OAB/__ ___

QUALIFICAÇÃO DO FALECIDO
__________ falecido em __/__/____, conforme certidão de óbito anexa.
Casado em regime __________ com __________ (cônjuge meeiro).

CLÁUSULA 1ª — DA HERANÇA
Os comparecentes declaram que são os únicos herdeiros, conforme certidão de inexistência de testamento (CENSEC), e que aceitam a herança e procedem à partilha consensual.

CLÁUSULA 2ª — DOS BENS (DESCRIÇÃO COMPLETA)
2.1. IMÓVEIS
   a) Apartamento [endereço], matrícula nº __ do __º CRI, valor de mercado R$ __________ (avaliação anexa)
   b) (...)
2.2. VEÍCULOS
   a) Veículo placa __, RENAVAM __, valor FIPE R$ __________
2.3. CONTAS BANCÁRIAS / INVESTIMENTOS
   a) Banco __ c/c __ saldo R$ __________
   b) (...)
2.4. AÇÕES / COTAS / PARTICIPAÇÕES
2.5. OUTROS

MONTE-MOR (TOTAL): R$ __________

CLÁUSULA 3ª — DA MEAÇÃO DO CÔNJUGE
Sendo regime __________, ao cônjuge meeiro cabe metade dos bens comuns: R$ __________ — atribuídos os seguintes bens: __________

CLÁUSULA 4ª — DAS DÍVIDAS DO ESPÓLIO
[Se houver]
- Empréstimo no Banco __ saldo R$ __________ — a ser quitado por __________

CLÁUSULA 5ª — DA PARTILHA DOS BENS DA HERANÇA
Após a meação, restam R$ __________ a serem partilhados entre os herdeiros nos termos da lei (sucessão legítima — CC 1.829):

5.1. Herdeiro 1 (filho): receberá __________ no valor de R$ __________
5.2. Herdeiro 2 (filho): receberá __________ no valor de R$ __________
... (na proporção igualitária entre filhos, salvo disposição contrária)

CLÁUSULA 6ª — DA TRIBUTAÇÃO
ITCMD pago conforme guia anexa: R$ __________
Recolhido em __/__/____.

CLÁUSULA 7ª — DAS DECLARAÇÕES E QUITAÇÕES
Os herdeiros se dão por inteiramente quitados quanto à herança e renunciam a qualquer direito ou ação futura.

CLÁUSULA 8ª — DAS AVERBAÇÕES E REGISTROS
Esta escritura serve como formal de partilha (Lei 11.441/2007) e será averbada nas matrículas dos imóveis e demais registros aplicáveis.

[Assinaturas]
[Tabelião]
```

## Sucessão legítima (CC 1.829)

Ordem de vocação hereditária:
1. **Descendentes** (filhos, netos) em concorrência com cônjuge sobrevivente (depende do regime de bens — CC 1.829 I)
2. **Ascendentes** (pais, avós) com cônjuge sobrevivente
3. **Cônjuge sobrevivente** sozinho (se não houver descendentes/ascendentes)
4. **Colaterais até 4º grau** (irmãos, tios, primos)

### Concorrência cônjuge × descendentes (CC 1.829 I) — REGRA COMPLEXA

Cônjuge **NÃO** concorre quando:
- Regime: comunhão universal (já tem meação)
- Regime: separação obrigatória (CC 1.641) — Súmula 377 STF aquestos comunicáveis
- Regime: comunhão parcial e o falecido não deixou bens particulares

Cônjuge **CONCORRE** quando:
- Regime: comunhão parcial e há bens particulares (concorre nos particulares)
- Regime: participação final dos aquestos
- Regime: separação convencional (Súmula 1.829 STJ — divergência; recentemente STJ admite concorrência)

União estável (CC 1.790 declarado inconstitucional) → STF Tema 809: aplica-se a regra do casamento (CC 1.829).

## Partilha desigual

Permitida (autonomia das partes), mas:
- ITCMD pode incidir sobre a parcela "doada" entre herdeiros (varia por estado)
- Documentar o motivo (ex.: cuidado prestado em vida — exonera tributo em alguns estados)

## Cessão de direitos hereditários

- Herdeiro pode ceder seus direitos antes da partilha (CC 1.793)
- Forma: escritura pública
- ITCMD na cessão entre herdeiros (não há) ou entre herdeiro e terceiro (ITBI/ITCMD sobre fração)

## Testamento + extrajudicial (Lei 14.382/2022)

Antes vedado. Agora possível em algumas hipóteses:
- Testamento caduco / inválido reconhecido judicialmente
- Todos os herdeiros e legatários maiores e capazes concordam

## Erros comuns

- Não pagar ITCMD em dia → multa estadual.
- Esquecer cônjuge concorrente quando há bens particulares (regime parcial).
- Imóvel sem matrícula atualizada — averbar morte é pré-requisito.
- Avaliação subdimensionada — Receita ou Estado glosa, exigindo complemento.
- Esquecer dívidas do espólio — herdeiros podem responder até o limite da herança.
- Bem omitido — sobrepartilha futura (CC 1.040), com possível ITCMD a maior.
- CENSEC não consultada — testamento esquecido aparece e invalida a partilha.

## Checklist

- [ ] Certidão de óbito + casamento + nascimentos dos herdeiros
- [ ] CENSEC: existência ou inexistência de testamento
- [ ] Inventário de bens com avaliações
- [ ] Inventário de dívidas
- [ ] Procurações com poderes específicos
- [ ] Certidões negativas (federal, estadual, municipal)
- [ ] Consultas a entidades (CRI, DETRAN, BACEN, CVM)
- [ ] ITCMD calculado e pago
- [ ] Escritura pública agendada e assinada
- [ ] Averbações em matrículas, RENAVAM, JUCESP (cotas), B3
- [ ] Encerramento de contas bancárias do falecido
- [ ] Distribuição de bens / declaração no IRPF dos herdeiros (Variação Patrimonial)

## Referências

- CC arts. 1.784-1.829, 1.829 (ordem sucessão), 1.790 (declarado inconstitucional Tema 809), 1.793, 1.831 (direito real habitação)
- CPC arts. 610-673
- Lei 11.441/2007
- Lei 14.382/2022
- Resolução CNJ 35/2007
- CENSEC (Central de Serviços Eletrônicos Compartilhados)
- Tema 809 STF
- Súmula 377 STF

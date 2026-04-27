---
name: acao-vicio-produto-servico
description: Estrutura ação por vício / defeito de produto ou serviço (CDC 12-25), com prazos decadenciais, escolha do consumidor (substituição, restituição, abatimento), responsabilidade objetiva e solidariedade da cadeia.
allowed-tools: Read Grep Bash Edit Write
user-invocable: true
---

## Quando usar

Produto/serviço apresenta:
- **Vício** (CDC 18-25): qualidade inadequada, quantidade falha, prazo de validade vencido, durabilidade reduzida
- **Defeito** (CDC 12-14): expõe consumidor a risco / acidente de consumo

## Distinção crítica

| | Vício (CDC 18-25) | Defeito (CDC 12-14) |
|---|---|---|
| O que é | Inadequação do produto/serviço | Defeito que causa acidente / dano |
| Responsabilidade | Solidária na cadeia (CDC 18 caput) | Fabricante (12); comerciante apenas se identificar (13) |
| Prazo decadencial | 30 dias (não duráveis) / 90 dias (duráveis) — CDC 26 | Prescrição de 5 anos — CDC 27 |
| Pretensão | Substituição, restituição, abatimento, conserto | Reparação dos danos (material + moral) |

## Inputs necessários

1. NF / contrato / comprovante de aquisição
2. Demonstração do vício/defeito (laudo, fotos, vídeos)
3. Histórico de tentativas de solução (SAC, ouvidoria, RMA)
4. Testemunhas eventuais
5. Comprovação dos danos (se houver acidente)

## Cadeia de responsabilidade

### Vício (CDC 18, 20)
**Solidária** entre fabricante, importador, distribuidor, comerciante.

### Defeito (CDC 12, 13, 14)
- Fabricante / produtor / construtor / importador
- Comerciante: apenas se não identificar fabricante OU não houver clareza
- Prestador de serviço: responsabilidade objetiva, salvo profissional liberal (responsabilidade subjetiva)

## Direitos do consumidor (CDC 18 § 1º — vício)

Quando vício não é sanado em 30 dias (ou prazo entre 7-180 dias se contratualmente reduzido/prorrogado):

a) **Substituição** do produto por outro da mesma espécie em perfeitas condições
b) **Restituição imediata** do valor pago + correção + perdas e danos
c) **Abatimento proporcional** do preço

Consumidor escolhe.

## Direitos por defeito (CDC 14)

- Reparação dos danos materiais (custos com hospital, perda)
- Indenização por danos morais
- Lucros cessantes
- Responsabilidade objetiva

## Estrutura

```
EXMO. SR. JUIZ DA __ª VARA CÍVEL DA COMARCA DE __________

[CONSUMIDOR] (qualificação)

vem propor

AÇÃO DE [SUBSTITUIÇÃO / RESTITUIÇÃO / INDENIZAÇÃO POR VÍCIO/DEFEITO] DE PRODUTO C/ DANOS

em face de [FORNECEDOR / FABRICANTE / IMPORTADOR / DISTRIBUIDOR — solidariamente]

I — DOS FATOS
1. Em __/__/____ o autor adquiriu __________ (NF nº ___, valor R$ __________).
2. O produto / serviço apresentou os seguintes vícios / defeitos:
   2.1. __________ [especificar]
   2.2. [...]
3. Em __/__/____ o autor levou ao SAC / loja / assistência técnica.
4. [Resposta: insatisfatória / não respondeu / 30 dias decorridos sem solução]

II — DO DIREITO

2.1. Da relação de consumo (CDC 2º, 3º; Súm 297 STJ)
2.2. [Vício — CDC 18-20] OU [Defeito — CDC 12-14]
2.3. Da solidariedade da cadeia (CDC 18 caput / 25 § 1º)
2.4. Do prazo de 30 dias para sanar (CDC 18 § 1º) — descumprido
2.5. Da responsabilidade objetiva
2.6. Do prazo decadencial respeitado (CDC 26 — 90 dias durável; ou prescrição CDC 27 — 5 anos defeito)
2.7. Da inversão do ônus da prova (CDC 6º VIII)

III — DOS PEDIDOS

a) Citação dos réus solidariamente;

b) Inversão do ônus da prova;

c) Procedência para:
   c.1) [VÍCIO]:
      ☐ Substituição do produto por outro idêntico em perfeitas condições, OU
      ☐ Restituição em dobro do valor pago, atualizado desde a aquisição, OU
      ☐ Abatimento proporcional de R$ __________
   c.2) Indenização por danos materiais: R$ __________ (gastos com idas, locação substituta, perda de uso)
   c.3) Indenização por danos morais: R$ __________ (transtornos significativos)
   c.4) Astreinte: multa diária de R$ __________ por descumprimento

d) Tutela de urgência (se cabível): substituição imediata enquanto se discute

e) Custas e honorários sucumbenciais

IV — DAS PROVAS
- Documental (NF, contratos, e-mails, prints)
- Pericial (técnica) sobre o vício/defeito
- Testemunhal

V — VALOR DA CAUSA: R$ __________
```

## Prazos decadenciais (CDC 26)

| Tipo | Prazo |
|---|---|
| Vício aparente / fácil constatação — produtos não duráveis | 30 dias |
| Vício aparente / fácil constatação — produtos duráveis | 90 dias |
| Vício oculto | A partir da evidência do vício, 30 ou 90 dias conforme tipo |
| Início | Da entrega do produto / término do serviço |

**Suspensão**: pela reclamação formal ou pela instauração de inquérito civil (CDC 26 § 2º).

## Prazos prescricionais (CDC 27)

- 5 anos da ciência do dano e da autoria, para reparação por **defeito** (CDC 12-14).

## Estratégias

### Substituição vs. restituição em dobro
- Tema 929 STJ: cobrança em má-fé → repetição em dobro
- Vício de produto: CDC 18 § 1º permite escolha
- Restituição em dobro do CDC 42 §ún aplica para cobrança indevida — não confundir

### Profissional liberal (CDC 14 § 4º)
- Médico, advogado, engenheiro, dentista
- Responsabilidade subjetiva (precisa provar culpa)
- Mas mantém os outros direitos do CDC

### Prazo de garantia legal vs. contratual
- Garantia legal: CDC 26
- Contratual: pode ser maior (geralmente 1 ano para eletrônicos, 5 anos para imóveis residenciais)
- Cumulam-se: contratual + legal

## Erros comuns

- Confundir vício com defeito.
- Acionar só o comerciante quando o defeito é do fabricante (em defeito, fabricante é o responsável principal).
- Esquecer prazo decadencial — não usa SAC para suspender (envie por escrito com AR ou pelo registrado).
- Pleitear apenas conserto quando 30 dias passaram → consumidor pode escolher substituição/restituição.
- Não pedir perícia em vício técnico complexo.
- Atender estritamente prazo de 30 dias da CDC sem demonstrar a impossibilidade prática.

## Checklist

- [ ] Vício ou defeito? Distinguir
- [ ] Prazo decadencial / prescricional respeitado
- [ ] Cadeia de responsabilidade identificada (solidária no vício)
- [ ] Tentativas extrajudiciais documentadas
- [ ] Escolha do consumidor explicitada
- [ ] Indenização por danos (se houver)
- [ ] Pericial requerida (se necessário)
- [ ] Astreinte
- [ ] Inversão do ônus
- [ ] Foro: domicílio do consumidor (CDC 101 I)

## Referências

- CDC arts. 12-25, 26-27, 39, 51, 101 I
- Súmulas STJ 297, 363, 477
- Tema 929 STJ (repetição em dobro)
- Resolução INMETRO (normas técnicas) — quando aplicável
- Lei 8.078/1990

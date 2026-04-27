---
name: partilha-bens
description: Conduz partilha de bens em divórcio, dissolução de união estável ou inventário (em ação autônoma — CPC 647), com avaliação, cálculo de tornas, ITCMD/ITBI e cláusulas de proteção.
allowed-tools: Read Grep Bash Edit Write
user-invocable: true
---

## Quando usar

Quando o casal/herdeiros precisa **dividir patrimônio comum**:
- Após divórcio decretado, antes ou depois de partilha
- Após dissolução de união estável
- Em inventário (com possível ação autônoma — CPC 647)
- Em sociedade que se dissolve

## Inputs necessários

1. Documento que estabelece o direito (sentença divórcio, escritura, inventário em curso)
2. Identificação dos bens com avaliação atualizada (avaliador, FIPE, IPTU, balanço de empresa)
3. Identificação das dívidas
4. Regime de bens / participação societária / quinhão hereditário
5. Tributos pendentes
6. Eventuais cláusulas restritivas em escrituras (incomunicabilidade, inalienabilidade — CC 1.911)

## Tipos de partilha

### Em divórcio (já decretado)
- Patrimônio dividido conforme regime de bens
- Comum ➝ 50% / 50% (em comunhão parcial / universal)

### Em união estável dissolvida
- Tema 809 STF: companheiros têm direitos sucessórios = casamento
- Partilha em vida: regime padrão (CC 1.725) é o da comunhão parcial; cada um leva o que lhe couber

### Em sucessão
- Conforme ordem de vocação (CC 1.829)
- Quinhão hereditário definido por inventário

## Cálculo da partilha

### 1. Levantar massa partilhável

```
Bens comuns/da herança..... R$ _________
(-) Dívidas comuns......... R$ _________
= Massa líquida............ R$ _________
```

### 2. Definir frações

```
Massa líquida × % cada parte = Quinhão
```

### 3. Atribuir bens específicos

Princípio da igualdade econômica. Quando os bens não são divisíveis igualmente:
- Quem recebe mais paga **torna** ao outro (em dinheiro)
- Ou um bem é vendido e o produto dividido

### 4. Tornas

```
Quinhão devido........ R$ _________
Bens recebidos........ R$ _________
Diferença a torna..... R$ _________
```

### 5. Tributação

| Situação | Tributo |
|---|---|
| Partilha igualitária | Sem ITBI/ITCMD |
| Bem atribuído sem torna ao cônjuge/herdeiro = quinhão | Sem tributo |
| Excesso = doação | ITCMD estadual |
| Bem atribuído acima do quinhão com torna em dinheiro | ITBI sobre o excesso |

## Bens problemáticos

### Empresas (cotas/ações)
- Avaliação por valuation (skill contadora 48)
- Direito de preferência dos sócios
- Cessão a terceiro pode exigir consentimento (CC 1.057)
- Apuração de haveres se um cônjuge sai (com base no patrimônio líquido da empresa)

### Imóveis financiados (SFH/SFI)
- Saldo devedor é dívida comum
- Quem fica com o imóvel assume a dívida (negociar com o banco a sub-rogação)
- Banco pode exigir liquidação se não há concordância

### Plano de previdência (PGBL/VGBL)
- STJ REsp 1.477.937: PGBL pode ser partilhado (depósito caracteriza poupança)
- VGBL: diverge — quando há renda explícita, mais protegido

### Investimentos / B3
- Conta conjunta: divisão simples
- Conta individual com origem comum: comum
- Alienar B3 pode gerar IR — verificar timing

### Veículo
- FIPE atualizada
- Multas e tributos em dia

## Estrutura — petição de partilha (em ação autônoma)

```
EXMO. SR. JUIZ DA __ª VARA DA FAMÍLIA E SUCESSÕES DA COMARCA DE __________

[QUALIFICAÇÃO DO REQUERENTE]

vem propor

AÇÃO DE PARTILHA DE BENS

em face de __________, com base no art. 647 do CPC.

I — DOS FATOS
1. As partes foram casadas pelo regime __ de __/__/____ a __/__/____, divorciadas conforme sentença / escritura (doc. ___).
2. Constituíram o patrimônio descrito a seguir, ainda não partilhado.

II — DA AVALIAÇÃO

II.1. IMÓVEL — apartamento [endereço]
   Matrícula: __ Avaliação: R$ _________ (laudo doc. ___)

II.2. VEÍCULO — placa __
   FIPE: R$ _________ (consulta doc. ___)

II.3. CONTAS BANCÁRIAS / INVESTIMENTOS
   Banco __ c/c __: saldo R$ _________ (extrato doc. ___)
   Aplicação __: R$ _________

II.4. EMPRESA — [nome], CNPJ __
   Cota: __% Valor R$ _________ (laudo de valuation doc. ___)

II.5. OUTROS

DÍVIDAS COMUNS
- Financiamento imóvel: saldo R$ _________
- (...)

MASSA PARTILHÁVEL: R$ _________ (50% para cada)

III — DA PROPOSTA DE PARTILHA
3.1. Imóvel apartamento: Requerente (com sub-rogação financiamento)
3.2. Veículo: Requerido
3.3. Cotas da empresa: 50% cada (mantém co-sócios) OU compra das cotas pelo Requerente com torna de R$ _________ ao Requerido
3.4. Saldo bancário: divisão 50% no momento da homologação

DIFERENÇA: Requerido a maior em R$ _________ → torna em dinheiro do Requerente

IV — DOS PEDIDOS
a) Citação do Requerido;
b) Designação de audiência de mediação (CPC 695);
c) Subsidiariamente, decisão judicial dirimindo eventuais divergências de avaliação (perícia);
d) Procedência para homologar a partilha conforme proposta (item III), com expedição do formal e mandado de averbação;
e) Custas e honorários (CPC 85);
f) Tutela de urgência: indisponibilidade de bens em risco de dilapidação (CPC 300).

V — DO VALOR DA CAUSA: R$ _________ (proveito econômico)
```

## Cláusulas de proteção

- **Cláusula penal** se descumprir torna em dinheiro
- **Hipoteca** sobre o bem em garantia da torna
- **Direito de preferência** caso o outro cônjuge venda o bem nos próximos __ anos
- **Não concorrência** (em divórcio empresarial)

## Erros comuns

- Avaliação desatualizada → uma das partes prejudicada.
- Ignorar bens "particulares" (heranças, doações) na partilha (não entram em comunhão parcial).
- Partilhar empresa em cotas iguais sem prever desligamento do "ex" do dia a dia → litígio futuro.
- Esquecer averbação no CRI / RENAVAM / JUCESP — propriedade ainda em condomínio.
- Bens em outro estado/país sem inventário/partilha lá.
- Tornas em dinheiro sem prazo / juros — vira dívida sem cobrança.
- ITCMD/ITBI esquecido em transferências desiguais.

## Checklist

- [ ] Patrimônio levantado e avaliado
- [ ] Dívidas levantadas
- [ ] Regime de bens / quinhão verificado
- [ ] Massa partilhável calculada
- [ ] Atribuição de bens equilibrada (com tornas)
- [ ] Cláusulas de proteção (cláusula penal, hipoteca)
- [ ] ITCMD/ITBI sobre excessos
- [ ] Sub-rogação financiamento negociada com banco
- [ ] Avaliação pericial em itens controvertidos
- [ ] Audiência de mediação
- [ ] Averbações em registros
- [ ] Formal de partilha

## Referências

- CC arts. 1.639-1.688 (regimes), 1.725 (união estável), 1.793, 1.829, 1.040
- CPC arts. 647 (autônoma), 695 (mediação)
- Tema 809 STF (união estável)
- Súmula 377 STF
- REsp 1.477.937 STJ (PGBL)

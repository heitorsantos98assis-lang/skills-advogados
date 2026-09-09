---
name: 09-acao-revisional-contrato
description: "Estrutura ação revisional de contrato bancário/financiamento/leasing/cartão de crédito com tese de juros abusivos, capitalização, cobrança de tarifas indevidas, comissão de permanência e refazimento da TR/CET."
allowed-tools: Read Grep Bash Edit Write
---

## Quando usar

Cliente sofre cobrança em contrato com instituição financeira / fornecedora e pretende:
- Reduzir juros remuneratórios (raro hoje — STJ Tema 27)
- Excluir capitalização ilegal (Súmula 539 STJ)
- Excluir tarifas indevidas (Tema 958 STJ)
- Repetir cobrança em dobro (CDC 42 §ún)
- Devolver valor pago a maior

## Inputs necessários

1. Contrato (cédula, financiamento, leasing, contrato bancário, cartão)
2. Extratos (faturas, demonstrativos)
3. Memória de cálculo do banco e cálculo alternativo
4. Aplicação do CDC: Tema 466 STJ — banco pode estar sob CDC ainda que se discuta juros (Súm 297 STJ confirma)
5. Cálculo refeito por contador / auxiliar técnico

## Teses comuns

### 1. Capitalização mensal sem pactuação expressa (Súmula 539 STJ)
- A capitalização anual era a regra; mensal só é admitida se **expressamente pactuada** (cláusula clara) e em contratos posteriores a 31/03/2000 (MP 1.963/2000 → Lei 10.931/2004).
- Verificação: Taxa anual ≠ Taxa mensal × 12 → houve capitalização.
- Pedido: refazer cálculo sem capitalização mensal.

### 2. Juros remuneratórios abusivos (Tema 27 STJ)
- STJ entende que juros pactuados em contratos bancários não estão limitados a 12% a.a.
- **Mas** podem ser revistos quando "manifestamente excessivos em relação à média de mercado" (REsp 1.061.530).
- **Estratégia**: comparar com a média do BACEN para a operação no mês de contratação. Diferença significativa (mais de 1,5x) sugere abusividade.

### 3. Comissão de permanência cumulada com correção / juros / multa
- Súmula 472 STJ: vedada cumulação. Tribunal exclui.

### 4. Tarifas indevidas (Tema 958 STJ — REsp 1.578.553)
- Lícitas: TC (tarifa de cadastro) na 1ª contratação; tarifa de avaliação de bem se efetivamente prestada; registro de contrato se efetivamente registrado; seguro proteção financeira (com escolha).
- Ilícitas: TAC (tarifa de abertura de crédito) duplicada, despesas administrativas genéricas.

### 5. Pagamento à seguradora (DPVAT, prestamista)
- Tema 972 STJ: válida desde que o consumidor possa escolher a seguradora.

### 6. CET (Custo Efetivo Total) divergente
- Resolução BACEN 3.517/2007: CET deve estar claramente expresso. Divergência grave gera nulidade da cláusula.

## Estrutura

```
[Cabeçalho — Vara Cível, foro do domicílio do consumidor — CDC 101 I; ou foro de eleição se válido]

Objeto: AÇÃO REVISIONAL DE CONTRATO BANCÁRIO C/C TUTELA DE URGÊNCIA E REPETIÇÃO DE INDÉBITO

I — DOS FATOS
1. As partes celebraram em __/__/____ contrato de [tipo] sob nº __________, no valor de R$ __________ a ser pago em __ parcelas de R$ __ cada (doc. ___).
2. Foram exigidas as seguintes tarifas: [listar].
3. A taxa de juros anunciada foi de __% a.m. / __% a.a., com CET de __% a.a. (doc. ___).
4. Após análise técnica (doc. ___), constatamos:
   a) Capitalização mensal sem pactuação expressa
   b) Juros acima da média BACEN para a operação
   c) Tarifas indevidas no valor total de R$ ____
   d) Comissão de permanência cumulada
5. Tentativas de solução extrajudicial: __________

II — DO DIREITO
2.1. Da aplicação do CDC (Súmula 297 STJ)
2.2. Da boa-fé objetiva e do dever de informação (CDC 4º, 6º III, 14, 39 V)
2.3. Das cláusulas abusivas (CDC 51)
2.4. Da capitalização (Súm 539 STJ)
2.5. Dos juros remuneratórios (Tema 27 STJ)
2.6. Das tarifas (Tema 958 STJ)
2.7. Da comissão de permanência (Súm 472 STJ)
2.8. Da repetição em dobro (CDC 42 § ún)

III — DA TUTELA DE URGÊNCIA
3.1. Probabilidade do direito (anexa: cálculo refeito comparando com média BACEN)
3.2. Perigo de dano (negativação iminente / busca e apreensão / parcelas insuportáveis)
3.3. Pedido específico: depósito mensal do valor incontroverso (parcela "limpa" de tarifas e capitalização) com manutenção do bem e abstenção de negativação

IV — DOS PEDIDOS
a) Concessão de tutela de urgência para que o autor deposite mensalmente em juízo o valor incontroverso de R$ ___, com manutenção da posse do bem e abstenção do réu de promover negativação ou busca e apreensão;
b) Citação do réu para contestar;
c) Procedência para:
   c.1) Declarar nula a capitalização mensal e refazer o cálculo (Súm 539);
   c.2) Excluir as tarifas indevidas no valor de R$ ___ (Tema 958);
   c.3) Excluir comissão de permanência cumulada (Súm 472);
   c.4) Reduzir juros remuneratórios à média de mercado BACEN (Tema 27);
   c.5) Determinar o refazimento da memória de cálculo pelo contador judicial;
   c.6) Repetir em dobro o que foi cobrado indevidamente (CDC 42 §ún);
d) Inversão do ônus da prova (CDC 6º VIII);
e) Custas e honorários (CPC 85);
f) Gratuidade (se aplicável).

V — DO VALOR DA CAUSA
R$ __________ (proveito econômico estimado)
```

## Tutela e bem dado em garantia

- Em **alienação fiduciária**, o STJ entende que o devedor pode depositar o valor incontroverso em juízo enquanto se discute → mantém o bem (Tema 1.062 STJ — fluxo).
- Cuidado: depositar valor irrisório → liminar negada e bem é apreendido.

## Erros comuns

- Pedir a redução dos juros sem comparar com a média BACEN — Tema 27 exige prova de abusividade.
- Esquecer pedido de tutela urgente quando há iminência de busca e apreensão.
- Não juntar memória de cálculo refeita — banco terá facilidade em refutar.
- Pedir a nulidade total do contrato quando é caso de revisão parcial.
- CDC vs. nãoCDC: cliente PJ usando o CDC sem demonstrar hipossuficiência ou destinação final do bem (Súm 363 STJ — pessoa jurídica pode ser consumidora).

## Checklist

- [ ] Contrato e extratos juntados
- [ ] Análise técnica (cálculo) anexa
- [ ] Comparação com média BACEN (caso queira reduzir juros)
- [ ] Capitalização verificada (Súm 539)
- [ ] Tarifas analisadas (Tema 958)
- [ ] Comissão de permanência (Súm 472)
- [ ] Tutela de urgência com depósito incontroverso
- [ ] Inversão do ônus da prova
- [ ] Repetição em dobro pleiteada (CDC 42 §ún)
- [ ] Custas / gratuidade

## Referências

- CDC arts. 4º, 6º III VIII, 14, 39 V, 42 §ún, 51, 101 I
- CC arts. 421, 422, 478 (resolução por onerosidade)
- Súmula 297 STJ — CDC e bancos
- Súmula 472 STJ — comissão de permanência
- Súmula 539 STJ — capitalização
- Tema 27 STJ — juros remuneratórios
- Tema 958 STJ — tarifas
- Tema 972 STJ — seguro
- Tema 1.062 STJ — depósito incontroverso
- Resolução BACEN 3.517/2007 — CET

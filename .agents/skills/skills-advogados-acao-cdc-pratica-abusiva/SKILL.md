---
name: skills-advogados-acao-cdc-pratica-abusiva
description: "Estrutura ação contra prática abusiva ou cláusula abusiva (CDC arts. 39, 51), com pedido de nulidade, indenização, repetição em dobro e tutela inibitória."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Codex, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Cliente exposto a:
- **Prática abusiva** (CDC 39): venda casada, recusa de venda, condicionar fornecimento ao consumo de outro produto, exigir vantagem manifestamente excessiva, valer-se da fraqueza ou ignorância
- **Cláusula contratual abusiva** (CDC 51): cláusulas que limitam direitos, transferem responsabilidade ao consumidor, são iníquas, abusivas
- **Publicidade enganosa ou abusiva** (CDC 36-37)

Pode ser ação **individual** ou **coletiva** (associação, MP, Defensoria).

## Inputs necessários

1. Contrato / publicidade / comportamento abusivo
2. Comprovação da prática (prints, gravações com aviso, NFs)
3. Documento da relação de consumo
4. Valor pretendido (indenização + nulidades)

## Práticas abusivas — CDC 39 (rol exemplificativo)

I. Venda casada
II. Recusa de atendimento
III. Enviar produto/serviço sem solicitação prévia (CDC 39 III + IV)
IV. Prevalecer-se de fraqueza/ignorância
V. Cobrar valor excessivo manifestamente
VI. Executar serviço sem autorização ou orçamento prévio
VII. Reaja para exigir ressarcimento
VIII. Colocar produto em desacordo com normas técnicas (NBR/INMETRO)
IX. Recusar venda à vista
X. Elevar preço sem justa causa
XI. Aplicar fórmula de cálculo abusiva
XII. Repassar custo de operação à consumidor (taxa de fornecimento de boleto, ex.: STJ jurisprudência consolidada como abusiva)

## Cláusulas abusivas — CDC 51 (rol exemplificativo)

I. Limitam responsabilidade do fornecedor
II. Subtraem opção de indenização ao consumidor
III. Transferem ao consumidor risco da atividade do fornecedor
IV. Estabelecem desvantagem exagerada
V. Permitem alteração unilateral do contrato
VI. Permitem ao fornecedor cancelar sem o consumidor
VII. Remetem decisão a opções unilaterais do fornecedor
VIII. Inversão do ônus da prova em prejuízo do consumidor
IX. Compelir uso de árbitro privado
X. Vedação a juízo arbitral conforme escolha do consumidor
XI. Cláusula resolutória ao livre arbítrio do fornecedor
XII. Renúncia a direitos
XIII. Possibilidade de variação unilateral do preço
XIV. Cláusula contrária à boa-fé / equidade

## Estrutura

```
EXMO. SR. JUIZ DA __ª VARA CÍVEL DA COMARCA DE __________

[CONSUMIDOR]

vem propor

AÇÃO DECLARATÓRIA DE NULIDADE DE CLÁUSULA ABUSIVA C/C INDENIZAÇÃO E REPETIÇÃO

em face de __________ [fornecedor], pelos motivos abaixo.

I — DOS FATOS
1. Em __/__/____ o autor contratou __________
2. O contrato/conduta apresenta as seguintes irregularidades:
   2.1. [Cláusula/Prática X]
3. [Eventos de aplicação da cláusula / efeitos no consumidor]

II — DO DIREITO

2.1. Aplicação do CDC (arts. 2º, 3º; Súm 297 STJ)

2.2. Da prática abusiva [CDC 39]
   - Hipótese: [identificar inciso aplicável]
   - Citações jurisprudenciais

2.3. Da cláusula abusiva [CDC 51]
   - Cláusula __ do contrato: [transcrever]
   - Enquadramento no inciso __ do art. 51
   - Nulidade de pleno direito (CDC 51 § 4º — pode ser declarada de ofício pelo juiz)

2.4. Da inversão do ônus da prova (CDC 6º VIII)

2.5. Da indenização e da repetição em dobro (CDC 42 § ún)

III — DA TUTELA DE URGÊNCIA
A urgência decorre da continuidade da prática [cobrança, fornecimento, recusa]. Há perigo de dano e probabilidade do direito.

Pleiteia-se:
   - Suspender imediatamente a cobrança / cláusula / prática
   - Astreinte de R$ __________ por descumprimento

IV — DOS PEDIDOS
a) Concessão da tutela de urgência;
b) Citação do réu;
c) Procedência para:
   c.1) Declarar nula a cláusula __ do contrato (CDC 51) ou a prática abusiva (CDC 39);
   c.2) Condenar a ré ao ressarcimento em dobro do valor cobrado em razão da cláusula/prática (CDC 42 § ún), corrigido desde cada cobrança;
   c.3) Condenar a ré ao pagamento de indenização por danos morais no valor de R$ __________;
   c.4) Determinar à ré que se abstenha de cobrar/aplicar tal cláusula/prática perante o autor;
   c.5) Em caso de descumprimento, multa diária de R$ __________;
d) Inversão do ônus da prova;
e) Custas e honorários sucumbenciais.

V — DOCUMENTOS
1. Contrato com cláusula abusiva
2. Comprovantes de cobrança / aplicação
3. Tentativas extrajudiciais
4. Eventual print/relato de prática

VI — VALOR DA CAUSA: R$ __________
```

## Casos paradigmáticos

### Tarifa de boleto (Tema 958 STJ — REsp 1.578.553)
- Cobrança de boleto **bancário** lícita; tarifa de avaliação de bem lícita
- Despesas administrativas/serviço de terceiros: ilícita
- Tarifa de cadastro: lícita apenas na primeira contratação

### Plano de saúde — limitação tempo internação (Súm 302 STJ)
- Cláusula nula

### Locação — cobrança de IPTU/condomínio do locatário sem previsão
- Súm 449 STJ aplicada

### Reajuste de mensalidade escolar acima do IPCA
- Lei 9.870/99: regula

### Multa de fidelização
- Limitada e com critério proporcional

### Cobrança de renovação automática
- CDC 52 § 2º: dever de informação clara

### "Calculadoras" e tarifas em financiamento
- Tema 958

## Tutela inibitória (CPC 497)

Pode-se pedir não só desfazer mas **proibir** prática futura.

```
Tutela inibitória: determine-se à ré abstenção definitiva da prática __, em todos os contratos atuais e futuros do mesmo modelo, sob pena de multa diária de R$ __________ (CPC 497).
```

## Erros comuns

- Pedir só nulidade sem repetição em dobro.
- Cláusula em contrato de adesão sem demonstrar abusividade objetiva.
- Inversão do ônus sem requerer formalmente.
- Astreinte sem prazo razoável.
- Esquecer pedido de obrigação de não fazer (manter abstenção futura).

## Checklist

- [ ] Cláusula ou prática especificamente identificada
- [ ] Enquadramento no CDC (39 ou 51)
- [ ] Documentos comprobatórios
- [ ] Pedido de nulidade
- [ ] Repetição em dobro
- [ ] Indenização moral (se houver)
- [ ] Inversão do ônus
- [ ] Tutela inibitória
- [ ] Astreinte
- [ ] Custas / gratuidade

## Referências

- CDC arts. 6º VIII, 36-37 (publicidade), 39 (práticas), 42 § ún, 49, 51 (cláusulas), 52
- CPC art. 497 (tutela inibitória)
- Tema 958 STJ
- Tema 929 STJ
- Súmulas STJ 297, 302, 449
- ADIs sobre cláusulas abusivas (vários temas STF)

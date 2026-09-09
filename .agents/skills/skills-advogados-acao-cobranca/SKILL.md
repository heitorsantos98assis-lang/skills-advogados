---
name: skills-advogados-acao-cobranca
description: "Estrutura ação de cobrança (rito comum) ou monitória (CPC 700-702) para créditos sem força executiva, com cálculo do principal + juros + multa, prazo prescricional e estratégia de penhora."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Codex, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

- **Ação de cobrança (rito comum)**: crédito sem título executivo (contrato verbal, e-mails, faturas, NFs simples)
- **Ação monitória (CPC 700-702)**: prova escrita sem eficácia executiva (cheque prescrito, NP sem aceite, contrato sem assinatura de testemunhas)
- **Execução** (não esta skill): título executivo extrajudicial — cheque dentro do prazo, duplicata aceita, contrato com 2 testemunhas, escritura pública

## Inputs necessários

1. Cliente credor (qualificação completa)
2. Devedor (qualificação — investigar bens para garantia)
3. Documentos do crédito: contratos, e-mails, NFs, comprovantes de entrega, prints, recibos
4. Histórico de inadimplência: data do vencimento, parcelas pagas, parcelas em aberto
5. Cláusulas contratuais: juros remuneratórios, juros de mora, multa, correção
6. Prazo prescricional (CC art. 206)
7. Tentativas amigáveis (provas de cobrança)

## Prazos prescricionais (CC art. 206) — principais

| Crédito | Prazo |
|---|---|
| Pretensão geral | 10 anos (CC 205) |
| Aluguel | 3 anos |
| Honorários profissionais | 5 anos (Súm 18 STJ — também varia) |
| Pretensão entre comerciantes (mercantil) | 3-5 anos (a depender) |
| Cobrança de NP / Cheque (executar) | 3 anos (após 6 meses do vencimento — pré-execução); para monitória: 5 anos do vencimento (Súmula 503 STJ — cheque sem força executiva) |
| Cobrança contra Fazenda Pública | 5 anos (Decreto 20.910/32) |
| Reparação civil | 3 anos |
| Pretensão para haver de seu segurado | 1 ano |

## Cálculo do crédito

```
Principal: R$ _________
+ Juros remuneratórios (cláusula contratual): __% a.m. desde __/__/____
+ Juros de mora: 1% a.m. desde a citação ou desde o vencimento (se contratado) (CC 406; Súm 54 STJ — extracontratual)
+ Multa contratual / cláusula penal: __%
+ Correção monetária pela tabela do TJ ou IPCA/INPC desde __/__/____
+ Honorários convencionais (se contrato prevê)
= Total atualizado: R$ _________
```

## Ação de cobrança — esqueleto

(Use a skill 01 Petição Inicial Cível como base)

```
[Cabeçalho — vara cível competente, geralmente foro do domicílio do réu — CPC 46]

Objeto: ação de COBRANÇA pelo rito comum

I — DOS FATOS
1. As partes celebraram em __/__/____ contrato de __________, no valor total de R$ __________ (doc. ___).
2. O réu deveria pagar __ parcelas de R$ __ cada, com vencimento __________. (doc. ___)
3. Pagas as parcelas __ a __, restou inadimplido o saldo de R$ __________. (doc. ___)
4. Apesar de notificações extrajudiciais (docs. __), o réu permanece inadimplente.

II — DO DIREITO
2.1. Da existência e exigibilidade do crédito (CC 313, 389, 397)
2.2. Dos encargos contratuais e legais
2.3. Da prescrição não consumada (citar dispositivo + datas)

III — DOS PEDIDOS
a) Citação do réu para pagar ou contestar;
b) Procedência para condenar o réu ao pagamento de R$ __________, atualizado pela tabela do TJ desde __/__/____, acrescido de juros legais de 1% a.m. da citação, multa contratual de __%, custas e honorários sucumbenciais (CPC 85).

IV — DO VALOR DA CAUSA: R$ __________
```

## Ação monitória (CPC 700-702)

Usada quando há **prova escrita** sem eficácia executiva.

```
Objeto: AÇÃO MONITÓRIA com fulcro nos arts. 700 e seguintes do CPC

I — DOS FATOS
[Mesma narrativa]

II — DA PROVA ESCRITA
A presente ação se apoia em [cheque prescrito / NP sem 2 testemunhas / contrato sem aceite / e-mails de confissão de dívida — descrever], que constitui prova escrita sem eficácia executiva, nos termos do art. 700 do CPC.

III — DOS PEDIDOS
a) Expedição do mandado monitório para que o réu, no prazo de 15 dias, pague a quantia de R$ __________ ou ofereça embargos monitórios;
b) Não havendo pagamento ou embargos, a constituição de pleno direito do título executivo judicial, nos termos do art. 701 § 2º do CPC;
c) Honorários iniciais de 5% sobre o valor (CPC 701 caput) reduzidos a __ se o réu pagar prontamente.
```

### Embargos monitórios
Se o réu opõe embargos, o procedimento se converte em ordinário.

### Não embargo, não pagamento
O mandado vira título executivo judicial automaticamente. Inicia-se cumprimento de sentença.

## Foro competente

- Regra geral: domicílio do réu (CPC 46)
- Cobrança fundada em contrato: foro do domicílio do réu OU do lugar onde se deve cumprir a obrigação
- Foro de eleição em contratos bancários/imobiliários: válido se pessoa jurídica capaz; CDC consumidor pode questionar

## Tutela de urgência (CPC 300)

- Arresto / penhora preventiva: provar perigo de o réu desfazer dos bens
- Bloqueio judicial via SISBAJUD
- Indisponibilidade

## Estratégia processual

1. **Pré-processual**: notificação extrajudicial, protesto de título, negativação (Serasa/SPC) — Súmula 572 STJ permite protesto de qualquer título.
2. **Conciliação**: audiência CPC 334.
3. **Cumprimento**: se procedente, fase executiva (skill 53).

## Erros comuns

- Pedir cobrança sem demonstrar prescrição não consumada.
- Apresentar contrato sem 2 testemunhas e ajuizar execução (correto: monitória).
- Não atualizar valor adequadamente (atualização desde a data correta).
- Esquecer juros de mora a partir do vencimento (se previsto contratualmente) ou da citação (se não).
- Usar foro de eleição em contrato consumidor — pode ser inválido (CDC 51 IV; Súmula 33 STJ).
- Não pedir bloqueio via SISBAJUD na cobrança quando há risco de inadimplência absoluta.

## Checklist

- [ ] Prescrição não consumada
- [ ] Crédito calculado e atualizado
- [ ] Documentos comprobatórios juntados
- [ ] Foro competente
- [ ] Notificação extrajudicial (recomendada)
- [ ] Petição estruturada (skill 01)
- [ ] Pedidos específicos (principal + juros + multa + sucumbência)
- [ ] Custas pagas
- [ ] Tentativa de conciliação
- [ ] Estratégia de execução pós-sentença mapeada

## Referências

- CC arts. 205-206 (prescrição), 313, 389, 397, 406 (mora)
- CPC arts. 318-321 (inicial), 46 (foro), 300 (tutela), 700-702 (monitória)
- Súmula 503 STJ (cheque na monitória)
- Súmula 572 STJ (protesto)
- Súmula 54 STJ (juros responsabilidade extracontratual)
- Lei 9.492/1997 (protesto de títulos)

---
name: skills-advogados-auxilio-doenca-recurso
description: "Conduz pedido / recurso / ação judicial de auxílio por incapacidade temporária (B31) ou acidentário (B91), aposentadoria por invalidez (B32) e auxílio-acidente (B94), com perícia INSS e judicial."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Codex, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Segurado com incapacidade laboral. Benefícios:
- **Auxílio por incapacidade temporária** (B31, antigo auxílio-doença) — Lei 8.213 art. 59
- **Auxílio-acidente** (B94) — após consolidação das lesões reduzindo a capacidade — art. 86
- **Aposentadoria por incapacidade permanente** (B32, antiga invalidez) — art. 42
- **Auxílio-doença acidentário** (B91) — quando origem é acidente de trabalho ou doença ocupacional

## Inputs necessários

1. Atestados, laudos médicos, exames, prontuários
2. CTPS + CNIS
3. CAT (Comunicação de Acidente de Trabalho — se acidentário)
4. Histórico de afastamentos
5. Procuração

## Carência (Lei 8.213 art. 25)

- Auxílio por incapacidade temporária: **12 contribuições mensais** (B31)
- Auxílio-doença acidentário (B91): **dispensa carência**
- Aposentadoria por invalidez (B32): 12 contribuições, salvo origem acidentária
- Auxílio-acidente (B94): dispensa carência (decorrente de acidente)

## Qualidade de segurado

Mantida durante:
- Período de pagamento normal
- Período de graça (12 meses após cessar; 24-36 meses para certas categorias)

## Pedido administrativo (Meu INSS)

1. Acessar Meu INSS
2. Solicitar benefício por incapacidade
3. Anexar atestado completo (CRM, dias previstos, CID)
4. Ater Atestmed (se < 180 dias) ou Perícia médica (> 180 dias / casos complexos)
5. Resposta em 45 dias (auxílio temporário) — Tema 1.066 STJ

## Atestmed (Atestado Médico)

- Sistema do INSS para análise documental
- Vigência: até 180 dias seguidos
- Se mais: perícia presencial

## Estrutura — ação judicial

```
EXMO. SR. JUIZ FEDERAL / DA __ª VARA PREVIDENCIÁRIA

[SEGURADO]

vem propor

AÇÃO DE CONCESSÃO / RESTABELECIMENTO DE [BENEFÍCIO]

em face do INSS

I — DOS FATOS
1. O autor é segurado do RGPS, com __ contribuições.
2. Em __/__/____ apresentou-se incapaz para o trabalho em razão de [doença / acidente] (laudos anexos).
3. Em __/__/____ requereu administrativamente — indeferido / cessado em __/__/____.
4. Quadro atual: incapacidade [temporária / permanente / parcial / total].

II — DO DIREITO
2.1. Da qualidade de segurado mantida (Lei 8.213 art. 15)
2.2. Da carência cumprida (ou dispensa por acidente)
2.3. Da incapacidade comprovada
2.4. Da espécie cabível: B31 / B91 / B32 / B94

III — DA TUTELA DE URGÊNCIA
A urgência decorre do caráter alimentar e da incapacidade comprovada. Pleiteia-se concessão imediata.

IV — DOS PEDIDOS
a) Tutela urgência: implantação imediata
b) Citação do INSS
c) Perícia médica judicial
d) Procedência para:
   d.1) Conceder/restabelecer o benefício (CID __ — incapacidade [...])
   d.2) DIB em __/__/____ (DER ou cessação)
   d.3) Pagamento de atrasados desde DER/cessação, com correção e juros
   d.4) Sucessivamente, em caso de aposentadoria por invalidez: conversão automática quando confirmada a permanência
e) Honorários, gratuidade
```

## Perícia médica judicial

- Perito médico nomeado pelo juízo
- Quesitos formulados pelas partes (quesitos do autor, INSS, do juízo)
- Pontos a explorar:
  - CID
  - Data do início da incapacidade (DII)
  - Início do efetivo afastamento
  - Tipo (temporária × permanente)
  - Total × parcial
  - Reabilitação possível?
  - Capacidade para outras atividades?
  - Origem: comum × acidentária

## Auxílio-acidente (B94)

- **Após** consolidação das lesões resultantes de acidente
- **Reduz a capacidade** para a atividade habitualmente exercida
- 50% do salário-de-benefício
- Acumulável com aposentadoria (Tema 555 STJ — alguns casos limitam)

## Aposentadoria por invalidez (B32)

- Incapacidade total e permanente
- Insuscetível de reabilitação
- 100% do salário-de-benefício (regra antiga) ou cálculo da Reforma (60% + 2% por ano > 20)

## Cessação e revisão (Lei 8.213 art. 60 § 9º)

- Auxílio por incapacidade temporária pós Lei 13.457/2017: prazo determinado de cessação (alta programada)
- Pedido de prorrogação até 15 dias antes do prazo
- Recurso administrativo (Junta de Recursos)

## Acidente de trabalho — específicos

- CAT em 24h da empresa (Lei 8.213 art. 22)
- Estabilidade no emprego: 12 meses após retorno (art. 118)
- Comunicação ao INSS

## Erros comuns

- Não juntar atestado completo (precisa CID, dias, CRM, assinatura).
- Esquecer de pedir prorrogação a tempo → cessa.
- Não pedir tutela urgência em caso de hipossuficiência.
- Não distinguir B31 (comum) de B91 (acidentário) — afeta carência e estabilidade.
- Pedir invalidez sem perícia robusta.
- Cumular benefícios indevidamente.

## Checklist

- [ ] Atestados / laudos médicos
- [ ] CNIS + CTPS
- [ ] Carência verificada
- [ ] DER / DIB / DCB
- [ ] CAT (se acidentário)
- [ ] Tutela urgência
- [ ] Perícia judicial requerida
- [ ] Atrasados
- [ ] Procuração e gratuidade

## Referências

- Lei 8.213/1991 arts. 15, 22, 25, 42, 59-63, 86, 118
- Lei 13.457/2017 (alta programada)
- Lei 14.331/2022 (BPC, alta processual)
- Decreto 3.048/1999
- Tema 555 STJ (cumulação)
- Tema 1.066 STJ (prazo administrativo)
- Súmulas TNU (várias)

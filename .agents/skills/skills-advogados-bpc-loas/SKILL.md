---
name: skills-advogados-bpc-loas
description: "Conduz pedido de BPC/LOAS (Lei 8.742/93 art. 20) para idoso 65+ ou pessoa com deficiência em situação de hipossuficiência (renda 1/4 SM família ou critério ampliado), com avaliação social e médica."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Codex, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

BPC (Benefício de Prestação Continuada) — LOAS:
- **Idoso ≥ 65 anos** sem condição de prover sustento
- **Pessoa com deficiência** (PcD) sem condição de prover sustento ou ter sustentado por sua família
- Renda mensal per capita do grupo familiar **inferior a 1/4 do SM** (regra geral)

Não é aposentadoria — é benefício assistencial. **Não dá direito a 13º** (Súm 9 TNU).

## Critério de renda

### Regra geral (Lei 8.742 art. 20 § 3º)
- 1/4 SM per capita

### Critério ampliado (jurisprudência STF Tema 27 + STJ)
- 1/2 SM per capita pode ser aceito quando há condições específicas que demonstram miserabilidade (gastos com saúde, deficiência, idoso)
- Análise caso a caso pela perícia social

### Exclusões da renda familiar
- O próprio BPC do idoso (Lei 13.146 EID)
- Bolsa Família / Auxílio Brasil
- Pensão alimentícia recebida apenas para o destinatário

## Inputs necessários

1. RG, CPF, comprovante de residência
2. CadÚnico atualizado
3. Composição familiar (todos no mesmo endereço)
4. Comprovação de renda de cada membro
5. Para PcD: laudos médicos, exames, atestados, CRM
6. Para idoso: certidão nascimento
7. Procuração

## Conceito de PcD (Lei 8.742 art. 20 § 2º; Lei 13.146 EID)

Pessoa com impedimento de longo prazo (≥ 2 anos):
- Físico
- Mental
- Intelectual
- Sensorial

Que, em interação com diversas barreiras, **possa obstruir sua participação plena e efetiva na sociedade em igualdade de condições**.

## Avaliação INSS

Inclui:
1. **Avaliação médica**: confirma a deficiência e o tempo
2. **Avaliação social**: assistente social analisa o ambiente, barreiras

## Estrutura — pedido administrativo (Meu INSS)

1. Acessar Meu INSS
2. Solicitar BPC (idoso ou PcD)
3. Anexar documentos
4. Aguardar agendamento de perícia médica (PcD) e social
5. INSS decide em 90 dias (Lei 9.784)

Se indeferido: ação judicial.

## Estrutura — ação judicial

```
EXMO. SR. JUIZ FEDERAL / DA __ª VARA PREVIDENCIÁRIA DE __________

[REQUERENTE — segurado]

vem propor

AÇÃO PARA CONCESSÃO DE BPC/LOAS

em face do INSS, com base na Lei 8.742/93.

I — DOS FATOS
1. O autor é [idoso com __ anos OU pessoa com deficiência]
2. Reside com __________ (composição familiar)
3. Renda familiar mensal: R$ __________ (per capita: R$ __________)
4. Em __/__/____ requereu administrativamente o BPC, indeferido sob argumento __________
5. [Para PcD: descrever o impedimento com base em laudos]

II — DO DIREITO
2.1. Do BPC/LOAS (Lei 8.742 art. 20)
2.2. Da hipossuficiência econômica
2.3. Da deficiência [se PcD] — Lei 13.146 EID
2.4. Do critério ampliado de renda (Tema 27 STF, REsp 1.355.052)

III — DA TUTELA DE URGÊNCIA
A urgência decorre da natureza alimentar do benefício. Há fumus boni iuris (laudos + composição familiar) e periculum (sustento imediato).

Pleiteia-se: implantação imediata.

IV — DOS PEDIDOS
a) Concessão da tutela urgência
b) Citação do INSS
c) Perícia médica e social
d) Procedência para:
   d.1) Conceder o BPC com DIB em __/__/____ (DER)
   d.2) Pagamento de atrasados desde DER com correção e juros
e) Honorários, gratuidade

V — VALOR DA CAUSA: 12 SM

VI — PROVAS: documental (anexa) + perícia médica + perícia social

[Local, data]
[Advogado] OAB
```

## Perícia em juízo

### Médica
- Perito do INSS ou independente nomeado
- Confirma a deficiência, classificação, prognóstico

### Social
- Assistente social do JFR / nomeado
- Visita domiciliar
- Avalia composição familiar, condições, gastos com saúde

## Cessação do BPC

- Idoso com mudança na renda (acima de 1/4 SM per capita)
- PcD: revisão a cada 2 anos para verificar se persiste
- Falecimento do beneficiário (não há reversão)
- Acúmulo com outros benefícios (vedado em geral)

## Migração para aposentadoria

- BPC pode migrar para aposentadoria por idade rural ou urbana se houver tempo de contribuição
- Atenção a vínculos antigos / contribuições facultativas

## Erros comuns

- Não esgotar via administrativa antes de ajuizar (Tema 350 STJ).
- Renda familiar mal calculada (incluir o BPC já recebido por outro membro — Lei 13.146 art. 20-A excluiu).
- Esquecer comprovação de gastos com saúde / deficiência (que afetam capacidade econômica).
- Confundir BPC com aposentadoria (BPC não tem 13º).
- PcD sem laudo médico recente.

## Checklist

- [ ] CadÚnico atualizado
- [ ] Composição familiar com renda comprovada
- [ ] Idade ≥ 65 OU laudos PcD
- [ ] DER administrativa
- [ ] Indeferimento administrativo
- [ ] Tutela urgência
- [ ] Perícia (médica + social)
- [ ] Atrasados desde DER
- [ ] Honorários
- [ ] Gratuidade

## Referências

- Lei 8.742/1993 (LOAS)
- Lei 13.146/2015 (EID)
- Decreto 6.214/2007 (regulamento BPC)
- Tema 27 STF (critério renda)
- Tema 350 STJ (prévio req)
- Súm 9 TNU (sem 13º)
- IN INSS 128/2022

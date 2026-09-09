---
name: skills-advogados-recuperacao-judicial-empresarial
description: "Estrutura petição inicial de recuperação judicial (Lei 11.101/2005 + alterações da Lei 14.112/2020), com plano, AGC, lista de credores, stay period e blindagem patrimonial."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Codex, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Empresa em crise econômico-financeira que pretende reorganizar dívidas e manter operação. Requisitos (Lei 11.101/2005 art. 48):
- Atividade regular há mais de **2 anos**
- Não ser falida (ou, se foi, com sentença extinta)
- Não ter obtido RJ nos últimos **5 anos**
- Não ter sido condenado por crime falimentar
- Pedido feito pelo próprio devedor, ou pelo cônjuge sobrevivente, herdeiros, etc.

## Inputs necessários

1. Última alteração contratual / estatuto e ata
2. Demonstrações contábeis (3 últimos exercícios + interim)
3. Lista nominal de credores com valores e classificação
4. Relação de bens e ativos (incluindo gravames)
5. Planilha de fluxo de caixa esperado
6. Ações em curso (cíveis, trabalhistas, fiscais)
7. Empregados ativos
8. Procuração com poderes específicos

## Tipos de RJ

### RJ ordinária (Lei 11.101 cap. III)
- Empresas médias e grandes
- Plano apresentado em 60 dias da decisão de processamento
- Assembleia Geral de Credores (AGC)

### RJ especial — ME e EPP (Lei 11.101 cap. III-A; LC 123/06)
- Empresas no Simples Nacional ME/EPP
- Procedimento simplificado
- Pagamento em 36 meses, parcelas iguais

## Estrutura — petição inicial

```
EXMO. SR. JUIZ DA __ª VARA DE FALÊNCIAS E RECUPERAÇÕES JUDICIAIS DA COMARCA DE __________

[QUALIFICAÇÃO DA REQUERENTE — empresa]

vem propor

RECUPERAÇÃO JUDICIAL

com fundamento na Lei 11.101/2005 e alterações.

I — DOS REQUISITOS (LEI 11.101 ART. 48)
1.1. Atividade regular há mais de 2 anos (CNPJ ativo desde __/__/____, com inscrição estadual e municipal)
1.2. Não há falência decretada
1.3. Não houve outro pedido de RJ nos últimos 5 anos
1.4. Não há condenação por crime falimentar

II — DA SITUAÇÃO ECONÔMICO-FINANCEIRA
2.1. Causas da crise:
   - [Pandemia / queda de mercado / inadimplência de cliente principal / aumento de custo / câmbio / etc.]
2.2. Quadro patrimonial atual:
   - Ativo: R$ __________
   - Passivo: R$ __________
   - Patrimônio líquido: R$ __________
2.3. Faturamento dos últimos 12 meses: R$ __________
2.4. Empregados: __ pessoas

III — DA LISTA DE CREDORES (Lei 11.101 art. 51 III)

| Credor | CNPJ/CPF | Classe | Valor (R$) | Vencimento |
|---|---|---|---|---|
| __ | __ | Trabalhista (até 150 SM por credor) | __ | __ |
| __ | __ | Garantia real | __ | __ |
| __ | __ | Quirografário | __ | __ |
| __ | __ | ME/EPP | __ | __ |

Total geral: R$ __________

[Detalhar conforme art. 51 da Lei]

IV — DOS DOCUMENTOS (Lei 11.101 art. 51)
   I. Causas da crise
   II. Demonstrações contábeis dos 3 últimos exercícios
   III. Relação nominal de credores (acima)
   IV. Relação de empregados
   V. Certidão da Junta Comercial (DRT)
   VI. Relação de bens particulares dos sócios
   VII. Extratos bancários atualizados
   VIII. Certidões dos cartórios de protestos
   IX. Relação de ações em curso

V — DOS PEDIDOS
a) O processamento da recuperação judicial (Lei 11.101 art. 52);
b) A nomeação do administrador judicial;
c) O **stay period** (Lei 11.101 art. 6º) — suspensão de execuções por 180 dias prorrogáveis;
d) A dispensa de apresentação de certidões negativas durante o procedimento (Súm 581 STJ);
e) A determinação para apresentação do plano em 60 dias;
f) A convocação da Assembleia Geral de Credores (AGC) quando necessária;
g) A dispensa do recolhimento de custas iniciais ou parcelamento;
h) A determinação para suspensão dos protestos cambiais;
i) A determinação à Junta Comercial / cartórios para anotação;
j) Eventual extensão dos efeitos a empresas do mesmo grupo econômico (consolidação substancial — em casos pertinentes);
k) A intimação do MP, das fazendas (federal, estadual, municipal) e demais interessados.

VI — DO VALOR DA CAUSA
R$ __________ (montante do passivo sujeito à RJ)

[Local], [data]
________________________
[Advogado] OAB/__ ______
```

## Classes de credores (Lei 11.101 art. 41)

| Classe | Descrição |
|---|---|
| I — Trabalhistas | Créditos decorrentes da legislação do trabalho ou acidente, até 150 SM. Excedente vai para quirografário |
| II — Garantia real | Créditos com garantia real (hipoteca, penhor, alienação fiduciária — observada a Súm 593 STJ) |
| III — Quirografários | Demais credores sem garantia ou privilégio especial |
| IV — ME e EPP | Pequenos credores (Lei 14.112/20 ampliou direitos) |

## Stay period (Lei 11.101 art. 6º)

- 180 dias suspensão de execuções e prazos prescricionais
- Prorrogação por mais 180 dias (excepcional)
- Não suspende:
  - Tributos (com exceção de algumas modalidades fiscais)
  - Créditos extraconcursais (gerados após a RJ)
  - ACC (adiantamento de contrato de câmbio)
  - Créditos com garantia fiduciária (Súm 593 STJ)

## Plano de recuperação (Lei 11.101 art. 50)

Apresentado em 60 dias contados da decisão de processamento. Pode prever:
- Concessão de prazos e descontos
- Cisão, incorporação, fusão, transformação
- Alteração societária
- Substituição de garantias
- Venda parcial dos bens
- Alongamento de prazos (até 60 meses para classe quirografária)
- Compensações
- DIP financing (financiamento durante o processo — Lei 14.112/20)

## AGC

- Convocada quando há objeção de credor
- Vota o plano (3 modalidades de aprovação)
- Cram down possível em hipóteses específicas (art. 58 § 1º)

## Cuidados especiais

### Crédito tributário
- Lei 14.112/20: parcelamento especial em até 120 meses para débitos com a Fazenda
- Súmula 581 STJ: certidões dispensadas durante a RJ

### Trabalhistas
- Pagamento em até 1 ano após a homologação do plano (Lei 11.101 art. 54)
- Rescisões sob a égide do plano: salários e verbas até 5 SM por empregado priorizadas

### DIP financing
- Captação de recursos durante o processo, com privilégio de pagamento

### Falência por descumprimento
- Inadimplemento das obrigações do plano por mais de 6 meses → falência (art. 73)

## Erros comuns

- RJ sem cumprir requisitos de art. 48 → indeferimento.
- Lista de credores incompleta → habilitação tardia.
- Plano superficial sem viabilidade econômica.
- Não identificar credor com garantia fiduciária (Súm 593 STJ).
- Esquecer ME/EPP como classe IV.
- Descumprir stay period — credor segue execução.
- Não convocar AGC quando devido.

## Checklist

- [ ] Requisitos do art. 48 cumpridos
- [ ] Documentos do art. 51 anexos
- [ ] Lista de credores por classe
- [ ] Demonstrações contábeis
- [ ] Stay period requerido
- [ ] Administrador judicial sugerido (se aceito)
- [ ] Honorários do administrador (Lei 11.101 art. 24)
- [ ] Procuração específica
- [ ] Custas / parcelamento

## Referências

- Lei 11.101/2005 (LRF)
- Lei 14.112/2020 (alterações)
- LC 123/2006 (RJ especial ME/EPP)
- Súmulas STJ 581, 593
- Tema 1.040 STF (DIP)
- Lei 13.043/2014 (parcelamento débitos fazendários)

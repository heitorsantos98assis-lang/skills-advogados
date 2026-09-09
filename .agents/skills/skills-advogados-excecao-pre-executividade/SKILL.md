---
name: skills-advogados-excecao-pre-executividade
description: "Estrutura exceção de pré-executividade (Súmula 393 STJ) sem garantia do juízo, para matérias de ordem pública (prescrição, decadência, nulidade da CDA, ilegitimidade), a qualquer tempo."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Codex, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Como **alternativa aos embargos à execução fiscal** (skill 32) quando não há condições de garantir o juízo (sem caixa, sem bem para penhorar) ou quando a matéria é manifestamente de ordem pública.

**Cabimento (Súm 393 STJ)**:
> "A exceção de pré-executividade é admissível na execução fiscal relativamente às matérias conhecíveis de ofício que não demandem dilação probatória."

## Características

| Embargos | Exceção PE |
|---|---|
| Exige garantia | NÃO exige |
| Prazo 30 dias | A qualquer tempo |
| Matéria ampla (mérito) | Apenas ordem pública sem dilação probatória |
| Suspensão da execução: condicional | Suspende durante análise da exceção (em geral) |
| Honorários sucumbenciais: sim | Sim, em caso de procedência |

## Inputs necessários

1. Cópia integral da execução fiscal (CDA, despacho, citação, eventuais penhoras)
2. Documentação que prove a matéria de ordem pública (sem necessidade de dilação)
3. Procuração

## Matérias cabíveis

### 1. Prescrição (CTN 174)
- Crédito constituído > 5 anos antes do ajuizamento da execução
- Documentos: CDA + data de constituição definitiva
- Não cabe se prescrição intercorrente exige análise probatória

### 2. Prescrição intercorrente (LEF art. 40 + Tema 568 STJ)
- Quando há documentos que demonstram inércia da Fazenda
- Pode ser via exceção se for clara

### 3. Decadência do lançamento (CTN 173 ou 150 § 4º)
- Auto após 5 anos do fato gerador / exercício seguinte
- Documental

### 4. Nulidade da CDA (CTN 202 + LEF 2º § 5º)
- Falta de elemento essencial (nome, valor, fundamento, termo, juros/multa, processo)
- Análise direta do título

### 5. Ilegitimidade passiva
- Devedor não é o real responsável (sócio sem vínculo, ex-sócio)
- Documental: contrato social atualizado, alteração registrada

### 6. Pagamento integral
- Comprovação documental

### 7. Imunidade ou isenção comprovada documentalmente

### 8. Inscrição em DA enquanto suspensa exigibilidade
- Decisão judicial / parcelamento ativo / depósito

### 9. Pagamento por parcelamento ativo
- Adesão regular não pode gerar execução

### 10. Bens impenhoráveis (CPC 833) já indicados pelo executado
- Casa de família (Lei 8.009/90), salário, etc.

## NÃO cabe via exceção

- Excesso de execução com necessidade de perícia
- Matéria de mérito complexo
- Compensação que demanda prova

## Estrutura

```
EXMO. SR. JUIZ DA __ª VARA DE EXECUÇÕES FISCAIS / FEDERAL DE __________

Processo de Execução Fiscal nº __________
Exequente: __________
Executado: __________

Vem, com fundamento na Súmula 393 do STJ, opor

EXCEÇÃO DE PRÉ-EXECUTIVIDADE

pelas razões a seguir.

I — DO CABIMENTO
A presente exceção tem cabimento (Súm 393 STJ) por se tratar de matéria de ordem pública, conhecível de ofício, sem necessidade de dilação probatória, demonstrada documentalmente.

II — DOS FATOS
1. Em __/__/____ foi ajuizada execução fiscal pela __________
2. Citação do executado em __/__/____
3. [Síntese do crédito objeto e da matéria suscitada]

III — DA MATÉRIA SUSCITADA

3.1. [Tese — exemplos]

   PRESCRIÇÃO (CTN 174)
   - Constituição definitiva em __/__/____
   - Ajuizamento em __/__/____ (após 5 anos)
   - Não houve causa interruptiva válida
   - Tema 1.073 STJ — interpretação restritiva
   - Pleiteia-se reconhecimento e extinção (CPC 487 II)

   OU

   NULIDADE DA CDA
   - A CDA anexa apresenta o seguinte vício:
     [...] não menciona o termo inicial dos juros
   - Violação ao art. 202 do CTN e LEF 2º § 5º
   - Inviável defesa adequada — direito ao contraditório (CF 5º LV)
   - Pleiteia-se nulidade da CDA e extinção da execução

3.2. [Demais teses, se cabíveis]

IV — DA SUSPENSÃO DA EXECUÇÃO
Pleiteia-se que, durante a análise desta exceção, sejam suspensos os atos de constrição, em razão da plausibilidade da matéria e da impossibilidade de prosseguimento sem o exame prévio.

V — DOS PEDIDOS
a) Conhecimento e processamento da exceção de pré-executividade;
b) Vista à Fazenda Pública para manifestação;
c) Acolhimento da matéria suscitada;
d) Extinção da execução fiscal (CPC 924 III ou 487 II conforme caso);
e) Levantamento de eventuais bloqueios (SISBAJUD, RENAJUD, indisponibilidade);
f) Condenação da Fazenda em honorários sucumbenciais (CPC 85 § 3º — escala progressiva);
g) Comunicação à PGFN/PGE/PGM para baixa do crédito.

[Local], [data]
________________________
[Advogado] OAB/__ ______
```

## Procedimento

1. Petição protocolada nos autos da execução
2. Vista à Fazenda Pública para impugnação (15 dias úteis em geral)
3. Decisão do juiz
   - Acolhimento: extinção da execução
   - Rejeição: agravo de instrumento (CPC 1.015)
   - Decisão de saneamento ou determinação de prova: pode descabê-la

## Erros comuns

- Apresentar matéria que demanda perícia → indeferimento por inadequação da via.
- Não juntar documentos comprobatórios desde a petição inicial.
- Esquecer pedido de honorários (Fazenda derrotada paga conforme CPC 85 § 3º).
- Apresentar exceção em vez de embargos quando há matéria de mérito ampla.
- Confundir exceção com manifestação simples nos autos — exceção tem natureza autônoma e gera ônus à Fazenda.

## Checklist

- [ ] Matéria de ordem pública sem dilação
- [ ] Documentação anexa
- [ ] Pedido de extinção
- [ ] Suspensão de bloqueios
- [ ] Honorários sucumbenciais
- [ ] Procuração

## Referências

- Súmula 393 STJ
- Lei 6.830/1980 (LEF)
- CTN arts. 173, 174, 202
- CPC arts. 487 II, 924, 1.015 (recurso de decisão), 85 § 3º
- Tema 568 STJ (prescrição intercorrente)
- Tema 1.073 STJ (causas interruptivas)

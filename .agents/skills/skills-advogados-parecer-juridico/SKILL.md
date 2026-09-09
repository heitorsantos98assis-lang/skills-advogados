---
name: skills-advogados-parecer-juridico
description: "Estrutura parecer jurídico para empresas, órgãos públicos ou particulares, com fatos, fundamentação, conclusão, recomendações e ponderação de riscos."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Claude, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Cliente pede análise técnica antes de tomar decisão ou ajuizar ação. Documento jurídico **opinativo** que orienta a decisão. Diferente da peça processual.

## Inputs necessários

1. Pergunta(s) específica(s) do cliente — clareza do questionamento
2. Fatos completos (com cronologia)
3. Documentos disponíveis (contratos, atos administrativos, correspondências)
4. Contexto da decisão (negócio, regulatório, tributário, etc.)
5. Prazo

## Estrutura padrão

```
PARECER JURÍDICO

Objeto: [resumo do tema]
Cliente: __________
Solicitação em: __/__/____
Parecer emitido em: __/__/____

I — DOS FATOS
[Narrativa cronológica e clara — não repetir documento por documento, mas sintetizar]

II — DAS QUESTÕES SUSCITADAS
1. [Pergunta 1]
2. [Pergunta 2]
3. [Pergunta 3]

III — DA FUNDAMENTAÇÃO

3.1. Quanto à questão 1
   3.1.1. Marco normativo
      - Lei __, art. __
      - Decreto __, regulamento ITGN
      - Convenção/tratado, se aplicável
   3.1.2. Doutrina
      - Citações de doutrinadores relevantes
   3.1.3. Jurisprudência
      - STF/STJ/Tribunais — temas, súmulas, acórdãos
   3.1.4. Análise
      - Aplicação ao caso concreto
      - Fragilidades e fortalezas

3.2. Quanto à questão 2
   [...]

3.3. Quanto à questão 3
   [...]

IV — DA PONDERAÇÃO DE RISCOS
4.1. Cenário favorável ao cliente — probabilidade ___%
4.2. Cenário desfavorável — probabilidade ___%
4.3. Riscos colaterais (tributário, reputacional, regulatório)
4.4. Cenários alternativos (negociação, mediação, arbitragem)

V — DA CONCLUSÃO

À luz do exposto, em resposta às questões formuladas:

1. Quanto à questão 1: __________
   Recomenda-se: __________

2. Quanto à questão 2: __________
   Recomenda-se: __________

3. Quanto à questão 3: __________
   Recomenda-se: __________

VI — DAS RECOMENDAÇÕES PRÁTICAS
- [Ação 1]
- [Ação 2]
- [Documento a produzir]
- [Cronograma]

VII — RESERVA E LIMITES DESTE PARECER
- Este parecer baseia-se nos fatos e documentos apresentados.
- Eventual surgimento de fato/documento novo pode alterar a conclusão.
- Não constitui garantia de resultado em eventual demanda.
- Análise considera a legislação e jurisprudência vigentes em [data].

[Local], [data]

________________________
[Advogado responsável] OAB/__ ______
```

## Tipos comuns

### 1. Parecer pré-contratual
- Análise de minuta de contrato
- Riscos de cláusulas
- Sugestão de redação

### 2. Parecer de viabilidade
- Antes de ajuizar uma ação
- Probabilidade de sucesso
- Custos e prazos

### 3. Parecer regulatório
- Antes de adotar prática (publicidade, lançamento de produto)
- Conformidade legal/regulatória

### 4. Parecer tributário
- Tese aplicável
- Risco de autuação
- Vantagens fiscais

### 5. Parecer trabalhista
- Política de RH
- Risco de pejotização
- Conformidade com CCT

### 6. Parecer societário
- Operação de M&A
- Reestruturação
- Sucessão familiar

### 7. Parecer LGPD / proteção de dados
- Política de privacidade
- Tratamento de dados sensíveis
- Compliance

## Cuidados

### Linguagem
- Técnica mas acessível
- Evitar verborragia jurídica
- Conclusão em linguagem direta

### Imparcialidade técnica
- Não defender; **orientar**
- Mostrar cenários
- Quantificar risco quando possível

### Citações
- Sempre confirmar a fonte
- Não citar súmula cancelada
- Indicar data da consulta

### Limitações
- Sempre incluir reserva (item VII)
- Esclarecer escopo
- Definir prazo de validade da análise

## Honorários

- Por hora: R$ varia (em cidades maiores: R$ 400-1500/h em escritórios médios)
- Fixo: definir escopo claro
- Tabela OAB local pode ser referência

## Modelo — parecer curto (síntese)

Para questões simples:

```
MEMORANDO JURÍDICO

Para: [Cliente]
De: [Advogado] OAB
Data: __/__/____
Assunto: [tema]

I. CONTEXTO
[2-3 parágrafos]

II. ANÁLISE
[3-5 parágrafos com fundamentação concisa]

III. CONCLUSÃO E RECOMENDAÇÃO
[Resposta direta]

[Assinatura]
```

## Erros comuns

- Parecer sem conclusão clara — cliente não sabe o que fazer.
- Repetir documentos sem síntese.
- Citar lei sem aplicar ao caso.
- Não quantificar risco quando viável.
- Esquecer reserva (item VII) — pode gerar responsabilização.
- Linguagem inacessível ao cliente leigo.
- Não datar o parecer (vinculação à legislação vigente naquele momento).

## Checklist

- [ ] Pergunta específica do cliente clara
- [ ] Fatos sintetizados
- [ ] Marco normativo correto e atualizado
- [ ] Doutrina relevante
- [ ] Jurisprudência (precedentes vinculantes)
- [ ] Aplicação ao caso concreto
- [ ] Ponderação de riscos
- [ ] Conclusão objetiva
- [ ] Recomendações práticas
- [ ] Reserva e limites
- [ ] Data e assinatura

## Referências

- Estatuto da OAB (Lei 8.906/94)
- Código de Ética e Disciplina da OAB
- Boa prática (publicações da OAB e doutrina)

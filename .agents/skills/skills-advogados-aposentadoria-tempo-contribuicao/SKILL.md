---
name: skills-advogados-aposentadoria-tempo-contribuicao
description: "Conduz aposentadoria por tempo de contribuição (regras de transição EC 103/2019), com cálculo do tempo, salário-de-benefício, fator previdenciário, regra do 25/30/35 anos e regras de transição."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Claude, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Segurado do RGPS (INSS) que pretende se aposentar por tempo de contribuição. **A aposentadoria por tempo de contribuição "pura" foi extinta em 13/11/2019 pela EC 103/2019**. Hoje, somente regras de **transição** (5 modalidades) ou aposentadoria por idade.

## Regras de transição da EC 103/2019

### 1. Pedágio de 50% (art. 17 EC 103)
Quem em 13/11/2019 estava a até 2 anos de completar tempo (35H/30M):
- Pedágio: 50% do tempo que faltava
- Sem idade mínima
- Cálculo: média de todas as contribuições × fator previdenciário

### 2. Idade Progressiva (art. 16 EC 103)
- Tempo: 35H/30M
- Idade mínima crescente: 61H6m/56M6m (2020), aumenta 6 meses por ano até 65H/62M (em 2031H/2033M)
- Para 2026: ≥ 64H/59M (verificar tabela)
- Cálculo: 60% da média + 2% por ano que exceder 20H/15M

### 3. Pedágio de 100% (art. 20 EC 103)
- Tempo: 35H/30M + pedágio 100% do tempo que faltava
- Idade mínima: 60H/57M
- Cálculo: 100% da média (sem fator)

### 4. Pontos (art. 15 EC 103)
- 35H/30M de tempo + soma idade + tempo
- Pontos crescentes: 96H/86M (2020), aumenta 1 ponto por ano até 105H/100M (2028H/2033M)
- Para 2026: ≥ 102H/92M (verificar)
- Cálculo: 60% + 2% por ano > 20H/15M

### 5. Idade Mínima (art. 18 EC 103) — para idade
- 65 anos H, 62 anos M, 15 anos contribuição (na data da transição) com adição de 6 meses ao ano até atingir o requisito final

## Inputs necessários

1. CTPS digital do cliente
2. CNIS (Cadastro Nacional de Informações Sociais)
3. Documentos de tempo especial (PPP, LTCAT — para conversão se aplicável)
4. Documentos de tempo rural (declaração do sindicato, notas de produtor)
5. Documentos de período militar
6. Recolhimentos como autônomo / facultativo
7. Vínculos no exterior (se houver acordo internacional)
8. Procuração

## Cálculos

### Salário-de-benefício pós-EC 103/2019 (art. 26)
- **Média de TODAS as contribuições** desde julho/1994 (não mais 80% maiores)
- Atualização monetária

### Coeficiente de cálculo
- Regra geral: 60% + 2% por ano que exceder 20H/15M
- Regra do pedágio 100%: 100% da média
- Regra antiga (até 13/11/2019): aposentadoria com fator previdenciário

### Fator previdenciário
- Vigente para regra do pedágio 50% ou direito adquirido até 13/11/2019
- f = (Tc × a / Es) × [1 + (Id + Tc × a) / 100]
  - Tc = tempo contribuição
  - a = alíquota (0,31)
  - Es = expectativa de sobrevida
  - Id = idade

## Tempo computável

| Tipo | Como comprovar |
|---|---|
| CLT | CTPS + CNIS |
| Servidor RPPS | Certidão de tempo de contribuição |
| Autônomo | GPS / Carnê de contribuição |
| Facultativo | GPS |
| Tempo rural antes de 1991 | Declaração do sindicato + testemunhas + notas produtor (Tema 642 STJ — prova material) |
| Tempo militar | CTC militar |
| Tempo especial → comum | PPP + LTCAT (skill 49) |

## Estrutura — petição inicial RPV / requerimento

### Pedido administrativo (Meu INSS)
1. Acessar Meu INSS (gov.br/meuinss)
2. Solicitar aposentadoria por tempo de contribuição (regra de transição)
3. Anexar documentação
4. INSS responde em 90 dias (Lei 9.784/99)

### Recurso administrativo (CRPS)
- 30 dias para recorrer ao Conselho de Recursos da Previdência Social
- Junta de Recursos: 1ª instância
- Câmara Especializada: 2ª

### Ação judicial (após exaurimento administrativo OU em paralelo)

```
EXMO. SR. JUIZ FEDERAL DA __ª VARA / DA __ª VARA PREVIDENCIÁRIA DE __________

[REQUERENTE]

vem propor

AÇÃO DE CONCESSÃO DE APOSENTADORIA POR TEMPO DE CONTRIBUIÇÃO

em face do INSS — Instituto Nacional do Seguro Social, pelos motivos a seguir.

I — DOS FATOS
1. O autor é segurado do RGPS, contando com __ anos, __ meses e __ dias de contribuição, conforme CNIS e CTPS (anexos).
2. Em __/__/____ requereu administrativamente a aposentadoria, indeferida (cópia anexa) sob argumento de __________
3. Cumpre os requisitos da regra de transição [especificar]:
   - Tempo: __ anos
   - Idade: __ anos
   - Pontos: __ (regra de pontos)
   - Pedágio: __ (regra de pedágio)

II — DO DIREITO
2.1. Da regra de transição [identificar]
2.2. Da contagem correta do tempo (períodos contestados)
2.3. Da conversão de tempo especial em comum [se aplicável]
2.4. Cálculo do RMI

III — DOS PEDIDOS
a) Concessão de tutela provisória de urgência: implantação imediata do benefício (CPC 300; em previdenciário: comprovado o direito + risco do tempo)
b) Citação do INSS;
c) Procedência para:
   c.1) Reconhecer o direito à aposentadoria;
   c.2) Determinar a implantação do benefício, com RMI calculado conforme a regra de transição;
   c.3) Pagamento dos atrasados desde a data do requerimento administrativo (DER), com correção e juros (Tema 905 STJ);
d) Honorários sucumbenciais ao INSS (CPC 85 § 3º — escala progressiva);
e) Gratuidade de justiça.

IV — DO VALOR DA CAUSA: R$ __________ (12 prestações)
```

## Atrasados (DIB ≠ DER)

- DIB (Data de Início do Benefício): com sentença
- DER (Data de Entrada do Requerimento): atrasados a partir desta data
- Súm 33 TNU + STJ: atrasados desde DER mesmo se a documentação foi completada depois

## Erros comuns

- Não esgotar via administrativa (necessário para ação judicial — Tema 350 STJ; mas há dispensa para casos específicos).
- Erro na regra de transição escolhida — escolher a mais favorável.
- Ignorar tempo rural anterior a 1991.
- Não converter tempo especial.
- Esquecer atrasados desde DER.
- Inclusão de períodos sem prova material.
- Médias mal calculadas (a partir de 1994 todas).

## Checklist

- [ ] CNIS atualizado e CTPS verificada
- [ ] Tempo bruto e líquido apurado
- [ ] Regra de transição mais favorável identificada
- [ ] Tempo especial convertido (se aplicável)
- [ ] Tempo rural reconhecido (se aplicável)
- [ ] Cálculo do RMI
- [ ] DER respeitada para atrasados
- [ ] Tutela de urgência se houver hipossuficiência
- [ ] Gratuidade
- [ ] Procuração
- [ ] Vara federal previdenciária

## Referências

- EC 103/2019 (Reforma da Previdência)
- Lei 8.213/1991 (Plano de Benefícios)
- Lei 8.212/1991 (Custeio)
- Decreto 3.048/1999 (RPS)
- Súmulas TNU
- Súmula 33 STJ (atrasados desde DER)
- Tema 350 STJ (prévio requerimento administrativo)
- Tema 642 STJ (tempo rural)
- Tema 905 STJ (correção monetária)

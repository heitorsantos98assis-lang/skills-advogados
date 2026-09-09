---
name: 39-acordo-acionistas
description: "Estrutura acordo de acionistas / quotistas (Lei 6.404/76 art. 118 + CC 1.025) com cláusulas de tag-along, drag-along, preferência, lock-up, voto em bloco, deadlock e arbitragem."
allowed-tools: Read Grep Bash Edit Write
---

## Quando usar

- Empresa familiar com sócios entrando ou querendo regulamentar gestão
- Investimento de fundo / VC / PE
- Joint venture
- Holding patrimonial com governança organizada

Aplica-se tanto a S.A. (CVM e Lei 6.404/76 art. 118) quanto a LTDA (CC 1.025 + jurisprudência STJ que aplica art. 118 por analogia em algumas hipóteses).

## Inputs necessários

1. Contrato social / estatuto atualizado
2. Quadro societário com participações
3. Plano de negócios (para vincular cláusulas de saída a milestones)
4. Identificação de "investidor" e "fundadores" (se for o caso)
5. Procuração

## Cláusulas típicas

### 1. Direito de preferência (CC 1.057, Lei 6.404 art. 109 II)
Sócio querendo vender cotas/ações deve oferecer aos demais nas mesmas condições.

```
CLÁUSULA __ — DIREITO DE PREFERÊNCIA
Caso qualquer sócio pretenda alienar suas cotas a terceiro, deverá previamente notificar os demais sócios, indicando preço, prazo e demais condições. Os demais terão prazo de 30 dias para manifestar interesse na aquisição em igualdade de condições, na proporção de suas cotas.
```

### 2. Tag-along (direito de venda conjunta)
Quando um sócio vende, os demais podem "ir junto" pelas mesmas condições.

```
CLÁUSULA __ — TAG-ALONG
No caso de alienação a terceiro de cotas equivalentes a mais de __% do capital, os demais sócios terão direito a vender suas cotas ao mesmo adquirente, pelo mesmo preço por cota e nas mesmas condições.
```

### 3. Drag-along (direito de venda forçada)
Sócio majoritário pode forçar minoritários a vender quando há comprador para 100%.

```
CLÁUSULA __ — DRAG-ALONG
Caso sócios titulares de mais de __% do capital decidam alienar a terceiro, poderão exigir que os demais sócios alienem suas cotas pelas mesmas condições, em ato simultâneo, ficando obrigados a aceitar a oferta sob pena de execução específica.
```

### 4. Lock-up (não venda por prazo)
Sócios não podem vender por X anos após a entrada do investidor / IPO.

```
CLÁUSULA __ — LOCK-UP
Os sócios fundadores comprometem-se a não alienar mais de __% de suas cotas pelo prazo de __ anos, salvo com anuência expressa dos demais sócios.
```

### 5. Acordo de voto em bloco (Lei 6.404 art. 118)
Sócios concordam em votar de forma unificada em assembleia.

```
CLÁUSULA __ — VOTO EM BLOCO
Os sócios obrigam-se a votar em conjunto nas seguintes deliberações: distribuição de lucros acima do mínimo legal, alteração do estatuto, eleição de administradores, aumento de capital. A definição interna do voto será por maioria dos integrantes do bloco; em caso de empate, prevalece o sócio __________.
```

### 6. Deadlock (resolução de impasses)
Quando há impasse, mecanismo de resolução.

```
CLÁUSULA __ — DEADLOCK
Em caso de impasse em deliberação relevante mantido por mais de __ dias, será aplicada a seguinte solução:
   a) Mediação obrigatória por __ dias
   b) Persistindo, **buy-or-sell** (Texas shoot-out): qualquer sócio pode oferecer comprar a participação do outro por preço X; o outro tem opção de vender por X ou comprar a participação do oferente por X
   c) Alternativa: arbitragem para definir o impasse
```

### 7. Vesting / Cliff
Para sócios fundadores em startups que querem proteção contra saída prematura.

```
CLÁUSULA __ — VESTING
A participação do sócio fundador __________ está sujeita a regime de vesting de __ anos, com cliff de 1 ano. Antes do cumprimento do cliff, retirada implicará perda da totalidade das cotas (que retornarão à sociedade ou serão cedidas aos demais). Após o cliff, vesting linear de 1/__ ao mês.
```

### 8. ROFR (Right of First Refusal — Direito de Última Oferta)
Sócio com direito de igualar oferta de terceiro.

### 9. Confidencialidade

```
CLÁUSULA __ — CONFIDENCIALIDADE
Os sócios obrigam-se a manter sigilo sobre informações estratégicas, financeiras, técnicas e comerciais, durante e por __ anos após a saída.
```

### 10. Não concorrência

```
CLÁUSULA __ — NÃO CONCORRÊNCIA
Por __ anos após a saída, o sócio retirante não poderá direta ou indiretamente exercer atividade concorrente no mesmo ramo, no território __________, sob pena de multa de R$ __________ por evento.
```

### 11. Pacto de votos em vetos (afirmative votes)
Investidor minoritário com poder de veto em decisões críticas.

```
CLÁUSULA __ — VETOS DO INVESTIDOR
As seguintes deliberações dependem do voto favorável do investidor __________:
   a) Aumento ou redução de capital
   b) Aprovação ou alteração do orçamento anual
   c) Contratação ou demissão do CEO
   d) Empréstimos > R$ __
   e) Alteração de objeto social
   f) Distribuição de lucros acima do mínimo
   g) Alienação de ativos > __%
```

### 12. Estatuto e regimento interno

### 13. Distribuição de lucros mínima

```
CLÁUSULA __ — POLÍTICA DE DIVIDENDOS
A sociedade distribuirá no mínimo __% do lucro líquido apurado anualmente, ressalvada decisão unânime para reinvestimento.
```

### 14. Aprovação prévia para gestos societários
Atos que mudem a estrutura ou o controle precisam de aprovação superior.

### 15. Resolução de litígios — arbitragem

```
CLÁUSULA __ — ARBITRAGEM
Litígios oriundos deste acordo serão resolvidos por arbitragem perante a Câmara de Arbitragem __________, conforme seu regulamento, sentença com força de coisa julgada nos termos da Lei 9.307/96.
```

## Estrutura — esqueleto

```
ACORDO DE SÓCIOS / ACIONISTAS DA __________

CONTRATANTES:
   - [Sócio 1] (qualificação)
   - [Sócio 2] (qualificação)
   - [Investidor] (qualificação)

INTERVENIENTE: __________ [Sociedade]

Considerando que [...]
Considerando que [...]
Resolvem celebrar o presente Acordo, em conformidade com o art. 118 da Lei 6.404/76 / art. 1.025 do CC, mediante as seguintes cláusulas:

CLÁUSULA 1ª — OBJETO E ABRANGÊNCIA
[Definir o que o acordo regula, indicar a sociedade, vincular as cotas/ações]

CLÁUSULA 2ª — DEFINIÇÕES
[Termos técnicos]

CLÁUSULA 3ª — VALORES DA SOCIEDADE / CAPITAL / DIRETORIA

CLÁUSULA 4ª — DIREITO DE PREFERÊNCIA
CLÁUSULA 5ª — TAG-ALONG
CLÁUSULA 6ª — DRAG-ALONG
CLÁUSULA 7ª — LOCK-UP
CLÁUSULA 8ª — VOTO EM BLOCO
CLÁUSULA 9ª — VETOS DO INVESTIDOR
CLÁUSULA 10ª — DEADLOCK
CLÁUSULA 11ª — DISTRIBUIÇÃO DE LUCROS
CLÁUSULA 12ª — VESTING (se aplicável)
CLÁUSULA 13ª — CONFIDENCIALIDADE
CLÁUSULA 14ª — NÃO CONCORRÊNCIA
CLÁUSULA 15ª — INDENIZAÇÕES (R&W — representations and warranties)
CLÁUSULA 16ª — RESCISÃO
CLÁUSULA 17ª — REGISTRO E EFICÁCIA PERANTE TERCEIROS
   "O presente acordo será arquivado na sede da sociedade e, em S.A., averbado no livro de registro de ações nominativas (Lei 6.404 art. 118 § 1º) para produzir efeitos perante terceiros."
CLÁUSULA 18ª — ARBITRAGEM
CLÁUSULA 19ª — DISPOSIÇÕES GERAIS

[Assinaturas + Visto OAB]
```

## Cláusulas que vinculam efetivamente

- Em S.A.: averbação no livro de registro (eficácia perante terceiros)
- Em LTDA: registro do acordo na sede + cláusula no contrato social pode dar efeito perante terceiros

## Cuidados

### Conflito com estatuto / contrato social
- Acordo deve se harmonizar com o estatuto
- Se conflitante, prevalece o estatuto em alguns aspectos

### Investidor estrangeiro
- Cláusulas em conformidade com regulação local + tributação
- Consultar regulação cambial do BCB

### Vesting com saída por justa causa
- Definir o que é justa causa
- Boa-fé do fundador

### Multa pecuniária
- Limites razoáveis (CC 412 — não ultrapassar valor da obrigação principal)

## Erros comuns

- Acordo sem registro / averbação → ineficácia perante terceiros.
- Cláusulas conflitantes com estatuto.
- Drag-along sem proteção mínima ao minoritário.
- Vesting sem cliff (sócio sai com tudo na semana 1).
- Veto generalizado sem critérios objetivos.
- Não-concorrência ilimitada (deve ter prazo e território).
- Arbitragem sem definir câmara.

## Checklist

- [ ] Identificação clara das partes e da sociedade
- [ ] Cláusulas patrimoniais (preferência, tag, drag, lock-up)
- [ ] Cláusulas de governança (voto, vetos, deadlock)
- [ ] Cláusulas de proteção (não concorrência, confidencialidade)
- [ ] Cláusulas de saída (vesting, recompra)
- [ ] Mecanismo de resolução de litígios
- [ ] Registro / averbação para eficácia perante terceiros
- [ ] Visto da OAB
- [ ] Compatibilidade com estatuto
- [ ] Tributação considerada

## Referências

- Lei 6.404/1976 art. 118
- CC arts. 1.025, 1.057, 412
- Lei 9.307/1996 (Arbitragem)
- Súmula CVM Pareceres
- Boa prática internacional (term sheets, modelos NVCA — adaptados)

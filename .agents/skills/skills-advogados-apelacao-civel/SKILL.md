---
name: skills-advogados-apelacao-civel
description: "Estrutura recurso de apelação cível (CPC 1.009-1.014) com tempestividade de 15 dias, preparo, razões com vícios apontados (error in procedendo / in judicando) e contrarrazões."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Claude, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Para impugnar **sentença** terminativa (sem resolução de mérito — CPC 485) ou definitiva (com mérito — CPC 487). Prazo: **15 dias úteis** (CPC 1.003 § 5º) da intimação da sentença, dobra para a Fazenda Pública e para litisconsortes com procuradores diferentes (CPC 229).

## Inputs necessários

1. Sentença (com data de publicação/intimação confirmada)
2. Comprovante de tempestividade (intimação no DJe ou pessoal)
3. Custas / preparo (depósito da guia + porte de remessa) ou gratuidade
4. Procuração e documentos
5. Tese a discutir: error in judicando (mérito) ou in procedendo (forma)

## Estrutura

```
EXMO. SR. DESEMBARGADOR RELATOR DA __ª CÂMARA CÍVEL DO TRIBUNAL DE JUSTIÇA DE __________

Apelante: __________
Apelado: __________
Origem: __ª Vara Cível de __________ — Processo nº __________

[CABEÇALHO ENDEREÇADO AO JUIZ DE 1ª INSTÂNCIA — CPC 1.010]
EXMO. SR. JUIZ DE DIREITO DA __ª VARA CÍVEL DA COMARCA DE __________

__________ [apelante], nos autos da ação __________ que move em face de __________, vem, com fundamento nos artigos 1.009 e 1.010 do CPC, interpor

APELAÇÃO

contra a r. sentença de fls. __, requerendo seu processamento e remessa ao TJ-__ para julgamento, conforme razões em anexo. Junta-se o preparo (CPC 1.007).

[Local, data]
________________________
[Advogado] OAB/__ ______

==========================================================
RAZÕES DE APELAÇÃO

EGRÉGIA CÂMARA / VENERANDOS DESEMBARGADORES

I — TEMPESTIVIDADE E PREPARO
Sentença publicada/intimada em __/__/____, ciente o apelante em __/__/____ — 15 dias úteis, com termo final em __/__/____. Apelação interposta nesta data, dentro do prazo legal. Preparo: guia DARJ/DARE/DJE nº __________ no valor de R$ __________ + porte de R$ __________.

II — DOS FATOS
[Resumo do processo até a sentença]

III — DO ERRO DE FATO E/OU DE DIREITO NA SENTENÇA
[Explanar especificamente onde a sentença errou]

IV — DOS FUNDAMENTOS DO RECURSO

4.1. Error in procedendo (vícios processuais)
   - Cerceamento de defesa
   - Nulidade por ausência de fundamentação (CF 93 IX e CPC 489 § 1º)
   - Julgamento extra/ultra/citra petita (CPC 492)
   - Falta de manifestação sobre prova essencial

4.2. Error in judicando (vícios materiais)
   - Aplicação errada da lei
   - Valoração equivocada de prova
   - Tese de mérito (apresentar tese)

V — DA TESE DEFENDIDA / DO MÉRITO
[Argumentar para reforma]

VI — DOS PEDIDOS
Pelo exposto, requer:
a) O conhecimento e o provimento do presente recurso, para reformar a r. sentença, [especificar a nova solução: julgamento de procedência/improcedência, anulação, redução do valor];
b) Subsidiariamente, a anulação da sentença e o retorno dos autos à origem para [novo julgamento, produção de prova];
c) A condenação do apelado ao pagamento de honorários recursais (CPC 85 § 11);
d) A inversão do ônus de sucumbência.

[Local, data]
________________________
[Advogado] OAB/__ ______
```

## Estrutura de protocolo (CPC 1.010)

A apelação é dirigida ao **juiz de 1º grau** (juízo a quo) que faz juízo de admissibilidade prévio (CPC 1.010 § 3º — sem efeito suspensivo automático após Lei 13.105/2015) e remete ao tribunal.

A petição é endereçada ao tribunal nas razões; mas o protocolo é no juízo originário.

## Efeitos da apelação (CPC 1.012)

### Efeito devolutivo
- Sempre. Devolve o conhecimento da matéria ao tribunal.
- Profundidade (§§ 1º a 4º): tudo que foi suscitado, mesmo sem decisão expressa.

### Efeito suspensivo
- Regra: **possui** efeito suspensivo (parte que apela suspende a sentença até julgamento).
- Exceções (CPC 1.012 § 1º) — sentença produz efeitos imediatos:
  - Homologa divisão/demarcação
  - Condena pagamento de alimentos
  - Extingue sem resolução de mérito ou julga improcedentes os embargos do executado
  - Julga procedente pedido de instituição de arbitragem
  - Confirma, concede ou revoga tutela provisória
  - Decreta a interdição

Nesses casos, o apelante pode requerer efeito suspensivo (CPC 1.012 §§ 3º e 4º) ao próprio relator no tribunal, demonstrando risco de dano grave.

## Preparo (CPC 1.007)

- Comprovado no momento da interposição
- **Pena de deserção**
- Em caso de ausência de preparo, há possibilidade de complementação (§ 2º) com multa de 50% se intimado para complementar.
- Beneficiário da gratuidade: dispensado.

## Sustentação oral

- Possível na sessão de julgamento, com 15 minutos, requerendo no momento.
- Útil em casos complexos.

## Honorários recursais (CPC 85 § 11)

- O tribunal MAJORA os honorários do advogado vencedor entre 1% e 5% sobre o valor já fixado, se o recurso for inadmissível ou improcedente.
- Limite total: 20% do valor da causa/condenação (10% Fazenda).

## Erros comuns

- Perder prazo (15 dias úteis — Fazenda 30) → preclusão.
- Esquecer preparo → deserção.
- Não impugnar todos os fundamentos da sentença (Súmula 283 STF — apenas para STJ/STF, mas a lógica vale).
- Apelação genérica sem especificar onde a sentença errou (CPC 1.010 II — exposição do fato e do direito; III — razões do pedido de reforma; IV — pedido de nova decisão).
- Não pedir honorários recursais.
- Não pedir efeito suspensivo quando regra é não suspender (CPC 1.012 § 1º).
- Apresentar provas novas em apelação (em regra, vedado — CPC 435 e exceção 438).

## Checklist

- [ ] Tempestividade (15 dias úteis ou 30 Fazenda) confirmada
- [ ] Preparo + porte + ARO (Apelado por Resistência ao Operador?) comprovados
- [ ] Cabeçalho ao juiz de 1º grau, razões ao tribunal
- [ ] Tempestividade demonstrada nas razões
- [ ] Erro fundamentado (in procedendo / in judicando)
- [ ] Pedido de reforma OU anulação
- [ ] Pedido de honorários recursais
- [ ] Pedido de efeito suspensivo se aplicável
- [ ] Sustentação oral requerida (se desejar)
- [ ] Procuração nos autos
- [ ] Protocolo eletrônico OK

## Erros recorrentes a evitar nas razões

- Repetir argumentos da inicial/contestação sem confrontar a sentença.
- Não atacar fundamento autônomo (Súmula 283/STF).
- Pedido genérico ("provimento do recurso").

## Referências

- CPC arts. 1.003 (prazo), 1.007 (preparo), 1.009-1.014 (apelação), 1.012 (efeitos), 85 §§ 11 (honorários recursais), 489 § 1º (motivação)
- CF 93 IX (motivação das decisões)
- Súmulas STJ e STF de admissibilidade
- Regimento Interno do TJ correspondente

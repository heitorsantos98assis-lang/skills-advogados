---
name: skills-advogados-habeas-corpus
description: "Estrutura HC liberatório/preventivo (CF 5º LXVIII; CPP 647-667) com competência por hierarquia da autoridade coatora, fundamentação no constrangimento ilegal e pedido de liminar."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Claude, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Sempre que houver **constrangimento ou ameaça** à liberdade de locomoção (CF 5º LXVIII):
- Prisão ilegal (em flagrante, preventiva, temporária, definitiva)
- Excesso de prazo na prisão
- Quebra de domicílio
- Coação no investigado
- Excesso na preventiva (cabendo medidas alternativas)
- Tranca-ação penal (pedidos de absolvição sumária / trancamento por ilegalidade manifesta)

**Sem prazo** — pode ser impetrado a qualquer tempo (CPP 648 estabelece hipóteses).

## Inputs necessários

1. Identificação do paciente (preso ou ameaçado)
2. Identificação da autoridade coatora (Delegado, Juiz, Promotor — quando atuação seja constrangedora)
3. Documentos: auto de prisão, decisão judicial, denúncia, IP
4. Provas do constrangimento ilegal
5. Procuração (HC dispensa CPP 654 — qualquer pessoa pode impetrar — mas advocacia pessoal facilita)

## Competência (CF + CPP)

| Coator | HC perante |
|---|---|
| Particular | Juiz de 1º grau |
| Delegado de Polícia | Juiz competente para a infração |
| Juiz de 1º grau (TJ/TJM) | TJ / TRF |
| Desembargador (TJ/TRF) | STJ |
| Ministro do STJ | STF (se ato individual) |
| TRT | TST |
| Tribunal Regional Eleitoral | TSE |
| Lei especial | Conforme indicado |

## Estrutura

```
EXMO. SR. DESEMBARGADOR PRESIDENTE DO TRIBUNAL DE JUSTIÇA / DOUTO MIN. DO STJ / EXMO. SR. JUIZ

__________ [impetrante] (qualificação completa, OAB), em favor de __________ [paciente] (qualificação), com fundamento na CF art. 5º LXVIII e nos arts. 647 a 667 do CPP, impetra

HABEAS CORPUS

contra ato do MM. Juiz da __ª Vara Criminal da Comarca de __________ (autoridade coatora), pelas razões a seguir.

I — DOS FATOS
1. O paciente foi preso/processado por __________ no dia __/__/____.
2. [Síntese: situação atual]
3. A autoridade coatora decidiu __ no dia __/__/____.

II — DO CONSTRANGIMENTO ILEGAL — CPP 648

Cabe HC quando:
   I — sem justa causa
   II — por mais tempo do que determina a lei
   III — quem ordenar coação não tiver competência
   IV — cessar motivo da coação
   V — não for admitida a fiança
   VI — processo manifestamente nulo
   VII — extinta a punibilidade

[Identificar a hipótese aplicável]

III — DAS RAZÕES DE DIREITO

3.1. [Tese principal]
   Ex.: ausência de fundamentação concreta na preventiva (Súm Vinculante STF + CPP 312)
   Ex.: existência de medida cautelar diversa suficiente (CPP 319 — Pacote Anticrime Lei 13.964/19)
   Ex.: excesso de prazo (HC 81.149 STF; Súm 64 STJ — soma do tempo de prisão para análise)
   Ex.: prisão sem flagrante / ilegalidade do flagrante (CPP 302-310)
   Ex.: trancamento da ação por atipicidade / inépcia / falta de justa causa

3.2. [Fundamentação legal]
3.3. [Jurisprudência: STF, STJ, súmulas]

IV — DO PEDIDO LIMINAR
A urgência é evidente (prisão atual). Há fumus boni iuris (constrangimento ilegal demonstrado) e periculum in mora (cada dia de prisão é dano irreparável). Requer-se:

a) Concessão liminar do HC para [soltura imediata / suspensão da preventiva / desbloqueio do procedimento];
b) Expedição de alvará de soltura urgente.

V — DOS PEDIDOS
a) Notificação da autoridade coatora para prestar informações em 24-48 horas;
b) Vista ao Ministério Público;
c) Concessão da ordem para [pedido específico];
d) Comunicação ao Juízo de origem;
e) Eventual extensão de efeitos a corréus em situação idêntica.

[Local], [data]
________________________
[Impetrante] OAB/__ ______
```

## Hipóteses comuns

### 1. Prisão preventiva sem fundamentação concreta
- CPP 312 § 2º (Pacote Anticrime): preventiva exige **periculum libertatis** concreto
- Argumento genérico ("para garantia da ordem pública") sem dados específicos = ilegal
- Súm Vinculante STF e jurisprudência consolidada

### 2. Excesso de prazo na instrução
- Soma do tempo total da prisão preventiva
- Sem justificativa para a demora atribuível à defesa
- Tempo razoável (Convenção Americana de Direitos Humanos)

### 3. Tranca-ação penal
- Atipicidade manifesta
- Inépcia da denúncia (CPP 41)
- Falta de justa causa
- Demanda análise abstrata, sem revolvimento de prova (Súmula 7 STJ)

### 4. Substituição da preventiva por medidas cautelares (CPP 319)
- Comparecimento periódico
- Proibição de acesso/aproximação
- Recolhimento domiciliar
- Monitoramento eletrônico
- Suspensão de funções
- Internação provisória
- Fiança

### 5. Direito ao silêncio / não autoincriminação
- CPP 186 + CF 5º LXIII

### 6. Quebra de domicílio sem mandado
- CF 5º XI: inviolabilidade salvo flagrante delito, desastre, prestar socorro, ou determinação judicial durante o dia

## Liminar

Em HC, a liminar é frequentemente decidida pelo relator no tribunal. Ataque urgente: telefonema/petição ao gabinete do plantão se necessário.

## HC coletivo

Pode-se pleitear extensão de efeitos a corréus em situação idêntica (CPP 580). HC coletivo (Tema 1.041 STF — admite ações coletivas).

## Erros comuns

- Impetrar HC contra ato de delegado quando o controle já passou ao juiz (audiência de custódia ratificou) → ineficiência.
- HC sem demonstrar urgência específica.
- HC contra prova ilícita sem alegação detalhada da nulidade.
- Tentar revolver prova (HC não substitui apelação para reanálise probatória — Súm 7 STJ).
- Esquecer pedido liminar.
- Não anexar a decisão coatora.

## Checklist

- [ ] Autoridade coatora identificada
- [ ] Competência correta (hierarquia)
- [ ] Constrangimento ilegal enquadrado em CPP 648
- [ ] Fundamentação com lei + jurisprudência
- [ ] Pedido liminar
- [ ] Documentos do paciente e da decisão
- [ ] Procuração (se houver advogado)
- [ ] Protocolo no PJe / Sistema do Tribunal

## Referências

- CF arts. 5º LXVIII, LXIII, LIV, LV, LVII
- CPP arts. 282, 312-316 (preventiva), 319, 320, 322, 647-667
- Lei 13.964/2019 (Pacote Anticrime)
- Súmula Vinculante 11 STF (algemas)
- Súmula 64 STJ (excesso prazo)
- Tema 1.041 STF (HC coletivo)
- HC 81.149 STF (excesso prazo razoável)

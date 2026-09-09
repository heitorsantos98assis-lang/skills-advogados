---
name: skills-advogados-inventario-judicial
description: "Conduz inventário judicial (CPC 610-673) com nomeação de inventariante, primeiras declarações, avaliação, ITCMD, sobrepartilha e formal de partilha — adequado quando há litígio, herdeiro incapaz ou testamento."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Claude, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Se uma das seguintes hipóteses (CPC 610):
- Há herdeiro **incapaz**, salvo decisão judicial autorizando extrajudicial (Lei 14.382/2022)
- Há **litígio** entre herdeiros
- Há **testamento** não passível de extrajudicial
- A massa hereditária é complexa (empresas, bens em vários países)

## Inputs necessários

(Mesmos da skill 20)

1. Certidão de óbito
2. Certidão de casamento + pacto antenupcial
3. Documentos dos herdeiros e cônjuge
4. CENSEC (testamento)
5. Lista de bens
6. Certidões negativas
7. Identificação do **inventariante** proposto (CPC 617 — ordem preferencial)

## Inventariante (CPC 617)

Ordem preferencial:
1. Cônjuge ou companheiro sobrevivente que residia com o falecido
2. Herdeiro mais velho que esteja na posse e administração dos bens
3. Qualquer herdeiro nomeado pelos demais
4. Testamenteiro
5. Cessionário de herdeiros
6. Inventariante judicial (provisório), em casos de litígio extremo
7. Inventariante dativo (juiz nomeia)

## Estrutura — petição inicial

```
EXMO. SR. JUIZ DA __ª VARA DE FAMÍLIA E SUCESSÕES DA COMARCA DE __________

[REQUERENTE]: __________

vem propor

INVENTÁRIO JUDICIAL

dos bens deixados por __________, falecido em __/__/____ (certidão anexa), com base nos arts. 610 e seguintes do CPC.

I — DOS FATOS
1. O autor é [filho/cônjuge/herdeiro] do falecido.
2. O falecido era casado com __ sob regime __, com filhos __________.
3. CENSEC: [há ou não há testamento] — certidão anexa.
4. Razão do inventário judicial: [há herdeiro menor/incapaz / há litígio / há testamento].

II — DOS PEDIDOS PRELIMINARES
a) Distribuição com gratuidade (se aplicável) ou recolhimento de custas;
b) Citação dos demais herdeiros (CPC 626);
c) Nomeação de **inventariante** na pessoa de __________ [nome], que aceita o encargo (termo anexo);
d) Determinação para apresentação das primeiras declarações em 20 dias (CPC 620).

III — DOS BENS DO ESPÓLIO
[Lista preliminar — completa em primeiras declarações]

IV — DAS DÍVIDAS DO ESPÓLIO

V — DO VALOR DA CAUSA: R$ __________ (estimativa do monte-mor)

[Local], [data] — Adv. OAB
```

## Procedimento (CPC 610-673)

### 1. Distribuição e nomeação do inventariante (CPC 617)
- Juiz nomeia
- Inventariante presta compromisso em 5 dias
- Termo de nomeação no processo

### 2. Primeiras declarações (CPC 620)
- Em 20 dias após termo
- Identificação do falecido, herdeiros, bens, dívidas
- Avaliações iniciais

### 3. Citação dos interessados (CPC 626)
- Cônjuge sobrevivente
- Herdeiros conhecidos
- Fazenda Pública (estadual e federal — interessada no ITCMD e tributos)
- Edital para herdeiros desconhecidos

### 4. Impugnações (CPC 627)
- Em 15 dias após primeiras declarações
- Contestar bens omitidos, valores, qualificação de herdeiros

### 5. Avaliação (CPC 630)
- Pode ser dispensada se houver consenso
- Perito judicial em caso de disputa

### 6. Últimas declarações (CPC 636)
- Inventariante apresenta
- Calculadas dívidas e créditos do espólio

### 7. Cálculo do ITCMD (CPC 637-638)
- Fazenda Estadual emite
- Pago pelo espólio

### 8. Pagamento de dívidas (CPC 642)

### 9. Partilha (CPC 647-657)
- Esboço de partilha apresentado pelo inventariante
- Recurso de impugnação
- Sentença homologatória

### 10. Formal de partilha (CPC 655)
- Documento que serve para registro nos cartórios

## Tipos de partilha

### Amigável (CPC 657)
- Consenso entre herdeiros maiores e capazes
- Termo levado ao juiz para homologação

### Judicial (CPC 648-651)
- Quando há divergência
- Esboço pelo inventariante
- Audiência se necessário
- Sentença

## Sobrepartilha (CPC 669; CC 1.040)

- Bens descobertos depois
- Bens em outro país
- Bens que estavam sendo discutidos

## Tributação

### ITCMD (estadual)
- Mesma lógica skill 20
- Em alguns estados, exige certidão de quitação para a sentença ser proferida

### IRPF do herdeiro
- Não há IR sobre o recebimento da herança (isento — Lei 9.250 art. 6º)
- Mas atualização do bem para o valor de mercado (na transmissão) gera **ganho de capital diferido** — quando o herdeiro vender o bem, calcular a partir do valor da partilha

### Repercussão na empresa do falecido
- Continuação dos contratos (CC 1.029, 1.028 — sociedade)
- Retirada dos haveres se herdeiros não querem participação

## Erros comuns

- Não citar a Fazenda → nulidade.
- Avaliação subestimada → ITCMD complementar exigido.
- Inventariante removível por má administração (CPC 622-624) — apresentar contas regularmente.
- Não fazer sobrepartilha de bens descobertos → herdeiros lesados.
- Imóvel rural sem CCIR atualizado.
- Bem em espólio: ainda em nome do falecido por longo tempo (anos depois) → IPTU, condomínio acumulam.
- Cônjuge sobrevivente esquecido como herdeiro concorrente.
- Renúncia de herança feita sem escritura pública → ineficaz (CC 1.806).

## Checklist

- [ ] Documentos completos
- [ ] CENSEC
- [ ] Lista de bens com avaliação
- [ ] Inventariante nomeado e termo de compromisso
- [ ] Primeiras declarações em 20 dias
- [ ] Citação de todos os interessados (incluindo Fazenda)
- [ ] Avaliação (perícia se houver disputa)
- [ ] Últimas declarações
- [ ] ITCMD calculado e pago
- [ ] Pagamento de dívidas
- [ ] Esboço / partilha amigável
- [ ] Sentença homologatória
- [ ] Formal de partilha emitido
- [ ] Averbações em matrículas, RENAVAM, JUCESP, B3
- [ ] Sobrepartilha dos bens descobertos

## Referências

- CC arts. 1.784-1.792, 1.829, 1.806, 1.040
- CPC arts. 610-673
- Lei 11.441/2007 (extrajudicial)
- Lei 14.382/2022
- Tema 809 STF (união estável = casamento)
- Súmula 377 STF
- CENSEC

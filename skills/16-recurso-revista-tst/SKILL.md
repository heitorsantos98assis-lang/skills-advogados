---
name: recurso-revista-tst
description: Estrutura recurso de revista ao TST com pressupostos extrínsecos (preparo, prazo) e intrínsecos (transcendência, divergência, violação literal CF/CLT/súmula), seguindo CLT 896 e IN 23/TST.
allowed-tools: Read Grep Bash Edit Write
user-invocable: true
---

## Quando usar

Para impugnar **acórdão do TRT** que julgou recurso ordinário (ou agravo de petição em execução). Cabe **apenas em hipóteses restritas** (CLT 896). Prazo: **8 dias úteis** da intimação do acórdão.

## Pressupostos

### Extrínsecos
- Tempestividade (8 dias úteis)
- Preparo: depósito recursal + custas (ou gratuidade)
- Procuração com poderes especiais
- Capacidade postulatória

### Intrínsecos (CLT 896)
Caber em apenas três hipóteses **alternativas**:

**a) Divergência jurisprudencial**
- Acórdão do TRT divergente de decisão de outro TRT, da SBDI-1 ou súmula do TST
- Pelo menos 1 acórdão paradigma

**b) Violação literal de dispositivo de lei federal ou da CF**
- Aponta o artigo específico violado
- Não basta interpretação razoável diferente — deve haver violação literal

**c) Contrariedade a súmula do TST ou súmula vinculante do STF**

### Transcendência (CLT 896-A)
Lei 13.467/17 introduziu o filtro:
- **Econômica**: valor da causa relevante
- **Política**: divergência em julgamento de assunto de relevância
- **Social**: norma de aplicação a um conjunto de trabalhadores
- **Jurídica**: novidade jurídica

Sem transcendência → não conhecido.

## Estrutura

```
EXMO. SR. PRESIDENTE DO TRT — __ª REGIÃO

Recorrente: __________
Recorrido: __________
Processo nº __________

__________, com fulcro no art. 896 da CLT, interpõe

RECURSO DE REVISTA

contra o v. acórdão de fls. __ que [resumir o que decidiu], conforme razões anexas.

Custas: R$ __________ — guia anexa.
Depósito recursal: R$ __________ — guia anexa (se empregador).

[Local, data]
________________________
[Advogado] OAB/__ ______

==========================================================
RAZÕES DE RECURSO DE REVISTA

EXMO. SR. PRESIDENTE DO TRIBUNAL SUPERIOR DO TRABALHO

I — TEMPESTIVIDADE E ADMISSIBILIDADE
Acórdão publicado em __/__/____. Intimação em __/__/____. 8 dias úteis. Termo final: __/__/____.

II — DOS PRESSUPOSTOS RECURSAIS
2.1. Preparo (depósito + custas) — guias anexas
2.2. Procuração com poderes — anexa
2.3. Pressuposto específico (CLT 896): [escolher uma das três]
2.4. Transcendência: [demonstrar uma das categorias do CLT 896-A]

III — DOS FATOS
[Síntese cronológica do processo]

IV — DAS RAZÕES DE REFORMA

4.1. Quanto ao item __ do acórdão:

   4.1.1. Trecho do acórdão (transcrição literal):
   "..."

   4.1.2. Da divergência jurisprudencial
   - Paradigma 1: TRT da __ª Região, RO ___, Rel. ____, DJ __/__/____. Trecho: "..."
     (Anexa-se cópia integral do paradigma — IN 23/TST exige)
   - Paradigma 2: SBDI-1, E-RR ____. Trecho: "..."

   4.1.3. Demonstração analítica da divergência
   [Mostrar que os fatos são similares e a conclusão é diferente]

   4.1.4. Subsidiariamente, da violação literal
   - O acórdão violou o art. __ da CLT / CF, pois __________

   4.1.5. Da contrariedade a súmula
   - Súmula __ do TST: "[texto]"
   - O acórdão contraria a súmula porque __________

V — DA TRANSCENDÊNCIA (CLT 896-A)
A matéria possui transcendência [econômica/política/social/jurídica] porque __________.

VI — DOS PEDIDOS
Diante do exposto, requer:
a) O recebimento e processamento do presente recurso;
b) Conhecimento e provimento para reformar o acórdão e __________;
c) Subsidiariamente, anular o acórdão e remeter ao TRT para novo julgamento;
d) Honorários recursais.

[Local, data]
________________________
[Advogado] OAB/__ ______
```

## Pressupostos específicos no detalhe

### Demonstração analítica (Súm 296 TST)
Para divergência, é obrigatório:
- Transcrever literalmente o trecho do acórdão recorrido
- Transcrever o trecho do paradigma
- Demonstrar que tratam da mesma matéria, com mesmo fato e tese contrária

### Paradigmas válidos
- Acórdãos de outro TRT, SBDI-1 do TST, súmulas do TST
- **NÃO valem**: paradigma do mesmo TRT (Súm 23 TST), turma diversa do TST que não seja SBDI

### Súmula 442 TST
"A divergência jurisprudencial em recurso de revista, em matéria de direito processual, é inadmissível, salvo nos casos do § 2º do art. 896 da CLT" — execução em processo trabalhista.

## Despacho de admissibilidade

- Presidente do TRT: faz juízo prévio (CLT 896 § 1º). Pode negar.
- Se denegado: cabe **agravo de instrumento ao TST** (CLT 897 alínea b) — 8 dias.

## Erros comuns

- Não comprovar transcendência → não conhecido (filtro automatic).
- Paradigma do mesmo TRT — Súm 23 TST.
- Paradigma genérico, sem analítica.
- Recurso cópia das razões do RO — não impugna o acórdão.
- Custas / depósito atrasados → deserção.
- Não anexar cópia integral do paradigma (IN 23/TST).
- Apontar "violação literal" de dispositivo sem indicar a literalidade.

## Checklist

- [ ] Acórdão TRT do RO/AP juntado
- [ ] Tempestividade
- [ ] Preparo + custas (ou gratuidade)
- [ ] Pressuposto: divergência OU violação literal OU súmula
- [ ] Transcendência demonstrada
- [ ] Paradigmas (se divergência) com cópia integral
- [ ] Demonstração analítica
- [ ] Razões impugnando cada ponto do acórdão
- [ ] Honorários recursais
- [ ] Protocolo no PJe-JT (TRT origem)

## Referências

- CLT arts. 896, 896-A, 897, 899
- IN 23/TST
- Súmulas TST 23, 296, 337, 442
- Lei 13.467/2017 (transcendência)
- Resoluções TST sobre depósito recursal

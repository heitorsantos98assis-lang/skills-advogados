---
name: 57-minuta-contrato-servicos
description: "Minuta contrato de prestação de serviços com obrigações, prazo, preço, cláusula de confidencialidade, propriedade intelectual, rescisão, foro/arbitragem e LGPD."
allowed-tools: Read Grep Bash Edit Write
---

## Quando usar

Para formalizar relação de prestação de serviços (não trabalhista). Aplicável a:
- Consultoria
- Desenvolvimento de software
- Marketing / agência
- Manutenção
- Projeto de engenharia
- Serviços profissionais (com adaptação ao Conselho)

Atenção: confundir com contrato de trabalho gera risco de **pejotização** (Tema 725 STF discute terceirização lícita; mas pessoalidade + subordinação + habitualidade = vínculo CLT).

## Inputs necessários

1. Identificação completa contratante e contratado
2. Objeto preciso (escopo do serviço)
3. Prazo (determinado / indeterminado)
4. Preço, forma e periodicidade do pagamento
5. Reajuste (índice e periodicidade)
6. Penalidades por descumprimento
7. Eventuais cláusulas especiais (NDA, IP, exclusividade)
8. Foro de eleição ou arbitragem

## Estrutura completa

```
CONTRATO DE PRESTAÇÃO DE SERVIÇOS

Pelo presente instrumento particular, as partes:

CONTRATANTE: __________ (PF/PJ — qualificação completa)
CONTRATADO: __________ (PF/PJ — qualificação completa)

têm entre si, justo e contratado o seguinte:

CLÁUSULA 1ª — OBJETO
1.1. O CONTRATADO prestará ao CONTRATANTE os seguintes serviços:
   __________ [descrever de forma específica e mensurável]
1.2. Escopo detalhado constante do Anexo I (Especificação Técnica).
1.3. Não estão incluídos os serviços listados no Anexo II (Exclusões), que poderão ser objeto de aditivo.

CLÁUSULA 2ª — PRAZO
2.1. Este contrato vigora por __ meses, a partir de __/__/____, prorrogável por igual período mediante aditivo escrito.
2.2. Qualquer das partes poderá denunciar o contrato sem causa, mediante aviso escrito com __ dias de antecedência.

CLÁUSULA 3ª — PREÇO E FORMA DE PAGAMENTO
3.1. O CONTRATANTE pagará ao CONTRATADO o valor de R$ __________, conforme cronograma:
   - 1ª parcela: R$ __________ em __/__/____
   - 2ª parcela: R$ __________ em __/__/____
   ...
3.2. Pagamento mediante apresentação de NFS-e e relatório de execução.
3.3. Mora: 1% a.m. + multa de __% + correção pelo IPCA.
3.4. Reajuste: anual pelo IPCA acumulado no período (a partir do 13º mês).

CLÁUSULA 4ª — OBRIGAÇÕES DO CONTRATADO
4.1. Executar os serviços com diligência, técnica e qualidade.
4.2. Cumprir prazos e entregar conforme escopo.
4.3. Manter sigilo de informações confidenciais.
4.4. Manter habilitação profissional (registro em Conselho, etc.).
4.5. Recolher tributos próprios (sem geração de vínculo CLT).
4.6. Responsabilizar-se por seus colaboradores (sem vínculo com CONTRATANTE).
4.7. Manter seguro de responsabilidade civil (se aplicável ao escopo).
4.8. Comunicar formalmente qualquer atraso ou óbice.

CLÁUSULA 5ª — OBRIGAÇÕES DO CONTRATANTE
5.1. Pagar pontualmente os valores devidos.
5.2. Disponibilizar informações necessárias.
5.3. Aprovar / rejeitar entregas em prazo razoável (__ dias úteis).
5.4. Não interferir na execução técnica do CONTRATADO.

CLÁUSULA 6ª — INEXISTÊNCIA DE VÍNCULO TRABALHISTA
6.1. As partes declaram que este contrato é de natureza civil/comercial, regido pelo Código Civil.
6.2. Não há subordinação, pessoalidade obrigatória ou habitualidade nos moldes da CLT.
6.3. O CONTRATADO atua com autonomia de meios e organização.
6.4. Encargos trabalhistas, previdenciários e tributários próprios são de responsabilidade exclusiva do CONTRATADO.

CLÁUSULA 7ª — CONFIDENCIALIDADE
7.1. Toda informação trocada é confidencial, salvo as de domínio público.
7.2. Vigência: durante e por __ anos após o término do contrato.
7.3. Multa por descumprimento: R$ __________ por evento + perdas e danos.

CLÁUSULA 8ª — PROPRIEDADE INTELECTUAL
8.1. Os direitos sobre os entregáveis pertencem ao [CONTRATANTE / CONTRATADO] (definir conforme caso).
8.2. Em caso de software / obra intelectual: cessão exclusiva pelo CONTRATADO ao CONTRATANTE para uso ___ (definir limite).
8.3. Direitos morais do autor permanecem com o CONTRATADO (CC 24 da Lei 9.610).

CLÁUSULA 9ª — LGPD (Lei 13.709/2018)
9.1. As partes se comprometem a tratar dados pessoais conforme a LGPD.
9.2. CONTRATANTE é o controlador; CONTRATADO atua como operador.
9.3. Cláusula contratual específica de DPA (Data Processing Agreement) anexo, contendo:
   - Finalidades do tratamento
   - Categorias de dados
   - Medidas de segurança
   - Sub-operadores autorizados
   - Notificação de incidentes
   - Términos do contrato e exclusão dos dados

CLÁUSULA 10ª — NÃO CONCORRÊNCIA E NÃO ALICIAMENTO [opcional]
10.1. Durante e por __ meses após o término, o CONTRATADO não prestará serviços a concorrentes diretos do CONTRATANTE listados no Anexo III, exceto com autorização.
10.2. Não aliciar empregados / clientes do CONTRATANTE durante igual período.

CLÁUSULA 11ª — RESCISÃO
11.1. Rescisão por descumprimento de qualquer cláusula, mediante notificação prévia de __ dias para regularizar.
11.2. Rescisão imediata em caso de:
   - Falência ou insolvência
   - Atos que comprometam a reputação
   - Descumprimento doloso
   - Uso indevido de propriedade intelectual / informação confidencial
11.3. Multa rescisória: __% do valor remanescente.

CLÁUSULA 12ª — RESPONSABILIDADE
12.1. Cada parte responde por seus atos e omissões.
12.2. Limite de responsabilidade do CONTRATADO: valor pago no contrato (cap), salvo dolo, fraude, violação grave da LGPD ou IP.
12.3. CONTRATANTE indenizará o CONTRATADO por demandas decorrentes de informações fornecidas erroneamente.

CLÁUSULA 13ª — FORÇA MAIOR / CASO FORTUITO
Não há responsabilidade por descumprimento decorrente de força maior ou caso fortuito (CC 393), comunicado em __ dias.

CLÁUSULA 14ª — CESSÃO
14.1. Nenhuma das partes pode ceder o contrato sem anuência expressa da outra.

CLÁUSULA 15ª — RESOLUÇÃO DE LITÍGIOS
15.1. Mediação prévia obrigatória por 30 dias antes de qualquer ação judicial / arbitragem.
15.2. [Foro de eleição] Para dirimir litígios, fica eleito o foro de __________, com renúncia a qualquer outro, por mais privilegiado que seja.

OU

15.2. [Arbitragem] Litígios serão resolvidos por arbitragem perante a Câmara __________, conforme seu regulamento, sentença com força de coisa julgada (Lei 9.307/96).

CLÁUSULA 16ª — DISPOSIÇÕES GERAIS
16.1. Este contrato representa o entendimento completo entre as partes, prevalecendo sobre acordos anteriores.
16.2. Alterações somente por aditivo escrito assinado pelas partes.
16.3. A invalidade de uma cláusula não afeta as demais.

E, por estarem assim justos e contratados, assinam o presente contrato em duas vias de igual teor e forma.

[Local], [data]

________________________
CONTRATANTE

________________________
CONTRATADO

Testemunhas:
1. ________________________ CPF __________
2. ________________________ CPF __________
```

## Cláusulas adicionais por caso

### Software / desenvolvimento
- SLA (Service Level Agreement) — disponibilidade, suporte
- Versionamento e manutenção
- Entrega do código-fonte
- Garantia de bugs por __ meses

### Consultoria
- Relatórios entregáveis
- Apresentações
- Confidencialidade reforçada

### Engenharia / construção
- Cronograma de obra
- Aditivos e medições
- ART/RRT
- Garantia de obra (CC 618 — 5 anos)

### Marketing / agência
- KPIs (CTR, conversão)
- Aprovação de criativos
- Direitos sobre material publicitário

## Cuidados

### Pejotização (Tema 725 STF)
- Pessoalidade + subordinação + habitualidade + onerosidade = vínculo CLT
- Mesmo com contrato bem redigido, se na prática há vínculo, justiça reconhece
- Cláusula 6 não basta se a realidade for diversa

### Tributação
- PJ contratado emite NFS-e
- Retenções pelo tomador (skill 13 contadora)
- ISS no município do prestador (regra geral)

### Encerramento
- Devolução de bens, dados, materiais
- Confidencialidade segue
- Documentos de encerramento (relatório final)

## Erros comuns

- Escopo vago — abre disputa.
- Sem cláusula de reajuste em contrato longo.
- Sem cláusula de rescisão imediata por inadimplência.
- LGPD esquecida — passivo regulatório.
- Foro de eleição em contrato de adesão a consumidor (CDC 51 IV — invalida).
- Multa rescisória abusiva.
- Não distinguir cessão de IP de licença de uso.

## Checklist

- [ ] Identificação completa das partes
- [ ] Escopo claro
- [ ] Prazo e prorrogação
- [ ] Preço e pagamento
- [ ] Mora e reajuste
- [ ] Obrigações de cada parte
- [ ] Cláusula anti-vínculo CLT
- [ ] Confidencialidade
- [ ] Propriedade intelectual
- [ ] LGPD / DPA
- [ ] Não concorrência (se aplicável)
- [ ] Rescisão e multas
- [ ] Resolução de litígios (foro / arbitragem)
- [ ] Testemunhas (para força executiva extrajudicial — CPC 784 III)

## Referências

- CC arts. 593-609, 421, 422, 478
- CLT (para evitar pejotização — Tema 725 STF)
- Lei 9.307/1996 (Arbitragem)
- Lei 13.709/2018 (LGPD)
- Lei 9.610/1998 (Direitos Autorais)
- CPC art. 784 III (título extrajudicial)

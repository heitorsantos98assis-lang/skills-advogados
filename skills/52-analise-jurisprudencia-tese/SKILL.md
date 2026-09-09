---
name: 52-analise-jurisprudencia-tese
description: "Pesquisa, organiza e cita jurisprudência e súmulas para fundamentar peças, identificando precedentes vinculantes (CPC 927), repercussão geral, recursos repetitivos, IRDR e teses dominantes."
allowed-tools: Read Grep Bash Edit Write
---

## Quando usar

Em qualquer peça jurídica que necessite fundamentação. Skill operacional usada como apoio às demais. Pode ser invocada para:
- Construir tese para uma ação nova
- Defender em recurso
- Avaliar viabilidade de demanda

## Hierarquia das fontes (CPC 927)

Em ordem de força vinculante:

1. **Decisões do STF em controle concentrado** (ADI, ADC, ADPF)
2. **Súmulas vinculantes** (STF)
3. **Acórdãos do STF/STJ em recurso extraordinário/especial repetitivo** (Tema com julgamento) e em IRDR
4. **Súmulas do STF (matéria constitucional)** e **STJ (matéria infraconstitucional)**
5. **Orientação do plenário do STF e STJ**
6. **Acórdãos do STJ em recurso repetitivo**
7. **IRDR** dos tribunais
8. **Acórdãos do STJ em recurso de embargos de divergência**
9. **Acórdãos com efeito vinculante por lei**

## Onde pesquisar

### STF
- portal.stf.jus.br > Jurisprudência > Pesquisa de Acórdãos
- portal.stf.jus.br > Repercussão Geral > Temas
- Súmulas vinculantes

### STJ
- scon.stj.jus.br (Pesquisa de Jurisprudência)
- Repetitivos: scon.stj.jus.br > Pesquisa Pronta > Temas Repetitivos
- Súmulas do STJ

### TST
- jurisprudencia.tst.jus.br
- Súmulas e OJs

### Tribunais de 2ª instância
- TJ-SP/RJ/MG (e outros) — sites próprios
- TRFs — para matéria federal

### Bases pagas (mais robustas)
- Vlex, Jusbrasil Premium, Westlaw, RIB, Magister

## Estratégia de pesquisa

### 1. Identificar termos-chave da tese
- Substantivos centrais
- Sinônimos jurídicos
- Tema STF/STJ correspondente

### 2. Filtros úteis
- Tribunal
- Período (jurisprudência muda)
- Órgão julgador (Pleno > Turma)
- Repetitivo / repercussão geral

### 3. Validação cruzada
- Texto integral (não só ementa)
- Verificar se foi superado posteriormente
- Conferir modulação de efeitos

## Como citar

### Súmula (texto curto)
> "Súmula 297 STJ: O Código de Defesa do Consumidor é aplicável às instituições financeiras."

### Tema com repercussão geral / repetitivo
> "STF, RE 574.706, Tema 69, Min. Cármen Lúcia, repercussão geral, 15/03/2017: o ICMS não compõe a base de PIS/COFINS."

### Acórdão isolado
> "STJ, REsp 1.221.170/PR, Tema 779, 2ª Seção, Min. Sérgio Kukina, j. 22/02/2018: '...' (citar trecho relevante)."

### Mostrar vínculo lógico
Não basta colar a ementa — relacionar com o caso concreto:
> "No caso dos autos, identifica-se hipótese análoga à do Tema 779, pois o gasto com EPI é essencial à operação produtiva. Aplica-se, portanto, o entendimento que reconhece o crédito de PIS/COFINS sobre tal despesa, conforme..."

## Estrutura — relatório de pesquisa para uma tese

```
TESE: __________
CASO: __________ (resumo)

1. FONTE PRIMÁRIA (lei + CF)
   - Art. ___ da Lei __
   - CF art. ___

2. SÚMULAS VINCULANTES STF
   - Súm Vin. ___ — aplicável (síntese)

3. TEMAS COM REPERCUSSÃO GERAL STF
   - Tema ___ (RE ___): tese fixada — síntese
   - Status: [decidido / pendente / modulado]

4. TEMAS REPETITIVOS STJ
   - Tema ___ (REsp ___): tese — síntese

5. SÚMULAS STJ
   - Súm ___: aplicável

6. JURISPRUDÊNCIA DO TJ-__ E OUTROS TRIBUNAIS DE 2ª
   - Apelação ___ TJ-SP, Rel. ___, __/__/____: trecho
   - Apelação ___ TJ-RJ, Rel. ___: trecho

7. DOUTRINA
   - Autor X, Obra, p. __: "..."

8. ANÁLISE CRÍTICA
   - Pontos a favor da tese
   - Riscos / contraposições jurisprudenciais
   - Estratégia de fundamentação

9. CITAÇÕES PRONTAS PARA INSERIR NA PEÇA
   [trechos formatados]
```

## Cuidados

### Súmula superada
- Verificar data e revisões
- STJ tem súmulas canceladas que ainda aparecem em sistemas

### Modulação de efeitos
- STF Tema 69: efeitos a partir de 15/03/2017 → ações antigas têm sorte diferente
- Crucial: data de ajuizamento e data do trânsito em julgado

### Tese ainda em julgamento
- Tese pendente: fundamento mais frágil
- Pode-se pedir sobrestamento (CPC 982 § 2º)

### Distinguishing
- Demonstrar que o caso atual é diferente do precedente quando for desvantajoso

### Overruling
- Mudança de entendimento — fundamentar com decisões mais recentes

## Banco de citações úteis (top 10 por área)

### Cível / Consumidor
- Súm 297 STJ — CDC banks
- Súm 326 STJ — sucumbência
- Súm 362 STJ — correção dano moral
- Tema 929 STJ — repetição em dobro
- Tema 958 STJ — tarifas

### Trabalhista
- Súm 6 TST — equiparação
- Súm 60, 172 TST — DSR
- Súm 437 TST — intervalo intra
- Tema 1.046 STF — negociado x legislado
- Tema 725 STF — terceirização

### Tributário
- Tema 69 STF — ICMS PIS/COFINS
- Tema 779 STJ — insumos
- Tema 962 STF — IR sobre Selic
- Tema 1.067 STF — ISS PIS/COFINS
- Tema 568 STJ — prescrição intercorrente

### Previdenciário
- Tema 350 STJ — prévio req
- Tema 555 STF — ruído + EPI
- Tema 905 STJ — correção
- Tema 642 STJ — tempo rural

### Família / Sucessões
- Tema 809 STF — união estável
- Súm 358 STJ — exoneração alimentos
- Súm 277 STJ — alimentos

### Criminal
- Tema 1.099 STF — bagatela
- Tema 1.016 STJ — reconhecimento
- Súm 545 STF — confissão
- Súm 444 STJ — dosimetria
- Tema 1.052 STF — tráfico privilegiado

## Erros comuns

- Citar súmula cancelada.
- Colar ementa sem ler a íntegra.
- Citar Tema sem verificar modulação.
- Acumular precedentes sem distinguir relevância.
- Não fazer distinguishing quando o precedente é desfavorável.
- Citar doutrina sem citar lei e jurisprudência (insuficiente).

## Checklist

- [ ] Precedente vinculante aplicável (CPC 927)
- [ ] Súmulas pertinentes
- [ ] Acórdãos secundários (TJ, TRF)
- [ ] Doutrina complementar
- [ ] Distinguishing se necessário
- [ ] Citação correta (formal)
- [ ] Vinculação ao caso concreto

## Referências

- CPC art. 927 (precedentes obrigatórios)
- CF (todas as fontes)
- Lei 8.038/1990 (rito STF/STJ)
- Lei 11.418/2006 (repercussão geral)
- Regimentos internos STF, STJ, TST, TJs

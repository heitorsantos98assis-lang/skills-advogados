---
name: skills-advogados-contestacao-civel
description: "Estrutura contestação cível com toda a matéria de defesa (preliminares + mérito + reconvenção quando cabível) seguindo CPC arts. 335-343, no prazo de 15 dias úteis após audiência ou citação."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Codex, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Ao receber citação como réu em ação cível. **Prazo: 15 dias úteis** (CPC arts. 219 e 335) contados:
- Da audiência de conciliação (se houver) — sem acordo;
- Da última retratação de pedido de cancelamento da audiência;
- Da juntada do AR (citação postal) — em ações sem audiência;
- Da juntada do mandado cumprido (oficial de justiça);
- 60 dias para Fazenda Pública e MP (CPC 183).

## Inputs necessários

1. Petição inicial e documentos juntados pelo autor
2. Decisão saneadora ou despacho inicial
3. Comprovação de citação (AR, certidão de OJ, edital)
4. Documentos do cliente para defesa (contratos, comprovantes, atos administrativos)
5. Eventual decisão de antecipação de tutela
6. Procuração e contrato de honorários

## Estrutura

```
EXMO. SR. JUIZ DE DIREITO DA __ª VARA CÍVEL DA COMARCA DE __________

Processo nº __________

[QUALIFICAÇÃO DO RÉU]
__________ [réu], por seu procurador signatário (procuração inclusa), nos autos da ação __________ proposta por __________, nos termos dos artigos 335 e seguintes do CPC, vem oferecer

CONTESTAÇÃO

pelos fatos e fundamentos a seguir.

I — PRELIMINARES (CPC art. 337)
[apenas as cabíveis]
1.1. Inexistência ou nulidade da citação
1.2. Incompetência (absoluta ou relativa)
1.3. Incorreção do valor da causa
1.4. Inépcia da petição inicial
1.5. Perempção
1.6. Litispendência
1.7. Coisa julgada
1.8. Conexão / continência
1.9. Incapacidade da parte / irregularidade de representação
1.10. Convenção de arbitragem
1.11. Ausência de legitimidade ou interesse processual (CPC 17, 485 VI)
1.12. Falta de caução ou prestação devida
1.13. Indevida concessão da gratuidade
1.14. Prescrição / decadência (CPC 487 II)

II — DAS IMPUGNAÇÕES ESPECÍFICAS (CPC 341)
[Impugnar **especificamente** cada fato narrado pelo autor — fato não impugnado é presumido verdadeiro]
2.1. Quanto ao item ___ da inicial: [impugnação fundamentada]
2.2. Quanto ao item ___: [...]

III — DO MÉRITO
3.1. [Tese 1 — ex.: nulidade do contrato]
3.2. [Tese 2 — ex.: inadimplemento do autor]
3.3. [Tese 3 — ex.: caso fortuito / força maior]
[Fundamentar com lei + jurisprudência]

IV — DA RECONVENÇÃO [CPC 343, se houver]
4.1. Cabimento
4.2. Causa de pedir
4.3. Pedido reconvencional
4.4. Valor da reconvenção

V — DOS PEDIDOS
Diante do exposto, requer:
a) O acolhimento das preliminares para extinguir o processo sem resolução do mérito (CPC 485);
b) Subsidiariamente, a improcedência total dos pedidos da inicial;
c) [Se houver reconvenção] A procedência da reconvenção, condenando-se o autor-reconvindo a __________;
d) A condenação do autor ao pagamento de custas e honorários sucumbenciais (CPC 85);
e) A produção de todas as provas em direito admitidas, especialmente __________ (testemunhal, pericial, documental complementar).

[Local], [data]
________________________
[Advogado] OAB/__ nº ______
```

## Princípio da impugnação específica (CPC 341)

Cada fato narrado pelo autor precisa ser **especificamente impugnado**. Caso contrário, presume-se verdadeiro (com 3 exceções):
- Não admitir confissão;
- Quando o documento essencial for autêntico (escritura, sentença);
- Quando os fatos forem contraditórios entre si.

**Boa prática**: enumerar e impugnar cada fato, mesmo que para reafirmar o que é verdadeiro mas com outro contexto.

## Reconvenção (CPC 343)

- Apresentada na **mesma peça** da contestação (não mais como petição autônoma).
- Pedido contra o autor, decorrente do mesmo contrato/fato ou conexo.
- Valor da reconvenção: separado, com custas próprias.
- Réu reconvinte = autor. Autor reconvindo = réu.

## Provas (CPC 369-484)

### Documental
- Juntar com a contestação (CPC 434 — princípio da concentração).
- Documentos novos: só se posteriores ou destinados a contrapor (CPC 435).

### Testemunhal
- Rol de testemunhas: até 10, no máximo 3 por fato (CPC 357 §6º).
- Apresentação: na fase de saneamento, se solicitado pelo juiz, com 15 dias de antecedência da audiência.

### Pericial
- Solicitar e indicar quesitos no momento adequado.

## Honorários sucumbenciais (CPC 85)

- 10-20% sobre valor da condenação OU valor da causa.
- Em causas com Fazenda: faixas progressivas (CPC 85 § 3º).
- Honorários recursais (§ 11): adicional em caso de recurso desprovido.

## Cuidados estratégicos

### 1. Ordem das preliminares
Algumas preliminares, se acolhidas, encerram o processo (perempção, litispendência, coisa julgada). Outras só transferem ou suspendem (incompetência, conexão).

### 2. Prescrição/Decadência
Pode ser conhecida de ofício (CPC 487 II), mas é melhor alegar para garantir o tema.

### 3. Tutela já concedida
Se há tutela contra o réu, pedir reconsideração ou agravar (skill 04 — agravo de instrumento).

### 4. Audiência de conciliação
Pode interessar conciliar para evitar sucumbência maior. CPC 334 prevê multa de 2% por não comparecimento sem justificativa.

## Erros comuns

- Perder prazo de 15 dias → revelia (CPC 344) → presunção de veracidade dos fatos (não dos efeitos jurídicos).
- Defesa genérica ("nego todos os fatos") → impugnação específica não atendida.
- Esquecer prescrição/decadência.
- Reconvenção em peça separada → não é mais admitido (deve ser na contestação).
- Não enumerar testemunhas no momento certo.
- Pedir prova pericial sem antecipar quesitos e indicar assistente técnico.
- Documento essencial deixado para "depois" — CPC 434 (princípio da concentração) prejudica.

## Checklist

- [ ] Prazo de 15 dias úteis confirmado e respeitado
- [ ] Procuração e documentos do réu juntados
- [ ] Preliminares cabíveis listadas (CPC 337)
- [ ] Cada fato da inicial impugnado especificamente (CPC 341)
- [ ] Mérito com fundamentação legal e jurisprudencial
- [ ] Reconvenção (se cabível) na mesma peça
- [ ] Provas requeridas (documental, testemunhal, pericial)
- [ ] Pedido sucumbencial (CPC 85)
- [ ] Eventual pedido de gratuidade
- [ ] Protocolo no sistema do tribunal

## Referências

- CPC (Lei 13.105/2015) arts. 335-343 (resposta), 337 (preliminares), 341 (ônus de impugnação), 369-484 (provas), 85 (sucumbência), 334 (audiência), 487 II (prescrição/decadência)
- Súmulas STJ aplicáveis ao tema da defesa
- Lei 11.419/2006 (PJe)

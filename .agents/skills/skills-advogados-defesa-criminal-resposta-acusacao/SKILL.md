---
name: skills-advogados-defesa-criminal-resposta-acusacao
description: "Estrutura resposta à acusação (CPP 396 e 396-A) com exceções, preliminares, mérito, rol de testemunhas e indicação de provas, no prazo de 10 dias após citação."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Codex, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Após o **recebimento da denúncia/queixa** (ou despacho liminar de citação), o réu é citado para apresentar resposta escrita em **10 dias** (CPP 396).

Esta é a **primeira manifestação formal** de defesa após a fase de investigação. Crucial para afastar acusação infundada (rejeição da denúncia, absolvição sumária — CPP 397).

## Inputs necessários

1. Denúncia/queixa-crime + recebimento
2. Inquérito policial (cópia integral)
3. Documentos do cliente
4. Provas em poder do réu
5. Procuração ad judicia (CPC 105 + CPP 261)
6. Indicação de testemunhas (até 8 — CPP 401)

## Estrutura

```
EXMO. SR. JUIZ DA __ª VARA CRIMINAL DA COMARCA DE __________

Processo nº __________ — Acusação: __________
Réu: __________

Vem, por seu defensor (procuração inclusa), apresentar

RESPOSTA À ACUSAÇÃO

nos termos dos arts. 396 e 396-A do CPP, pelas razões a seguir.

I — PRELIMINARES (CPP 395 — rejeição da denúncia, e absolutórias do CPP 397)

1.1. Inépcia da denúncia (CPP 41 + 395 I)
   - Falta narração de circunstâncias essenciais
   - Pluralidade de réus sem individualização (Súm 1 STJ aplica subsidiariamente)
   - Imputação genérica
1.2. Falta de pressuposto processual ou condição da ação
1.3. Falta de justa causa (CPP 395 III)
   - Ausência de lastro probatório mínimo no IP
1.4. Litispendência / coisa julgada
1.5. Incompetência (CPP 69-83)
1.6. Causas de absolvição sumária (CPP 397):
   I. Existência manifesta de excludente de ilicitude
   II. Existência manifesta de excludente de culpabilidade
   III. Fato não constitui crime (atipicidade)
   IV. Extinta a punibilidade (prescrição, perempção, decadência)

II — DOS FATOS [se houver continuidade no mérito]
[Versão da defesa — relato cronológico]

III — DO MÉRITO
3.1. [Tese central — atipicidade, excludentes, dúvida razoável]
3.2. [Fundamentação legal e jurisprudencial]
3.3. [Indicação de provas]

IV — DAS TESTEMUNHAS
Arrola-se até 8 testemunhas (CPP 401):
1. ________________ qualificação, endereço
2. ________________
... (até 8)
[+ testemunhas referidas — CPP 209 § 1º]
[+ informantes — CPP 206]

V — DAS PROVAS REQUERIDAS
- Documental complementar (juntar)
- Pericial: solicitar perícia em [arma, corpo, locais, documentos, contábil] com quesitos (em anexo se for o caso)
- Acareação se houver contradição entre depoimentos
- Reconhecimento de pessoas/objeto (CPP 226 — controle do procedimento; STJ Tema 1.016)
- Reprodução simulada (CPP 7º)

VI — DOS PEDIDOS
a) O recebimento e processamento da resposta;
b) A absolvição sumária com base no CPP 397, hipótese __;
c) Subsidiariamente, a rejeição da denúncia (CPP 395);
d) Sucessivamente, a designação de audiência de instrução com oitiva das testemunhas arroladas.

[Local], [data]
________________________
[Defensor] OAB/__ ______
```

## Possíveis preliminares — exemplos

### 1. Inépcia da denúncia
- Não descreve modus operandi, dolo específico, ou individualiza conduta
- Imputação genérica em concurso de pessoas → defesa concreta inviabilizada (Súmula 1 STJ + jurisprudência)

### 2. Atipicidade material (insignificância)
- Bagatela: STF Tema 1.099 + critérios HC 84.412/SP
- Mínima ofensividade, ausência de periculosidade social, reduzido grau de reprovabilidade, inexpressividade da lesão

### 3. Excludente de ilicitude (CP 23)
- Legítima defesa
- Estado de necessidade
- Estrito cumprimento de dever legal
- Exercício regular de direito

### 4. Excludente de culpabilidade (CP 26-28)
- Inimputabilidade (doença mental)
- Erro inevitável sobre ilicitude
- Coação moral irresistível
- Embriaguez involuntária completa

### 5. Prescrição
- Da pretensão punitiva (CP 109): pelo máximo da pena cominada
- Retroativa (sentença condenatória): pela pena concretizada
- Súmula 438 STJ: prescrição em perspectiva (virtual) é inadmissível

## Provas

### Acreditação
- Custodial: encadeamento custodial documentado (apreensões, perícias)
- Reconhecimento: STJ Tema 1.016 — reconhecimento sem observância do CPP 226 é prova sem força para condenação isolada

### Quebra de sigilo
- Bancário, fiscal, telefônico, telemático: exige autorização judicial fundamentada
- Sem ordem judicial: prova ilícita (CF 5º LVI)

### Confissão
- Atenuante (CP 65 III "d") quando espontânea
- Pode ser revogada por qualquer meio admitido pelo direito

## Erros comuns

- Não levantar todas as preliminares possíveis nesta fase (preclusão).
- Esquecer rol de testemunhas → preclusão (CPP 401).
- Repetir matéria de mérito sem confrontar a denúncia.
- Não apontar atipicidade e excludentes mesmo quando claros.
- Pleitear prova pericial sem indicar quesitos.
- Não juntar documentos à resposta (CPP 396-A).
- Defesa silente sobre o concurso de pessoas no fato.
- Não distinguir testemunha de informante (familiar próximo).

## Checklist

- [ ] Denúncia + IP analisados
- [ ] Procuração específica
- [ ] Preliminares aplicáveis (CPP 395 e 397)
- [ ] Tese de mérito clara
- [ ] Rol de testemunhas (até 8)
- [ ] Provas indicadas com fundamento
- [ ] Documentos juntados
- [ ] Pedido absolutório sumário ou rejeição
- [ ] Pedido subsidiário de instrução
- [ ] Protocolo no PJe-Crim ou e-SAJ Criminal

## Referências

- CPP arts. 41, 261, 395, 396, 396-A, 397, 401, 405, 406
- CP arts. 23-28, 65, 107-119
- CF 5º LV, LVI, LVII (devido processo)
- Súmulas STJ 1, 438
- Tema 1.016 STJ (reconhecimento — CPP 226)
- HC 84.412/SP STF (bagatela)

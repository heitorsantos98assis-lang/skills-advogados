---
name: skills-advogados-reclamacao-trabalhista-inicial
description: "Estrutura reclamação trabalhista (CLT 840 + CPC subsidiário) com pedido líquido (Lei 13.467/17), narrativa cronológica, jus postulandi vs. advogado, e cálculo discriminado das verbas."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Claude, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Empregado com vínculo (CLT, doméstico, rural, terceirizado) reivindicando verbas não pagas, reconhecimento de vínculo, horas extras, equiparação salarial, danos morais, rescisão indireta etc. Prazo: **2 anos** após extinção do contrato (CF art. 7º XXIX).

Imprescritibilidade aparente: prazo bienal para ajuizar; prazo quinquenal para verbas (5 anos retroativos da data do ajuizamento). Verbas anteriores aos 5 anos prescritas.

## Inputs necessários

1. Cliente reclamante (qualificação completa)
2. Reclamado/empregador (CNPJ, endereço, eventual grupo econômico)
3. CTPS digital, contracheques, controle de ponto
4. Datas: admissão, demissão (se houver), motivo
5. Salário e variáveis (HE, comissões)
6. Documentos das pretensões (atestados, e-mails, prints, testemunhas)
7. Sindicato e CCT/ACT vigente
8. Tentativa extrajudicial / Comissão de Conciliação Prévia (CCP — se setor tiver)

## Pedido líquido (Lei 13.467/2017 — CLT 840 § 1º)

- Cada pedido deve vir com **valor certo** ou indicação de cálculo.
- Fundamento: facilita a celeridade e a sucumbência.
- Exceção (ressalvada): se a apuração depende de informação que só a empresa tem (cartão de ponto), pode-se indicar limites mínimos.

## Estrutura

```
EXMO. SR. JUIZ DA __ª VARA DO TRABALHO DE __________

[QUALIFICAÇÃO DO RECLAMANTE]
__________ [reclamante], [nacionalidade, estado civil, profissão], CPF __________, CTPS __________ série ___, residente em __________, [pode ser representado pelo sindicato OU advogado outorgado por procuração], vem propor

RECLAMAÇÃO TRABALHISTA

em face de __________ [reclamada], CNPJ __________, com sede em __________, pelos motivos a seguir.

I — DOS FATOS
1. Admissão em __/__/____ na função de __________ (CBO ___), com salário inicial de R$ ___.
2. [Descrever rotina: jornada, função, evolução salarial, eventos relevantes]
3. Demissão / desligamento em __/__/____ (motivo: ____). [Se ainda empregado: continuar trabalhando]
4. [Pretensões — pelo menos uma das seguintes]:
   a) Não pagamento de verbas rescisórias
   b) Horas extras não pagas
   c) Equiparação salarial (CLT 461)
   d) Adicional não pago (insalubridade, periculosidade, noturno)
   e) Reconhecimento de vínculo (pejotização)
   f) Acúmulo de função
   g) Dano moral por assédio
   h) Rescisão indireta (CLT 483)

II — DO DIREITO
2.1. [Fundamentação por pedido]
2.2. CCT/ACT vigente (cláusula __ — anexo)
2.3. Súmulas TST aplicáveis

III — DOS PEDIDOS (LÍQUIDOS)
Diante do exposto, requer:

a) Notificação da reclamada para audiência (CLT 841);
b) Procedência para condenar a reclamada ao pagamento das seguintes verbas:

   1. Saldo de salário (___ dias): R$ _________
   2. Aviso prévio indenizado (___ dias — Lei 12.506/2011): R$ _________
   3. 13º proporcional (___ avos): R$ _________
   4. Férias proporcionais (___ avos) + 1/3: R$ _________
   5. Férias vencidas (___ período) + 1/3: R$ _________
   6. Multa do art. 477 § 8º CLT: R$ _________
   7. Multa do art. 467 CLT (50% sobre verbas incontroversas): R$ _________
   8. Horas extras com adicional de 50% (___ HE × valor) + reflexos em 13º, férias, FGTS, DSR: R$ _________
   9. Adicional [insalubridade/periculosidade/noturno]: R$ _________
   10. FGTS: depósitos em atraso + multa 40% (sobre saldo + parcelas em atraso): R$ _________
   11. Dano moral: R$ _________
   12. Honorários sucumbenciais (CLT 791-A): __% sobre o valor liquidado, com acréscimo de honorários contratuais já pactuados.

c) Liberação do FGTS (saque) e habilitação ao seguro-desemprego (skill 24);
d) Compensação tributária e previdenciária na forma da lei;
e) Justiça gratuita (CLT 790 § 3º);
f) Produção de prova testemunhal (rol em audiência), documental e pericial (insalubridade/periculosidade);

IV — DO VALOR DA CAUSA
R$ __________ (soma dos pedidos líquidos)
```

## Cálculo de horas extras

```
Jornada contratual: __ horas/dia, __ horas/sem
Jornada efetiva (cartão): __ horas/dia
HE diária = (Efetiva − Contratual) horas

Valor da hora normal = Salário / 220 (CLT 64)
HE 50% = Valor hora × 1,5
HE 100% = Valor hora × 2 (domingos/feriados, ou conforme CCT)

Reflexos:
+ DSR (Súm 60 e 172 TST)
+ 13º proporcional ao mês com HE
+ Férias + 1/3
+ FGTS 8%
+ INSS sobre HE
```

## Pretensões com regras especiais

### Equiparação salarial (CLT 461)
- Mesma função, mesma localidade, mesma empresa, diferença ≤ 4 anos no exercício, ≤ 2 anos no emprego, mesma produtividade e perfeição técnica.
- Lei 13.467/17 reformou: agora limita ao mesmo estabelecimento.

### Insalubridade × Periculosidade
- Insalubridade: exposição a agentes nocivos (NR-15) — 10/20/40% do salário-mínimo (Súm 228 TST suspensa: STF Tema 1.075 — base de cálculo é o SM).
- Periculosidade: exposição a perigo (NR-16) — 30% do salário base.
- Empregado pode escolher a mais vantajosa, **não cumula**.
- Exigem perícia técnica.

### Vínculo de emprego (pejotização — Súmula 363 TST e jurisprudência atual)
- Provar: pessoalidade, subordinação, habitualidade, onerosidade.
- ATENÇÃO: STF tem confirmado pejotização lícita em vários casos (Tema 725 RE 958.252) — terceirização da atividade-fim. Cuidado com a tese.

### Dano moral trabalhista
- Assédio moral, sexual, condições degradantes, exposição vexatória.
- Lei 13.467/17 trouxe parâmetros (CLT 223-G § 1º) — alíquotas conforme grau (leve, médio, grave, gravíssimo) — mas STF Tema 1.121 declarou inconstitucional os parâmetros tarifados.

### Rescisão indireta (CLT 483)
- Quando empregador comete falta grave: descumprimento contratual, agressão, exposição a perigo.
- Empregado para de trabalhar e pleiteia em juízo. Risco: se improcedente, vira pedido de demissão.

## Erros comuns

- Pedido genérico sem valor → CLT 840 §1º exige liquidação.
- Esquecer reflexos das HE.
- Pretensão prescrita (mais de 5 anos para trás) → corrigir.
- Pejotização sem prova robusta dos requisitos → improcedência + sucumbência.
- Pedido de dano moral sem narrativa concreta do assédio.
- Não anexar CCT vigente — base de muitas verbas.
- Equiparação sem mesma localidade e mesmo estabelecimento (pós-reforma).
- Justiça gratuita: empregado com salário > 40% do teto INSS precisa comprovar (CLT 790 § 4º).

## Checklist

- [ ] Documentos: CTPS, contracheques, ponto, CCT
- [ ] Cada pedido com valor líquido (CLT 840 §1º)
- [ ] Reflexos de HE/adicionais
- [ ] Multas (477 §8º, 467, 50% rescisão)
- [ ] FGTS + multa 40%
- [ ] CCT vigente anexa
- [ ] Procuração e justiça gratuita
- [ ] Rol de testemunhas para audiência (3 por fato — CPC 357)
- [ ] Perícia (insalubridade/periculosidade)
- [ ] Honorários sucumbenciais (CLT 791-A)
- [ ] Foro: do local da prestação ou domicílio do empregado (CLT 651)

## Referências

- CLT — toda
- Lei 13.467/2017 (Reforma Trabalhista)
- Lei 12.506/2011 (aviso prévio)
- CF 7º XXIX (prescrição)
- Súmulas TST 6, 60, 85, 172, 228, 264, 437
- Tema 725 STF (terceirização)
- Tema 1.075 STF (base insalubridade)
- Tema 1.121 STF (tarifa dano moral)

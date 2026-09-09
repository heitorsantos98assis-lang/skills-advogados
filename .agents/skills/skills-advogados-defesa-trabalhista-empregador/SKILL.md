---
name: skills-advogados-defesa-trabalhista-empregador
description: "Estrutura defesa do empregador (CLT 847) com preliminares, impugnação ponto a ponto, prova documental concentrada, rol de testemunhas, contradita e estratégia de instrução."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Claude, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Defesa em processo trabalhista. Apresentada **na audiência una** (CLT 847) ou no prazo definido pelo juízo (geralmente até a audiência). PJe permite protocolização prévia — recomendável.

## Inputs necessários

1. Reclamação trabalhista + documentos do reclamante
2. Pasta funcional do empregado (admissão, contracheques, ponto, ASOs, CCT)
3. Apuração das verbas pagas (rescisão, FGTS extrato)
4. Testemunhas potenciais (3 por fato)
5. Política interna (regulamento, manual, código de conduta)
6. Procuração com poderes para receber citação e firmar acordo
7. Carta de preposição (CLT 843 § 1º — empregado tem que ser preposto designado por escrito)

## Preposto

- O preposto representa o empregador na audiência.
- Lei 13.467/17 + Súmula 377 TST cancelada: **não precisa ser empregado**, pode ser pessoa indicada para isso (mas precisa **conhecer os fatos**).
- Carta de preposição assinada anexa.

## Estrutura

```
EXMO. SR. JUIZ DA __ª VARA DO TRABALHO DE __________

Processo nº __________

Reclamada: __________
Reclamante: __________

Vem, por seu procurador (procuração e carta de preposição em anexo), apresentar

DEFESA / CONTESTAÇÃO

às pretensões da reclamação, pelos motivos abaixo.

I — PRELIMINARES (CPC 337 + CLT)
1.1. Inépcia da inicial (faltam pedidos líquidos — CLT 840 § 1º)
1.2. Incompetência (territorial / material)
1.3. Ilegitimidade passiva (grupo econômico mal indicado)
1.4. Prescrição quinquenal (verbas anteriores a 5 anos do ajuizamento — CF 7º XXIX)
1.5. Coisa julgada / litispendência
1.6. Carência de ação

II — IMPUGNAÇÃO ESPECÍFICA AOS FATOS (CPC 341)
[Cada fato narrado pelo reclamante: confessar, negar com prova, ou explicar contexto]

2.1. Quanto à admissão e função: [confirmar/divergir]
2.2. Quanto à jornada: [apresentar cartão de ponto, regime — turno ininterrupto de revezamento, banco de horas]
2.3. Quanto às horas extras: [pagas conforme contracheques, OU acordo de compensação válido — CLT 59-A; OU jornada efetivamente inferior ao alegado]
2.4. Quanto aos adicionais: [pagos / não devidos por inexistir agente]
2.5. Quanto aos reflexos: [bases de cálculo aplicadas]

III — DO MÉRITO POR PEDIDO

3.1. Verbas rescisórias: pagas em __/__/____ (TRCT anexo). Improcedência.
3.2. Aviso prévio: indenizado ou trabalhado, conforme TRCT.
3.3. Horas extras: 
    a) controle de ponto anexo, jornada conforme CCT
    b) acordo de compensação (Súm 85 TST) ou banco de horas
    c) pagamento de eventuais HE conforme contracheques
3.4. Adicional insalubridade:
    a) NR-15 não preenchida no setor (ASOs e LTCAT anexos)
    b) Foi fornecido EPI (CLT 191 II) — neutralização (Súm 80 TST e jurisprudência)
3.5. Adicional periculosidade:
    a) Não há contato habitual com agente perigoso (NR-16)
3.6. Equiparação salarial: improcedente — paradigma trabalha em setor diferente / mais antigo / mais produtivo (CLT 461 com redação Lei 13.467)
3.7. Dano moral: 
    a) Inexistência de assédio
    b) Tratamento profissional dentro dos limites
    c) Reclamante não comprova abalo
3.8. Vínculo de emprego (pejotização): improcedente — relação foi de prestação de serviço autônomo, sem subordinação habitual, conforme contrato de prestação de serviço (anexo)
3.9. FGTS: regularmente depositado (extrato CAIXA anexo)

IV — DOS PEDIDOS COMPLEMENTARES
[Eventuais pedidos da reclamada, como reconvenção em raros casos]

V — DA PRODUÇÃO DE PROVA
- Documental concentrada (já anexada)
- Testemunhal: rol será apresentado em audiência (3 por fato)
- Pericial (se houver insalubridade/periculosidade)

VI — DOS PEDIDOS
Diante do exposto, requer:
a) O acolhimento das preliminares;
b) Subsidiariamente, a improcedência total dos pedidos;
c) Eventual procedência parcial deve respeitar a prescrição quinquenal;
d) Honorários sucumbenciais à reclamada (CLT 791-A);
e) Os benefícios da prova testemunhal e demais provas em direito admitidas;
f) Compensação de eventuais valores pagos a maior.

[Local], [data]
________________________
[Advogado] OAB/__ ______
```

## Documentos essenciais a juntar

- Pasta funcional completa
- Contrato de trabalho assinado
- Aditivos e termos
- Contracheques de todos os meses (5 anos)
- Cartões de ponto (5 anos — CLT 74 § 2º; obrigatório para empresa > 20 empregados)
- TRCT + GRRF + comprovantes
- ASOs (admissional, periódico, demissional)
- LTCAT (laudo técnico das condições ambientais — para insalubridade/periculosidade)
- CCT/ACT vigentes
- Comprovantes FGTS (extrato CAIXA)
- Atestados, advertências, suspensões
- Política interna assinada pelo empregado

## Estratégia de instrução

### Audiência una (rito sumário)
- 1ª tentativa de conciliação
- Defesa apresentada
- Prova oral (testemunhas)
- 2ª tentativa de conciliação
- Sentença

### Audiência inicial + instrução (rito ordinário)
- 1ª: tentativa de acordo + defesa
- Designada audiência de instrução
- Testemunhas (3 por fato), perito, depoimento das partes
- Razões finais
- Sentença

## Erros comuns

- Carta de preposição esquecida → preposto sem representação válida (Súm 377 TST cancelada, mas preposição formal continua sendo exigida).
- Documentos juntados intempestivamente → preclusão.
- Cartão de ponto britânico (entrada e saída sempre iguais) → invalidado (Súm 338 TST).
- Acordo de compensação sem CCT/ACT — pode ser invalidado.
- Não impugnar especificamente um pedido → presunção (CPC 341 aplica subsidiariamente).
- Pedir prova pericial sem indicar agente / sem suportar honorários (CLT 790-B reforma).
- Subestimar prescrição — alegar e quantificar o que prescreveu.
- Empresa de grupo econômico não citada — pedir nulidade.

## Checklist

- [ ] Procuração + carta de preposição
- [ ] Pasta funcional completa
- [ ] Contracheques 5 anos
- [ ] Cartões de ponto 5 anos
- [ ] CCT/ACT vigente(s)
- [ ] LTCAT/PPRA/PCMSO se aplicável
- [ ] Comprovantes de pagamento (FGTS, INSS)
- [ ] Preliminares cabíveis
- [ ] Impugnação ponto a ponto
- [ ] Prescrição alegada (5 anos)
- [ ] Rol de testemunhas pronto para a audiência
- [ ] Eventual perícia requerida
- [ ] Sucumbência (CLT 791-A)

## Referências

- CLT — toda, especialmente arts. 477, 482, 483, 59, 59-A, 461, 191, 195, 790, 790-B, 791-A, 818-A, 840, 841, 843, 847
- Lei 13.467/2017 (Reforma)
- Súmulas TST 6, 80, 85, 90, 113, 124, 264, 338, 366, 437
- CPC arts. 337, 341, 369-484 (subsidiariamente)

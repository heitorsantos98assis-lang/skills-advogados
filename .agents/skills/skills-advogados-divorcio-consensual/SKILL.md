---
name: skills-advogados-divorcio-consensual
description: "Estrutura divórcio consensual judicial ou extrajudicial (Lei 11.441/2007), com partilha de bens, alimentos, guarda dos filhos menores, regime de bens e cláusulas de proteção."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Codex, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Casal **de pleno acordo** sobre todos os pontos: divórcio, partilha, alimentos, guarda, visita.

Pode ser:
- **Extrajudicial** (cartório de notas) — Lei 11.441/2007 + Resolução CNJ 35/2007 + Lei 14.382/2022:
  - Sem filhos menores ou incapazes (mas se forem maiores ou nascituro com decisão judicial autorizando, pode!)
  - Mesmo com filhos menores se já há decisão judicial sobre alimentos/guarda
  - Casal assistido por advogado
  - Documento público (escritura)
- **Judicial** quando houver:
  - Filhos menores ou incapazes sem decisão prévia
  - Discordância em qualquer ponto (vira litigioso)
  - Pleno consenso, mas alguma especialidade (cliente prefere o juiz)

## Inputs necessários

1. Certidão de casamento atualizada (90 dias)
2. Documentos pessoais de ambos (RG, CPF, comprovante de endereço)
3. Pacto antenupcial (se houver)
4. Lista de bens e dívidas (com avaliação)
5. Documentação dos filhos (RG, certidão nascimento)
6. Acordo escrito sobre alimentos, guarda, visita
7. Procuração com poderes específicos (CPC 105 + Lei 11.441 — assistência obrigatória de advogado)

## Regimes de bens (CC 1.639-1.688)

| Regime | Bens comuns | Bens próprios |
|---|---|---|
| Comunhão parcial (padrão pós 1977) | Bens adquiridos onerosamente na constância | Anteriores, doações, heranças, sub-rogação |
| Comunhão universal | Todos | Apenas alguns excepcionados (uso pessoal, doações com cláusula) |
| Separação total | Nenhum | Todos próprios |
| Separação obrigatória (CC 1.641) | Idosos +70, casamentos com causa suspensiva, sem prévio inventário | Súmula 377 STF: aquestos comunicáveis com prova de esforço comum |
| Participação final dos aquestos | No fim, partilha aquestos | Durante, separação |

## Estrutura — divórcio extrajudicial (escritura)

```
ESCRITURA PÚBLICA DE DIVÓRCIO CONSENSUAL

Aos __ dias do mês de __ de 20__, na cidade de __________, perante mim, Tabelião do __º Tabelionato de Notas, comparecem:

[CÔNJUGE A] (qualificação completa, assistido por adv. Dr. ____ OAB/__ ___)
[CÔNJUGE B] (qualificação, assistido por adv. Dr. ____ OAB/__ ___)

Casados em __/__/____, sob o regime de __________, conforme certidão de casamento anexa.

Os comparecentes, livres e capazes, declaram que decidem dissolver o casamento por divórcio direto consensual, com fundamento na CF art. 226 § 6º (EC 66/2010) e na Lei 11.441/2007.

CLÁUSULA 1ª — DISSOLUÇÃO DO VÍNCULO
Fica dissolvido o casamento havido entre as partes, encerrando-se todos os deveres do art. 1.566 do CC.

CLÁUSULA 2ª — RETOMADA DO NOME DE SOLTEIRO
[Cônjuge A] retoma seu nome de solteiro: __________ / [Cônjuge A] mantém o nome de casado.

CLÁUSULA 3ª — DA PARTILHA DOS BENS
Constituem o patrimônio comum:
3.1. Imóvel matrícula nº __ do __º Cartório de Imóveis: caberá a __________
3.2. Veículo placa __, RENAVAM __: caberá a __________
3.3. Saldo conta nº __ banco __: divisão 50% / 50%
3.4. (...)

CLÁUSULA 4ª — DAS DÍVIDAS
4.1. Financiamento imóvel: ficará por conta de __________
4.2. (...)

CLÁUSULA 5ª — DOS ALIMENTOS ENTRE CÔNJUGES
[Há ou não há pensão alimentícia entre cônjuges. Se houver: valor, forma, prazo]

CLÁUSULA 6ª — DOS FILHOS MAIORES
Os filhos maiores são __________. Não há disposição sobre alimentos / guarda (não se aplica em escritura).

CLÁUSULA 7ª — DA EFICÁCIA E DOS REGISTROS
Esta escritura tem eficácia imediata e independe de homologação judicial. Será averbada na certidão de casamento e nas matrículas dos imóveis.

___________________
Cônjuge A

___________________
Cônjuge B

___________________
Adv. A — OAB ___

___________________
Adv. B — OAB ___

___________________
Tabelião
```

## Estrutura — divórcio consensual judicial

```
EXMO. SR. JUIZ DE DIREITO DA __ª VARA DA FAMÍLIA E SUCESSÕES DA COMARCA DE __________

[CÔNJUGES A e B], qualificados, casados em __/__/____ sob regime __________, vêm, em conjunto e por seus procuradores constituídos (procurações em anexo), com fulcro na CF 226 §6º e nos arts. 731 e seguintes do CPC, propor

DIVÓRCIO CONSENSUAL

formulando os seguintes pedidos:

I — DOS FATOS
1. As partes contraíram matrimônio em __/__/____, conforme certidão (doc. ___).
2. Têm os seguintes filhos: __________ (menor com __ anos) — ou nenhum.
3. Constituíram o patrimônio descrito a seguir e estão de pleno acordo quanto à dissolução, partilha, guarda, alimentos e visita.

II — DOS PEDIDOS
a) Decretação do divórcio direto consensual, com retomada do nome de solteiro pelo cônjuge __________ / manutenção do nome;
b) Homologação da partilha dos bens nos seguintes termos: [listar];
c) Homologação do acordo sobre os filhos:
   c.1) Guarda compartilhada com lar de referência com __________
   c.2) Convivência (visita) ao genitor não-residente: [esquema detalhado, fins-de-semana alternados, períodos de férias, datas comemorativas]
   c.3) Alimentos: __% do salário-mínimo / __% dos rendimentos líquidos do alimentante / R$ ___, depositados até o dia __ de cada mês na conta __________
   c.4) Plano de saúde mantido pelo genitor __________
   c.5) Despesas extraordinárias (escola, médico, etc.): rateio na proporção __ / __
d) Concessão da gratuidade de justiça (se aplicável) ou recolhimento de custas;
e) Audiência de ratificação dispensada (CPC 731 § ún), por se tratar de pedido consensual com instrução documental completa;
f) Expedição de mandado de averbação ao cartório de registro civil;
g) Atualização das matrículas dos imóveis no respectivo CRI.

III — DO VALOR DA CAUSA
R$ __________ (CPC 292 — soma do patrimônio partilhado / valor estimado).
```

## Cuidados na partilha

### Avaliação
- Imóveis: avaliação de corretor ou ITBI/IPTU
- Veículos: tabela FIPE
- Empresas: balanço + skill contadora 48 (valuation PME)
- Bens móveis: valor estimado de mercado

### Sub-rogação
- Bem adquirido com dinheiro pré-casamento → próprio (provar)
- Sub-rogação cuidadosa para não cair na presunção de comunhão

### Partilha desigual
- Permitida (dispositivo das partes), mas atenção:
  - Doação ao cônjuge: pode incidir ITCMD do estado
  - Excessiva = doação tributável

### Bens omitidos
- Sobrepartilha futura sempre possível (CC 1.040)

## Cláusulas comuns adicionais

- **Manutenção do plano de saúde**: cônjuge dependente continua até prazo definido
- **Pensão temporária**: alimentos transitórios entre cônjuges para ajuste econômico
- **Direito real de habitação**: viúvo/divorciado vulnerável (CC 1.831)
- **Cláusula de não concorrência** (em divórcio empresarial)

## Erros comuns

- Filhos menores sem prévia decisão sobre alimentos/guarda → cartório nega; ir ao judicial.
- Bem omitido → futura sobrepartilha gera nova disputa.
- Avaliação subdimensionada → ITCMD a maior cobrado posteriormente / um dos cônjuges questiona.
- Pacto antenupcial não juntado → regime presumido errado.
- Pensão entre cônjuges definida como vitalícia sem cláusula de revisão.
- Não averbar a sentença/escritura no registro civil — divórcio "existe" mas não aparece na certidão.
- Não atualizar matrículas dos imóveis — bem ainda em nome de ambos.

## Checklist

- [ ] Certidão de casamento atualizada
- [ ] Documentos pessoais e dos filhos
- [ ] Pacto antenupcial (se houver)
- [ ] Lista completa de bens com avaliação
- [ ] Lista de dívidas
- [ ] Acordo sobre filhos (guarda + visita + alimentos)
- [ ] Forma: extrajudicial cabível? (sem menores ou já decidido)
- [ ] Procurações específicas para divórcio
- [ ] ITBI/ITCMD avaliados (se partilha desigual)
- [ ] Cláusulas patrimoniais protetivas
- [ ] Averbação no registro civil agendada
- [ ] Atualização de matrículas/RENAVAM

## Referências

- CF art. 226 § 6º (EC 66/2010)
- CC arts. 1.571-1.582, 1.639-1.688, 1.821-1.832, 1.040
- CPC arts. 731-734
- Lei 11.441/2007 (extrajudicial)
- Lei 14.382/2022 (atualização)
- Resolução CNJ 35/2007 (procedimentos)
- Súmula 377 STF (aquestos)

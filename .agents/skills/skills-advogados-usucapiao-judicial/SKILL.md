---
name: skills-advogados-usucapiao-judicial
description: "Estrutura ação de usucapião judicial (CC 1.238-1.244 + CPC 246-249) quando há litígio ou ausência de anuência, com citação dos confinantes, intimação das Fazendas e perícia."
---

## Compatibilidade Codex

Leia primeiro as instruções `AGENTS.md` aplicáveis e inspecione a stack real do projeto. Preserve escolhas explícitas do usuário e convenções existentes. As tecnologias citadas abaixo são preferências do material de origem, não autorização para substituir a stack atual.

Use as ferramentas disponíveis no Codex. Não presuma nomes de ferramentas do Codex, não exponha segredos e não execute publicação, envio, exclusão ou mudanças externas sem a autorização apropriada.

Para conteúdo jurídico, contábil, de engenharia ou arquitetura, valide normas atuais em fontes oficiais e trate a saída como rascunho sujeito a revisão profissional.

## Quando usar

Mesmas hipóteses da skill 45, mas em casos onde:
- Algum titular anterior ou confinante não anuiu
- Imóvel sem matrícula identificável
- Há litígio com terceiros
- Imóvel rural extenso
- Peculiaridades que demandem instrução probatória

## Inputs necessários

(Mesmos da extrajudicial, mas adaptados para juízo)

1. Documentos pessoais do requerente
2. Planta georreferenciada e memorial descritivo
3. Comprovação da posse (mínimo 5 testemunhas, fotos, IPTU, contas)
4. Documentos da matrícula (se conhecido)
5. Identificação dos confinantes
6. Eventual justo título
7. Procuração

## Estrutura

```
EXMO. SR. JUIZ DA __ª VARA CÍVEL / DE REGISTROS PÚBLICOS DA COMARCA DE __________

[REQUERENTE]

vem propor

AÇÃO DE USUCAPIÃO

com fundamento nos arts. 1.238 e seguintes do Código Civil, pelos motivos a seguir.

I — DOS FATOS
1. O autor exerce posse mansa, contínua e pacífica do imóvel localizado em __________ desde __/__/____, totalizando __ anos.
2. Trata-se de imóvel [urbano / rural] com área de __ m², descrito no memorial anexo (georreferenciado).
3. Posse com animus dominil — utiliza para __________ (moradia, comércio, agricultura).
4. [Se ordinária]: Possui justo título — escritura/promessa anexa.
5. Imóvel é objeto da matrícula __ do __º CRI, em nome de __________ (titular cuja localização é __________).

II — DO DIREITO
2.1. Da posse e da usucapião (CC 1.238-1.244)
2.2. Da modalidade aplicável: [Extraordinária / Ordinária / Especial Urbana (CF 183) / Especial Rural (CF 191) / Familiar (CC 1.240-A)]
2.3. Do prazo cumprido
2.4. Do animus dominil

III — DOS PEDIDOS
a) Citação:
   a.1) Dos titulares registrais (atual e anteriores)
   a.2) Dos confinantes do imóvel:
      - Norte: __________
      - Sul: __________
      - Leste: __________
      - Oeste: __________
   a.3) De terceiros eventualmente interessados, por edital (CPC 259 III)
b) Intimação das Fazendas Federal, Estadual e Municipal (CPC 246 § 3º + Lei 6.015 art. 213-A);
c) Intimação do MP (Lei 6.015 art. 213-A § 3º — em algumas hipóteses);
d) Procedência para:
   d.1) Declarar a aquisição da propriedade pelo autor por usucapião na modalidade __;
   d.2) Determinar o registro/matrícula em nome do autor no CRI;
e) Provas: documental, testemunhal, pericial (vistoria, georreferenciamento);
f) Custas e gratuidade (se aplicável).

IV — DO VALOR DA CAUSA
R$ __________ (valor venal do imóvel — ITR/IPTU)
```

## Particularidades processuais

### Citação dos confinantes (CPC 246)
- Pessoal por mandado
- Por edital se desconhecidos / em local incerto

### Intimação das Fazendas
- Federal (União), Estadual, Municipal
- Manifestação em 15 dias

### Justa causa para usucapir
- Posse mansa = sem oposição
- Contínua = sem interrupções voluntárias
- Pacífica = sem violência
- Com animus dominil = como se fosse dono

### Soma de posses (accessio possessionis)
- Possuidor pode somar a posse do antecessor (CC 1.243)
- Útil quando comprou de quem tinha posse iniciada antes

### Imóvel em nome de morto
- Usucapir contra espólio: possível, mas inventário pode complicar
- Prazo continua correndo

### Reforma agrária / Funai
- Áreas indígenas e quilombolas: reflexões adicionais

## Modalidades — detalhes

### Extraordinária (CC 1.238)
- 15 anos
- 10 anos se moradia / serviços produtivos no imóvel
- Sem necessidade de justo título / boa-fé

### Ordinária (CC 1.242)
- 10 anos
- 5 anos se imóvel adquirido onerosamente, com base em registro cancelado, e estabelecida moradia ou investimentos de interesse social
- Necessita justo título + boa-fé

### Especial Urbana (CF 183 + CC 1.240)
- 5 anos
- Área urbana ≤ 250 m²
- Moradia
- Não possui outro imóvel urbano ou rural
- Não pode ser concedida 2 vezes ao mesmo possuidor

### Especial Rural (CF 191 + CC 1.239)
- 5 anos
- Área rural ≤ 50 ha
- Produção agrícola
- Moradia da família
- Não pode ser proprietário de outro imóvel rural ou urbano

### Familiar (CC 1.240-A)
- 2 anos (mais curto)
- Cônjuge/companheiro com posse direta + abandono pelo outro
- Imóvel urbano ≤ 250 m², copropriedade
- Não possui outro imóvel

## Pericia técnica

- Engenheiro/agrimensor
- Vistoria do imóvel
- Confirmação de área e marcos

## Erros comuns

- Não citar todos os confinantes → nulidade.
- Esquecer Fazendas (CPC 246 § 3º).
- Modalidade trocada (alegar especial sem cumprir requisito de "único imóvel").
- Posse interrompida por afastamento prolongado.
- Justo título vencido (descobrir vício antes pode descaracterizar boa-fé).
- Imóvel registrado em nome de PJ pública → não cabe.
- Imóvel sob hipoteca (restou com gravame).
- Não juntar planta georreferenciada — sentença fica vaga.

## Checklist

- [ ] Modalidade identificada e fundamentada
- [ ] Posse comprovada (5+ testemunhas, IPTU, contas)
- [ ] Planta georreferenciada
- [ ] Confinantes identificados
- [ ] Citação por mandado e/ou edital
- [ ] Intimação das Fazendas
- [ ] Justo título (se ordinária)
- [ ] Pedido de registro no CRI
- [ ] Custas / gratuidade
- [ ] Procuração

## Referências

- CC arts. 1.238-1.244, 1.240-A
- CF arts. 183, 191
- CPC arts. 246, 259, 357 (saneamento)
- Lei 6.015/1973 (Registros Públicos) art. 213-A
- Súmulas STJ 11, 73, 197, 391; STF 340

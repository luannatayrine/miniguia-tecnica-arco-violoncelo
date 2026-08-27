# Cicatrizes e Troubleshooting

## 1. Sobre esta seção

Esta seção registra as dificuldades encontradas durante o desenvolvimento do projeto e as estratégias utilizadas para solucioná-las.

O objetivo não é apresentar apenas o resultado final da pesquisa, mas tornar visível parte do processo de construção do conhecimento com apoio da Inteligência Artificial.

Durante o desenvolvimento do projeto, percebeu-se que obter uma resposta sobre determinado assunto não significava necessariamente obter uma resposta adequada para o objetivo da pesquisa.

Em diferentes momentos, foi necessário:

* restringir o escopo das perguntas;
* especificar as fontes que deveriam ser utilizadas;
* solicitar a identificação das evidências;
* verificar respostas anteriores;
* separar informações diretamente apresentadas pelas fontes de interpretações;
* reformular prompts;
* eliminar conclusões que não apresentavam sustentação suficiente.

Assim, as "cicatrizes" representam os problemas encontrados durante o processo e as mudanças realizadas para melhorar a qualidade da investigação.

---

# 2. O que significa "cicatriz" neste projeto?

Neste projeto, uma **cicatriz** é um registro de uma dificuldade que ocorreu durante a pesquisa e que provocou alguma mudança na estratégia de investigação.

Uma cicatriz pode surgir quando:

* uma pergunta produz uma resposta ampla demais;
* a IA apresenta uma síntese sem deixar claro de onde veio a informação;
* duas fontes são apresentadas como concordantes sem que a concordância tenha sido verificada;
* uma recomendação parece plausível, mas não está explicitamente sustentada pela fonte;
* uma resposta mistura informações das fontes com conhecimento externo;
* uma conclusão interpretativa é apresentada como se fosse uma afirmação documental.

O registro dessas situações é importante porque mostra que o projeto não consistiu simplesmente em perguntar algo à IA e copiar a resposta.

O processo exigiu investigação, comparação, verificação e revisão.

---

# 3. Cicatriz 1 — A pergunta ampla demais

## Problema

Uma das primeiras dificuldades identificadas foi perceber que uma pergunta ampla pode produzir uma resposta igualmente ampla.

Quando o objetivo é investigar um aspecto específico da técnica de arco, uma pergunta genérica pode fazer com que diferentes conceitos sejam reunidos sem que fique claro:

* qual fonte sustenta cada informação;
* se determinada afirmação está realmente presente nas fontes;
* se a resposta representa uma síntese;
* ou se a IA completou a resposta utilizando conhecimento externo.

Esse tipo de resposta pode parecer satisfatório à primeira leitura, mas apresenta um problema de rastreabilidade.

## Ajuste

A estratégia adotada foi restringir progressivamente os prompts.

Em vez de solicitar simplesmente uma explicação geral, passou-se a indicar:

* o assunto específico;
* as fontes que deveriam ser consideradas;
* o objetivo da investigação;
* o tipo de informação procurada;
* a necessidade de indicar a origem das afirmações.

## Aprendizado

Uma pergunta mais específica não serve apenas para obter uma resposta mais curta.

Ela aumenta o controle sobre **o que está sendo investigado**.

---

# 4. Cicatriz 2 — A resposta parecia correta, mas a fonte precisava ser verificada

## Problema

Uma resposta da IA pode apresentar uma explicação coerente e tecnicamente plausível sem que isso seja suficiente para afirmar que determinado autor realmente disse aquilo.

Esse foi um ponto metodológico importante do projeto.

A pergunta deixou de ser apenas:

> "A resposta parece correta?"

e passou a ser:

> "Onde essa informação está sustentada nas fontes?"

Essa mudança é fundamental para um projeto baseado em curadoria documental.

## Ajuste

Foram elaborados prompts solicitando explicitamente a identificação das evidências utilizadas.

A investigação passou a exigir que as afirmações fossem relacionadas às respectivas fontes, evitando que uma síntese da IA fosse automaticamente tratada como conteúdo original do autor.

## Aprendizado

**Plausibilidade não é o mesmo que evidência.**

Uma resposta pode ser coerente e ainda assim precisar de verificação documental.

---

# 5. Cicatriz 3 — Duas fontes pareciam concordar

## Problema

Durante a comparação entre fontes, surgiu outro risco:

> considerar que duas fontes concordam simplesmente porque a IA apresentou os dois conteúdos como semelhantes.

Uma concordância precisa ser demonstrada.

Não basta que duas ideias pareçam próximas.

É necessário verificar se as fontes realmente sustentam a mesma afirmação.

## Ajuste

Foi criado um prompt específico para revisar as concordâncias identificadas anteriormente:

> "Revise a resposta anterior e verifique, especificamente, as afirmações apresentadas como concordâncias entre as duas fontes."

A solicitação também exigia que fossem indicadas as passagens ou evidências presentes em cada fonte.

Quando uma afirmação não estivesse claramente sustentada pelas duas fontes, a orientação era:

> sinalizá-la explicitamente em vez de inferir ou completar a informação.

## Aprendizado

A comparação entre fontes precisa ser uma **verificação**, e não apenas uma aproximação temática.

---

# 6. Cicatriz 4 — A IA pode completar lacunas

## Problema

Outro risco identificado foi a tendência de uma resposta aparentemente completa preencher lacunas que não estavam efetivamente cobertas pelas fontes.

Isso pode ocorrer porque a IA consegue produzir uma explicação coerente utilizando conhecimento relacionado ao tema.

Para um projeto de pesquisa baseado em fontes selecionadas, entretanto, isso pode comprometer a rastreabilidade.

## Ajuste

Quando o objetivo era investigar exclusivamente as fontes selecionadas, os prompts passaram a conter restrições explícitas, como:

* utilizar exclusivamente as fontes selecionadas;
* indicar a fonte de cada recomendação;
* não fazer inferências além do que estivesse respaldado;
* não completar lacunas com conhecimento externo.

## Aprendizado

Quanto mais importante for a fidelidade às fontes, mais explícita precisa ser a delimitação do prompt.

---

# 7. Cicatriz 5 — Recomendações não são todas iguais

## Problema

Durante a pesquisa, uma recomendação pode aparecer em uma resposta de IA sem que esteja claro qual é o seu nível de sustentação documental.

Isso cria uma dificuldade:

**A fonte realmente recomenda isso ou a IA chegou a essa conclusão a partir da fonte?**

Essa diferença é metodologicamente importante.

## Ajuste

Foi criada uma etapa específica de classificação das recomendações.

Cada recomendação passou a ser analisada segundo três possibilidades:

### A — Explicitamente recomendada

A fonte apresenta claramente a prática, ajuste ou estratégia.

### B — Síntese ou interpretação

A conclusão resulta da combinação ou interpretação de informações presentes na fonte.

### C — Não suficientemente sustentada

A informação não pode ser atribuída à fonte com segurança.

Essa classificação passou a funcionar como uma espécie de filtro antes da utilização das informações no miniguia.

## Aprendizado

Não basta saber **o que** uma fonte diz.

Também é necessário saber **com que grau de segurança podemos atribuir determinada conclusão a ela**.

---

# 8. Cicatriz 6 — A necessidade de separar evidência e interpretação

Uma das principais dificuldades metodológicas do projeto foi perceber que diferentes tipos de afirmação podem aparecer misturados em uma mesma resposta.

Para evitar isso, foi adotada uma classificação em três níveis.

## A — Evidência direta

Informação apresentada explicitamente por uma fonte.

## B — Síntese entre fontes

Conclusão construída a partir da combinação de informações apresentadas por diferentes fontes.

## C — Inferência ou interpretação

Conclusão que não aparece explicitamente nas fontes e resulta de interpretação.

Essa classificação passou a orientar a leitura das respostas produzidas pela IA.

## Aprendizado

Uma síntese pode ser válida sem ser uma citação de uma fonte.

Por isso, o projeto procura deixar clara a diferença entre:

**o que a fonte afirma**

e

**o que o projeto conclui a partir das fontes**.

---

# 9. Cicatriz 7 — Uma fonte não precisa explicar tudo

## Problema

Outra dificuldade foi a expectativa de que uma única fonte pudesse responder integralmente às questões do projeto.

O tema envolve diferentes dimensões:

**física → corpo → movimento → técnica → som**

Uma fonte especializada em física da interação arco-corda não necessariamente apresenta uma explicação detalhada sobre biomecânica.

Da mesma forma, uma fonte voltada à organização corporal não necessariamente explica todos os aspectos físicos da interação entre arco e corda.

## Ajuste

Em vez de procurar uma fonte capaz de responder a todas as perguntas, o projeto passou a utilizar as fontes de maneira complementar.

### Georg Mertens

Contribui principalmente para a compreensão da física e da interação entre arco e corda.

### Maria Inês Vaz Torres

Contribui principalmente para aspectos técnicos, corporais, pedagógicos e biomecânicos.

### Catarina Putzner

Contribui principalmente para a investigação das tensões relacionadas ao polegar e sua relação com a técnica de arco.

## Aprendizado

A complementaridade das fontes é mais importante do que tentar transformar uma única fonte em autoridade absoluta sobre todo o tema.

---

# 10. Cicatriz 8 — A síntese final precisa preservar as diferenças entre as fontes

## Problema

Ao reunir informações de diferentes fontes, existe o risco de produzir um texto uniforme demais.

Quando isso acontece, as contribuições individuais dos autores podem desaparecer.

O resultado parece uma única teoria, mesmo quando as fontes possuem objetivos e perspectivas diferentes.

## Ajuste

A etapa de integração das três fontes foi realizada somente depois das etapas de investigação, comparação, verificação e classificação.

O objetivo foi identificar:

* a contribuição específica de cada fonte;
* os conceitos que podem ser relacionados;
* as complementaridades;
* os limites da síntese.

## Aprendizado

Integrar fontes não significa apagar suas diferenças.

A síntese deve preservar a origem e o papel de cada contribuição.

---

# 11. Cicatriz 9 — Refinar o prompt é parte da pesquisa

Um dos principais aprendizados do projeto foi perceber que a reformulação de um prompt não representa necessariamente uma falha.

Ela faz parte do próprio processo de investigação.

O primeiro prompt pode revelar que:

* a pergunta está ampla;
* a resposta não está suficientemente documentada;
* a fonte não foi delimitada;
* a solicitação permite interpretações demais;
* o formato da resposta não atende ao objetivo.

Nesse caso, o prompt seguinte funciona como uma ferramenta de refinamento.

O processo pode ser representado como:

```text
PERGUNTA
   ↓
RESPOSTA
   ↓
ANÁLISE DA RESPOSTA
   ↓
IDENTIFICAÇÃO DO PROBLEMA
   ↓
REFORMULAÇÃO DO PROMPT
   ↓
NOVA RESPOSTA
   ↓
VERIFICAÇÃO
```

Assim, o prompt não é apenas uma pergunta.

Ele funciona como parte da metodologia de pesquisa.

---

# 12. Troubleshooting metodológico

As principais dificuldades encontradas podem ser resumidas da seguinte maneira.

| Problema                          | Risco                                    | Solução adotada              |
| --------------------------------- | ---------------------------------------- | ---------------------------- |
| Pergunta ampla                    | Resposta genérica                        | Restringir o escopo          |
| Fonte não identificada            | Perda de rastreabilidade                 | Solicitar atribuição         |
| Concordância presumida            | Falsa convergência                       | Verificar cada fonte         |
| Lacunas preenchidas pela IA       | Introdução de conhecimento externo       | Delimitar as fontes          |
| Recomendações sem classificação   | Confusão entre evidência e interpretação | Classificar A/B/C            |
| Síntese apresentada como citação  | Atribuição incorreta                     | Separar síntese de evidência |
| Uma fonte tratada como suficiente | Simplificação excessiva                  | Cruzar perspectivas          |
| Prompt insuficiente               | Resposta inadequada                      | Refinar iterativamente       |

---

# 13. O que foi aprendido sobre o uso da IA

O projeto mostrou que a utilização da Inteligência Artificial para pesquisa não deve ser reduzida à obtenção de respostas prontas.

A IA foi mais útil quando utilizada para:

1. formular perguntas;
2. explorar conceitos;
3. localizar informações;
4. comparar fontes;
5. verificar afirmações;
6. identificar relações;
7. organizar informações;
8. produzir sínteses;
9. revisar possíveis problemas.

Entretanto, a avaliação da resposta permaneceu como responsabilidade do pesquisador.

A IA pode auxiliar na investigação, mas não elimina a necessidade de análise crítica.

---

# 14. O ciclo de aprendizagem construído

As experiências registradas nas cicatrizes permitiram estruturar um ciclo de aprendizagem:

```text
PERGUNTAR
    ↓
INVESTIGAR
    ↓
COMPARAR
    ↓
QUESTIONAR
    ↓
VERIFICAR
    ↓
SINTETIZAR
    ↓
APLICAR
    ↓
REVISAR
```

Esse ciclo é coerente com o objetivo geral do projeto: utilizar a Inteligência Artificial como ferramenta de aprendizagem ativa.

O estudante não recebe simplesmente uma resposta final.

Ele participa do processo de investigação, avaliação e construção do conhecimento.

---

# 15. O que não funcionou — e por quê

As dificuldades encontradas também permitem identificar estratégias que devem ser evitadas.

### 15.1. Perguntar sem delimitar

Perguntas excessivamente amplas podem produzir respostas difíceis de rastrear.

### 15.2. Aceitar a primeira resposta

Uma resposta coerente não é automaticamente uma resposta verificada.

### 15.3. Considerar uma síntese como fala do autor

A IA pode combinar informações de maneiras que não aparecem dessa forma em nenhuma fonte individual.

### 15.4. Presumir concordância

Duas fontes podem abordar o mesmo assunto sem apresentar exatamente a mesma explicação.

### 15.5. Completar lacunas automaticamente

Quando uma informação não está suficientemente sustentada, o correto é registrar a limitação, e não preencher a lacuna por inferência.

### 15.6. Utilizar conhecimento externo quando a pergunta exige exclusividade documental

Isso pode tornar impossível distinguir o que veio das fontes selecionadas e o que foi acrescentado pela IA.

---

# 16. O que funcionou melhor

A estratégia que apresentou melhores resultados foi a investigação progressiva.

O processo adotado foi:

**pergunta → comparação → verificação → extração → classificação → síntese**

Cada etapa respondeu a um problema identificado na etapa anterior.

### Pergunta

Define o objeto da investigação.

### Comparação

Coloca diferentes fontes em relação.

### Verificação

Testa se as conclusões possuem sustentação.

### Extração

Seleciona informações relevantes para o objetivo do projeto.

### Classificação

Diferencia evidência, síntese e informação insuficientemente sustentada.

### Síntese

Integra os resultados preservando a origem das informações.

---

# 17. Por que registrar as cicatrizes?

Registrar somente o resultado final esconderia uma parte importante do projeto.

As dificuldades mostram:

* como as perguntas foram aprimoradas;
* como os erros foram identificados;
* como a confiabilidade das respostas foi avaliada;
* como as fontes foram comparadas;
* como as limitações da IA foram consideradas;
* como o método foi construído.

Portanto, as cicatrizes não representam apenas problemas.

Elas representam **aprendizados metodológicos**.

---

# 18. Síntese final

O principal aprendizado desta etapa foi que a qualidade de uma pesquisa apoiada por Inteligência Artificial depende não apenas da ferramenta utilizada, mas da maneira como ela é questionada e, principalmente, de como suas respostas são avaliadas.

Durante o projeto, tornou-se necessário passar de perguntas gerais para perguntas controladas, de respostas para verificações e de sínteses automáticas para análises críticas.

O processo pode ser resumido em uma ideia:

> **Não basta perguntar à IA. É necessário investigar a resposta.**

As cicatrizes registram justamente essa transformação.

O projeto começou utilizando a IA como ferramenta para obter informações e avançou para uma utilização mais crítica, na qual a IA passou a participar de um processo estruturado de:

**investigação → comparação → verificação → síntese → revisão.**

Esse processo tornou o resultado final mais rastreável e permitiu distinguir aquilo que está diretamente sustentado pelas fontes daquilo que foi construído como síntese ou interpretação durante o desenvolvimento do projeto.

---

# 19. Relação com os prompts utilizados

As cicatrizes documentadas nesta seção estão diretamente relacionadas à evolução dos prompts utilizados no projeto.

A sequência registrada em `prompts-utilizados.md` é:

**1. Investigação sobre tensão no polegar**
↓
**2. Comparação entre fontes**
↓
**3. Verificação das concordâncias**
↓
**4. Identificação de recomendações**
↓
**5. Classificação das recomendações**
↓
**6. Integração das três fontes**

Essa progressão demonstra que os prompts foram sendo refinados para aumentar o controle sobre a qualidade e a rastreabilidade das informações.

---

# 20. Conclusão

As cicatrizes e os problemas encontrados durante o projeto não são elementos secundários.

Eles fazem parte da própria demonstração de aprendizagem ativa.

O GitHub registra não apenas o miniguia final, mas também o caminho percorrido para construí-lo.

A principal conclusão metodológica é:

**uma boa resposta da IA não encerra a investigação; ela inicia a etapa de verificação.**

---

[← Voltar para os prompts utilizados](./prompts-utilizados.md)

[→ Ir para os prompts reutilizáveis](./prompts-reutilizaveis.md)

[↑ Voltar ao README](../README.md)

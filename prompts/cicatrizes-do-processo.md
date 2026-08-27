# Cicatrizes e Troubleshooting — Uso do NotebookLM

Esta seção registra dificuldades encontradas durante o processo de pesquisa com IA, as alterações realizadas nos prompts e os critérios utilizados para melhorar a qualidade das respostas.

A intenção é documentar não apenas o resultado final, mas também o processo de refinamento das perguntas.

## 1. Primeiro problema: respostas muito amplas

### Situação

O primeiro conjunto de perguntas buscava compreender a técnica de arco de maneira geral. As respostas apresentavam diversos conceitos relacionados ao violoncelo, mas nem sempre deixavam suficientemente claro quais informações estavam diretamente fundamentadas nas fontes selecionadas.

### Ajuste realizado

O prompt foi refinado para solicitar que a resposta utilizasse prioritariamente as fontes carregadas no NotebookLM e identificasse a origem das informações.

### Aprendizado

Uma pergunta ampla pode produzir uma resposta informativa, mas não necessariamente adequada para um trabalho que exige rastreabilidade das informações. Por este motivo, tornou-se necessário restringir o escopo e solicitar referências explícitas.

---

## 2. Segundo problema: separar informação da fonte e interpretação

### Situação

Ao comparar informações sobre física, biomecânica e técnica, surgiu o risco de apresentar como consenso das fontes uma conclusão que, na realidade, era uma síntese produzida a partir da comparação entre elas.

### Ajuste realizado

Os prompts passaram a solicitar uma distinção entre:

* informação diretamente apresentada pela fonte;
* informação sustentada pela combinação de fontes;
* interpretação ou inferência produzida durante a análise.

### Aprendizado

A IA pode produzir uma síntese coerente sem deixar evidente quais partes estão literalmente fundamentadas em uma fonte específica. Solicitar explicitamente essa diferenciação melhora a confiabilidade da pesquisa.

---

## 3. Terceiro problema: necessidade de verificar afirmações

### Situação

Algumas respostas apresentavam explicações técnicas de maneira muito direta. Isso poderia levar à aceitação automática de uma afirmação sem verificar se ela estava efetivamente sustentada pelos documentos utilizados.

### Ajuste realizado

Foram elaborados prompts solicitando que as afirmações fossem classificadas conforme seu grau de sustentação nas fontes.

### Critério utilizado

A análise passou a considerar três possibilidades:

**A — Evidência direta:** a informação está explicitamente apresentada em uma fonte.

**B — Síntese entre fontes:** a conclusão resulta da combinação de informações presentes em mais de uma fonte.

**C — Inferência/interpretação:** a conclusão não está explicitamente apresentada nas fontes e deve ser tratada como interpretação.

### Aprendizado

Essa classificação ajudou a evitar que interpretações fossem apresentadas como fatos documentados.

---

## 4. Quarto problema: transformar pesquisa em material de estudo

### Situação

As respostas do NotebookLM eram úteis para investigação, mas não estavam necessariamente organizadas na forma de um material de revisão.

### Ajuste realizado

Depois da etapa de investigação, foram utilizados prompts específicos para organizar as informações em tópicos, relações entre conceitos, sínteses e aplicações práticas.

### Aprendizado

A IA foi utilizada em etapas diferentes: primeiro como ferramenta de investigação e comparação e depois como ferramenta de organização do conhecimento.

---

## 5. O que foi aprendido sobre elaboração de prompts

O principal aprendizado do processo foi que a qualidade da resposta depende não apenas da pergunta, mas também das restrições fornecidas.

Prompts mais eficientes passaram a especificar:

* quais fontes deveriam ser utilizadas;
* qual era o objetivo da pergunta;
* qual nível de detalhe era desejado;
* como as evidências deveriam ser apresentadas;
* quando uma informação deveria ser tratada como inferência;
* qual estrutura deveria ser utilizada na resposta.

Assim, o processo evoluiu de perguntas gerais para perguntas mais controladas, verificáveis e orientadas ao objetivo do estudo.

## Síntese do troubleshooting

**Prompt amplo → identificação do problema → restrição do escopo → solicitação de evidências → comparação das fontes → síntese final.**

Esse processo foi incorporado ao método de construção do Caderno Temático.

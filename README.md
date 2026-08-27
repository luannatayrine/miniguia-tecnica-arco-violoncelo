#  Miniguia Técnico do Arco do Violoncelo

> Um guia introdutório que relaciona física, biomecânica e técnica de arco para compreender como o movimento do violoncelista influencia a interação entre arco e corda e, consequentemente, a produção sonora.

## Sobre o projeto

O arco é um dos principais meios de produção sonora do violoncelo. Seu funcionamento envolve uma interação entre instrumento, arco, corda e corpo do instrumentista.

Este projeto busca explicar essa relação de maneira integrada, conectando conceitos físicos aos aspectos técnicos e biomecânicos envolvidos na execução.

O miniguia foi desenvolvido a partir de três fontes principais:

- Georg Mertens — *Re-Thinking Bow Technique: An Objective Analysis of Bow Technique — An Insight about the Behaviour of Bow and String*;
- Maria Inês Vaz Torres — *Introdução à técnica de arco no violoncelo. Estratégias pedagógicas para uma prática saudável*;
- Catarina Putzner — *Os impactos das tensões do polegar na técnica de arco*.

## Objetivo

Construir uma explicação acessível sobre a técnica de arco, relacionando:

**física → corpo → movimento → técnica → som**

O projeto procura responder não apenas **"como fazer?"**, mas também:

> **"O que está acontecendo fisicamente e corporalmente quando fazemos isso?"**

## Metodologia

O projeto foi desenvolvido utilizando a Inteligência Artificial como ferramenta de aprendizagem ativa por meio do NotebookLM.

O processo foi organizado em etapas:

1. **Definição do tema:** escolha dos fundamentos da técnica de arco no violoncelo como objeto de estudo.
2. **Curadoria:** seleção de três fontes abertas relacionadas à física da interação arco-corda, biomecânica, técnica e tensões corporais.
3. **Organização das fontes:** preparação e carregamento dos materiais selecionados no NotebookLM.
4. **Investigação:** elaboração de perguntas estratégicas sobre os conceitos estudados.
5. **Comparação:** análise das informações apresentadas pelas diferentes fontes.
6. **Verificação:** solicitação de referências e distinção entre evidências diretas, sínteses entre fontes e interpretações.
7. **Refinamento:** reformulação dos prompts quando as respostas eram amplas, pouco específicas ou insuficientemente rastreáveis.
8. **Síntese:** organização dos resultados em um miniguia de estudo.
9. **Revisão:** construção de glossário e prompts reutilizáveis para futuras sessões de estudo.

Dessa forma, a IA não foi utilizada apenas para gerar texto, mas como ferramenta para pesquisar, comparar, questionar, verificar e organizar o conhecimento.

## Estrutura

###  Fontes

A pasta `fontes/` contém a organização e a análise das referências utilizadas.

- [Física do arco](fontes/01-fisica-do-arco.md)
- [Biomecânica do arco](fontes/02-biomecanica-do-arco.md)
- [Técnica do arco](fontes/03-tecnica-do-arco.md)
- [Integração entre física e biomecânica](fontes/04-integracao-fisica-biomecanica.md)


###  Guia

A pasta `guia/` contém o conteúdo didático desenvolvido a partir da pesquisa.

- [Introdução](guia/01-introducao.md)
- [Como o arco produz o som](guia/02-como-o-arco-produz-o-som.md)
- [Parâmetros do arco](guia/03-parametros-do-arco.md)
- [Corpo e movimento](guia/04-corpo-e-movimento.md)
- [Polegar e tensão](guia/05-polegar-e-tensao.md)

###  Prompts

A pasta `prompts/` registra os prompts utilizados como parte do processo de pesquisa e desenvolvimento do projeto.

## Modelo conceitual

```text
CORPO
  ↓
MOVIMENTO
  ↓
ARCO
  ↓
INTERAÇÃO ARCO-CORDA
  ↓
VIBRAÇÃO
  ↓
SOM

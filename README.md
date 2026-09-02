# Desafio-Dio-Notebook-Lm
# Como ensinar uma IA a responder melhor?

## Experimentos de Engenharia de Prompts com NotebookLM

![NotebookLM](https://img.shields.io/badge/Ferramenta-NotebookLM-blue)
![DIO](https://img.shields.io/badge/Projeto-DIO-orange)
![Prompt Engineering](https://img.shields.io/badge/Tema-Prompt%20Engineering-purple)

---

## Sobre o projeto

Este projeto foi desenvolvido como parte de um desafio da **DIO**, utilizando o NotebookLM como ferramenta de aprendizagem ativa.

A proposta foi investigar, de forma prática, **como diferentes estratégias de Engenharia de Prompts podem influenciar a qualidade das respostas de uma Inteligência Artificial**.

Em vez de apenas estudar conceitos de Prompt Engineering, foram realizados experimentos diretamente no NotebookLM, modificando progressivamente a forma de elaborar perguntas e instruções.

A pergunta central do projeto foi:

> **Como ensinar uma IA a responder melhor?**

Durante os experimentos, foram observados aspectos como clareza, profundidade, relevância, estrutura, utilização das fontes e aderência às instruções.

---

#  Objetivos

### Objetivo geral

Investigar como diferentes estratégias de Engenharia de Prompts podem alterar a qualidade, a estrutura e a confiabilidade das respostas geradas por uma IA.

### Objetivos específicos

* Comparar prompts simples e prompts estruturados;
* Observar o efeito da inclusão de contexto;
* Testar critérios e restrições;
* Analisar divergências entre fontes;
* Avaliar a capacidade da IA de revisar suas próprias respostas;
* Testar Few-shot Prompting;
* Identificar falhas na interpretação de instruções;
* Desenvolver um prompt final combinando as estratégias que apresentaram melhores resultados;
* Registrar erros, descobertas e aprendizados durante o processo.

---

# Metodologia

Foi criado um notebook no **NotebookLM**, reunindo mais de 40 fontes relacionadas a Inteligência Artificial, Engenharia de Prompts, RAG e utilização de modelos de linguagem.

As fontes utilizadas incluíram vídeos, artigos e documentos.

A investigação foi realizada de forma progressiva, modificando a maneira de elaborar os prompts a cada experimento.

Os resultados foram analisados considerando seis critérios:

| Critério                    | O que foi observado                                          |
| --------------------------- | ------------------------------------------------------------ |
| **Clareza**                 | Se a resposta era compreensível e objetiva                   |
| **Profundidade**            | Quanto o assunto foi explorado                               |
| **Relevância**              | Se as informações eram úteis para a tarefa                   |
| **Estrutura**               | Se a resposta estava organizada adequadamente                |
| **Fontes**                  | Se as informações estavam relacionadas às fontes disponíveis |
| **Aderência às instruções** | Se a IA realmente realizou a tarefa solicitada               |

Além das avaliações, foram registradas as principais falhas encontradas durante os testes.

Essas falhas foram chamadas de **“cicatrizes”**, representando problemas que contribuíram para compreender melhor as limitações da interação com uma IA.

---

# Experimentos

## Experimento 01 — Prompt simples

### Técnica

**Prompt direto / Zero-shot**

### Prompt

> O que é engenharia de prompts?

### Resultado

O NotebookLM produziu uma resposta bastante completa, abordando:

* conceito de prompt;
* Engenharia de Prompts;
* contexto;
* persona;
* objetivos e limitações;
* formato de saída;
* Zero-shot;
* Few-shot;
* Chain-of-Thought;
* Markdown/XML;
* evolução da área.

### Avaliação

| Critério                | Nota |
| ----------------------- | ---: |
| Clareza                 |  5/5 |
| Profundidade            |  5/5 |
| Relevância              |  5/5 |
| Estrutura               |  4/5 |
| Fontes                  |  4/5 |
| Aderência às instruções |  5/5 |

### Aprendizado

Uma pergunta simples pode gerar uma resposta bastante completa quando existem fontes relevantes disponíveis.

Porém, uma pergunta aberta oferece maior liberdade para a IA decidir o que considera relevante.

### Cicatriz

> **Uma resposta completa não significa necessariamente uma resposta perfeitamente direcionada ao objetivo do usuário.**

---

## Experimento 02 — Contexto + objetivo

### Técnica

**Inclusão de contexto e objetivo**

O segundo experimento passou a fornecer mais direcionamento para a IA.

O NotebookLM apresentou conceitos como:

* contexto;
* instrução;
* persona;
* formato;
* Zero-shot;
* Few-shot;
* Chain-of-Thought;
* Tree-of-Thoughts;
* ReAct;
* Self-Refine;
* Chain-of-Verification.

### Avaliação

| Critério                | Nota |
| ----------------------- | ---: |
| Clareza                 |  5/5 |
| Profundidade            |  5/5 |
| Relevância              |  4/5 |
| Estrutura               |  4/5 |
| Fontes                  |  4/5 |
| Aderência às instruções |  5/5 |

### Aprendizado

Adicionar contexto e definir melhor o objetivo ajuda a direcionar o conteúdo.

Por outro lado, o aumento de instruções também pode tornar a resposta mais extensa.

---

## Experimento 03 — Critérios + restrições

### Técnica

**Definição de critérios**

Foram adicionados critérios mais específicos para orientar a resposta.

O NotebookLM apresentou cinco elementos relacionados à construção de prompts:

1. Instrução;
2. Contexto;
3. Persona;
4. Exemplos;
5. Formato.

Também foram discutidas técnicas como:

* Zero-shot;
* Few-shot;
* Chain-of-Thought;
* Role Prompting;
* Rephrase-and-Respond.

### Avaliação

| Critério                | Nota |
| ----------------------- | ---: |
| Clareza                 |  5/5 |
| Profundidade            |  4/5 |
| Relevância              |  4/5 |
| Estrutura               |  5/5 |
| Fontes                  |  4/5 |
| Aderência às instruções |  5/5 |

### Aprendizado

Critérios adicionais aumentaram o controle sobre a organização da resposta.

Entretanto:

> **Adicionar instruções não garante automaticamente uma resposta mais objetiva ou significativamente melhor.**

---

## Experimento 04 — Análise crítica das fontes

### Técnica

**Comparação de fontes e identificação de divergências**

O objetivo passou a ser identificar diferenças entre as fontes, possíveis contradições e diferentes interpretações sobre Engenharia de Prompts.

O NotebookLM encontrou divergências relacionadas a:

* Engenharia de Prompts como ciência ou prática de design;
* utilização de personas;
* importância da escolha das palavras;
* futuro da profissão de Prompt Engineer;
* técnicas simples versus técnicas complexas.

### Resultado

A IA conseguiu reunir diferentes perspectivas e organizar os principais pontos de divergência.

Porém, a análise também apresentou algumas afirmações fortes que posteriormente precisaram ser verificadas.

### Aprendizado

A IA consegue combinar informações de diferentes fontes, mas isso não significa que todas as associações ou interpretações estejam necessariamente corretas.

###  Cicatriz

> **A IA pode combinar corretamente informações de diferentes fontes e ainda assim atribuir ou interpretar incorretamente determinados conceitos.**

---

## Experimento 05 — Estruturação da análise

### Técnica

**Instruções estruturadas + análise de divergências**

A resposta foi organizada em quatro partes:

1. Consensos;
2. Divergências;
3. Análise das divergências;
4. Conclusões baseadas nas evidências.

Também foi solicitado que a IA:

* identificasse as fontes;
* utilizasse títulos claros;
* evitasse tabelas;
* não apresentasse conclusões como fatos sem evidência suficiente;
* deixasse incertezas explícitas.

### Avaliação

| Critério                | Nota |
| ----------------------- | ---: |
| Clareza                 |  5/5 |
| Profundidade            |  4/5 |
| Relevância              |  4/5 |
| Estrutura               |  5/5 |
| Fontes                  |  5/5 |
| Aderência às instruções |  5/5 |

### Aprendizado

A estrutura explícita aumentou o controle sobre o formato e a organização da resposta.

Porém:

> **Mais instruções podem aumentar o controle e a profundidade sem necessariamente aumentar a objetividade.**

---

## Experimento 06 — Autoauditoria

### Técnica

**Self-Refine / revisão crítica**

A IA recebeu a tarefa de revisar criticamente sua própria resposta anterior.

Ela deveria procurar:

1. afirmações mais fortes que as evidências;
2. informações que precisavam de fontes;
3. repetições;
4. pontos importantes omitidos;
5. possíveis interpretações ou generalizações incorretas.

Depois, deveria produzir uma versão corrigida.

### Resultado

O NotebookLM identificou problemas concretos, incluindo:

* associação incorreta de uma afirmação a uma fonte;
* confusão entre o estudo LIMA e Engenharia de Prompts;
* atribuições que precisavam ser corrigidas;
* extrapolações sobre APIs e economia de computação;
* pontos relevantes que haviam sido omitidos.

### Aprendizado

A autoauditoria mostrou que uma IA pode ser utilizada para **questionar e revisar uma resposta anterior**.

Entretanto, a própria revisão continuou apresentando afirmações que exigiam análise crítica.

###  Cicatriz

> **A autoauditoria pode ajudar a encontrar erros, mas não substitui a verificação humana das fontes.**

---

## Experimento 07 — Few-shot Prompting

### Técnica

**Few-shot Prompting**

Foi apresentado à IA um exemplo de como uma afirmação deveria ser analisada.

A estrutura apresentada era:

* Afirmação;
* Avaliação;
* Justificativa;
* Nível de confiança;
* Conclusão.

Em seguida, foram fornecidas três afirmações específicas para análise.

### Resultado

O NotebookLM reproduziu muito bem a estrutura apresentada no exemplo.

Porém, ocorreu uma falha importante:

**as três afirmações fornecidas não foram analisadas.**

Em vez disso, o modelo afirmou que não havia recebido uma lista específica e escolheu outras afirmações para analisar.

### Avaliação

| Critério                | Nota |
| ----------------------- | ---: |
| Clareza                 |  5/5 |
| Profundidade            |  4/5 |
| Relevância              |  3/5 |
| Estrutura               |  5/5 |
| Fontes                  |  4/5 |
| Aderência às instruções |  2/5 |

### Aprendizado

O Few-shot funcionou muito bem para ensinar **como estruturar uma resposta**, mas não garantiu que a IA executasse corretamente **qual tarefa deveria realizar**.

###  Cicatriz

> **Uma resposta pode estar muito bem estruturada e ainda assim estar errada porque não realizou a tarefa solicitada.**

Esse experimento demonstrou uma diferença importante:

> **Qualidade textual ≠ aderência à tarefa.**

---

## Experimento 08 — Prompt otimizado

### Objetivo

Combinar as estratégias que apresentaram melhores resultados nos experimentos anteriores sem simplesmente criar um prompt excessivamente longo.

Foram utilizados:

* objetivo claro;
* contexto;
* utilização das fontes;
* tarefa dividida em etapas;
* formato de saída;
* diferenciação entre evidência e interpretação;
* tratamento de divergências;
* verificação final de aderência.

### Tarefa

Analisar a afirmação:

> **“Prompts mais longos produzem respostas melhores.”**

### Resultado

O NotebookLM concluiu que a afirmação **depende do contexto**.

A resposta diferenciou o tamanho do prompt da qualidade das informações presentes nele e apresentou situações em que um prompt mais detalhado pode ser útil e situações em que informações redundantes podem prejudicar o resultado.

### Avaliação

| Critério                | Nota |
| ----------------------- | ---: |
| Clareza                 |  5/5 |
| Profundidade            |  5/5 |
| Relevância              |  5/5 |
| Estrutura               |  5/5 |
| Fontes                  |  4/5 |
| Aderência às instruções |  5/5 |

### Aprendizado

O prompt final conseguiu combinar os principais elementos que apresentaram bons resultados durante os experimentos.

Mesmo assim, algumas afirmações apresentadas pelo NotebookLM eram bastante específicas e fortes, demonstrando novamente que uma resposta bem estruturada e baseada em fontes ainda precisa ser verificada criticamente.

---

# Comparação dos experimentos

| Exp. | Técnica                  | Clareza | Prof. | Relev. | Estrut. | Fontes | Aderência |
| ---- | ------------------------ | ------: | ----: | -----: | ------: | -----: | --------: |
| 01   | Prompt simples           |       5 |     5 |      5 |       4 |      4 |         5 |
| 02   | Contexto + objetivo      |       5 |     5 |      4 |       4 |      4 |         5 |
| 03   | Critérios + restrições   |       5 |     4 |      4 |       5 |      4 |         5 |
| 04   | Análise crítica          |       — |     — |      — |       — |      — |         — |
| 05   | Estrutura + divergências |       5 |     4 |      4 |       5 |      5 |         5 |
| 06   | Autoauditoria            |       — |     — |      — |       — |      — |         — |
| 07   | Few-shot                 |       5 |     4 |      3 |       5 |      4 |         2 |
| 08   | Prompt otimizado         |       5 |     5 |      5 |       5 |      4 |         5 |

> **Observação:** os experimentos 04 e 06 foram avaliados principalmente de forma qualitativa durante a análise dos resultados, portanto não foram atribuídas notas retrospectivas.

---

# Cicatrizes do projeto

As falhas encontradas durante os experimentos foram tão importantes quanto os resultados positivos.

### Cicatriz 01 — Resposta completa não significa resposta perfeita

Uma pergunta simples pode produzir uma resposta rica, mas a IA possui liberdade para decidir o que considera relevante.

### Cicatriz 02 — Mais instruções não significam necessariamente melhor resposta

O aumento da quantidade de instruções pode melhorar o controle, mas também pode tornar a resposta mais extensa e menos objetiva.

### Cicatriz 03 — Estrutura aumenta o controle

Definir previamente como a resposta deve ser organizada tornou os resultados mais previsíveis.

### Cicatriz 04 — Atribuição incorreta de informações

Durante a autoauditoria, foram encontradas associações incorretas entre informações, fontes e conceitos.

### Cicatriz 05 — Autoauditoria não substitui verificação

A IA conseguiu identificar erros, mas a própria revisão ainda apresentou afirmações que exigiam análise crítica.

### Cicatriz 06 — Few-shot não garante aderência

Um exemplo pode ensinar muito bem o formato de uma resposta sem garantir que a IA execute exatamente a tarefa solicitada.

---

# Principais descobertas

## 1. Mais texto não significa necessariamente melhor resultado

O comprimento do prompt não deve ser utilizado isoladamente como indicador de qualidade.

O que importa é a presença de **informações relevantes, contexto adequado e instruções claras**.

## 2. Estrutura ajuda a controlar a resposta

Definir etapas, critérios e formato tornou as respostas mais previsíveis e organizadas.

## 3. Contexto direciona a IA

Fornecer informações relevantes ajuda a reduzir ambiguidades e direcionar a tarefa.

## 4. Fontes não eliminam a necessidade de verificação

Mesmo utilizando um sistema baseado em fontes, é necessário conferir se a interpretação e as atribuições realizadas pela IA estão corretas.

## 5. Few-shot possui vantagens e limitações

Exemplos ajudam a demonstrar o formato desejado, mas não garantem aderência completa à instrução.

## 6. Uma resposta bem escrita pode estar errada

Esse foi um dos principais aprendizados do projeto.

Qualidade textual, estrutura e aparência de confiança não devem ser confundidas com precisão ou cumprimento da tarefa.

---

# Mini guia de estudo

## O que é um prompt?

É uma instrução, pergunta ou conjunto de informações fornecidas a um modelo de IA para orientar sua resposta.

## O que é Engenharia de Prompts?

É a prática de elaborar e testar instruções para obter resultados mais adequados de um modelo de IA.

## Elementos importantes de um prompt

### Objetivo

Define o que a IA precisa realizar.

### Contexto

Fornece informações necessárias para compreender a tarefa.

### Restrições

Define o que deve ou não ser feito.

### Formato

Determina como a resposta deverá ser organizada.

### Exemplos

Demonstram o tipo de resultado esperado.

### Critérios

Permitem avaliar se a resposta atende ao objetivo.

---

# Glossário

| Termo                  | Definição                                                                           |
| ---------------------- | ----------------------------------------------------------------------------------- |
| **Prompt**             | Instrução ou entrada fornecida a uma IA.                                            |
| **Prompt Engineering** | Processo de criação e otimização de prompts.                                        |
| **Zero-shot**          | Solicitação feita sem fornecer exemplos da resposta desejada.                       |
| **Few-shot**           | Utilização de exemplos para orientar o comportamento da IA.                         |
| **Chain-of-Thought**   | Técnica relacionada à orientação de tarefas de raciocínio em etapas.                |
| **Role Prompting**     | Definição de um papel ou perspectiva para orientar a resposta.                      |
| **Self-Refine**        | Processo de revisão e refinamento de uma resposta.                                  |
| **RAG**                | Técnica que combina recuperação de informações com geração de respostas.            |
| **Contexto**           | Informações fornecidas para ajudar a IA a compreender a tarefa.                     |
| **Hallucination**      | Geração de informações incorretas ou não sustentadas apresentadas como verdadeiras. |

---

# Prompts reutilizáveis

## Prompt para análise crítica

```text
Analise a afirmação abaixo utilizando as fontes disponíveis.

Afirmação:
[INSIRA A AFIRMAÇÃO]

Avalie se ela é verdadeira, falsa ou depende do contexto.

Apresente:
1. Avaliação
2. Evidências das fontes
3. Possíveis limitações
4. Conclusão

Diferencie claramente o que as fontes afirmam diretamente de interpretações.
Se houver divergência entre as fontes, deixe isso explícito.
```

---

## Prompt para revisão de uma resposta

```text
Revise criticamente a resposta anterior.

Verifique:
1. Afirmações mais fortes que as evidências;
2. Informações sem suporte nas fontes;
3. Repetições ou informações desnecessárias;
4. Pontos importantes que foram omitidos;
5. Possíveis interpretações ou generalizações incorretas.

Depois, produza uma versão corrigida.

Não trate uma interpretação como fato e deixe explícitas as incertezas relevantes.
```

---

## Prompt estruturado para tarefas complexas

```text
Objetivo:
[O QUE PRECISA SER FEITO]

Contexto:
[INFORMAÇÕES IMPORTANTES]

Tarefa:
[DESCREVA EXATAMENTE O QUE A IA DEVE FAZER]

Formato:
[COMO A RESPOSTA DEVE SER ORGANIZADA]

Critérios:
- Utilize as fontes disponíveis;
- Diferencie fatos de interpretações;
- Não faça afirmações além das evidências;
- Indique divergências quando existirem;
- Seja objetivo.

Antes de finalizar, verifique se todos os itens solicitados foram respondidos.
```

---

#  Fontes utilizadas

O notebook reuniu mais de 40 fontes durante o processo de pesquisa.

Para a apresentação final do projeto, foram selecionadas quatro fontes principais:

1. **Optimizing LLM Accuracy | OpenAI API**
   → [Inserir link]

2. **Advanced Prompt Engineering Techniques: Examples & Best Practices**
   → [Inserir link]

3. **AI MVP Development: Foundation Model APIs, RAG vs Fine-Tuning, and Cost Benchmarking**
   → [Inserir link]

4. **Building Production RAG: Architecture, Chunking, Evaluation & Monitoring (2026 Guide)**
   → [Inserir link]

---

# Conclusão

Os oito experimentos demonstraram que melhorar uma resposta de IA não significa simplesmente escrever prompts cada vez maiores.

A evolução observada durante o projeto mostrou que **contexto, clareza, estrutura, critérios e verificação** possuem papel importante na obtenção de respostas mais adequadas.

Também foram observadas limitações importantes: a IA pode interpretar fontes de maneira incorreta, produzir afirmações mais fortes do que as evidências disponíveis e até ignorar partes de uma instrução mesmo quando o formato solicitado é bastante claro.

O projeto também demonstrou que diferentes técnicas apresentam vantagens diferentes.

O **Few-shot**, por exemplo, apresentou grande capacidade de orientar a estrutura de uma resposta, mas não garantiu aderência à tarefa.

Já a combinação de **objetivo, contexto, critérios, formato e verificação** apresentou o melhor equilíbrio entre os critérios avaliados no experimento final.

Por isso, a principal conclusão deste projeto é:

> **Ensinar uma IA a responder melhor não significa fornecer mais instruções, mas fornecer as instruções certas, no contexto certo e de uma forma que permita verificar o resultado.**

A Engenharia de Prompts pode ser compreendida, portanto, não apenas como uma forma de “fazer a IA obedecer”, mas como um processo de **comunicação, experimentação, avaliação e refinamento**.

---

## Projeto DIO

**Tema:** Como ensinar uma IA a responder melhor?

**Ferramenta principal:** NotebookLM

**Metodologia:** Experimentação progressiva de técnicas de Engenharia de Prompts.

**Resultado:** Investigação prática das vantagens, limitações e melhores práticas observadas durante oito experimentos.

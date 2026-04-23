## Dia 23 de Abril de 2026
###  Hyper Velocity Engineering: Velocidade, qualidade e controle como vantagem competitiva com Fabricio Soares | Microsoft
linkedin: fsoaresbr

HVE é um modelo operacional. 
Existem em três  pilares: Plataforma interna, IA com guardrails e métricas DORA.
Testes desde a primeira release.
As empresas devem automatizar o máximo possível dentro dos seus processos.
A IA não substitui o engenheiro, mas multiplica.
A IA vem ajudar com as tarefas repetitivas do engenheiro.
[Imagem com qr code para DevSquad Copilot]


Meça- relatório DORA e implementação de 4 métricas KPIs
Conecte - Mapeamento dos gargalos
Acelere - a implementação em si.

Para pesquisar:
- Backdoors
- Métrica DORA

### Agentes de IA na prática: como a BIA Tech AgentiX acelera o desenvolvimento de soluções no Bradesco | Marcel Carvalho Manfio & Bruno Pereira Soares
linkedin: bruno-pereira-soares e marcelmanfio
Percebo que a o foco do bradesco é ir para o Java 21.
A tendência no futuro, é que o desenvolvedor passe mais tempo no monitoramento e observação e menos na intervenção.

Para pesquisar:
- Bia Tech AgentiX
- Agent as a code
- Programa Tech Modernization
- Devin
- OpenRouter

### Eficiência de Tokens: o caminho para escalar LLMs | Gabriel D'Amore Marciano | TOTVS

Eficiência e Eficaz. Ser eficaz é atingir o objetivo.
Janela de Contexto: o número max de tokens que o modelo pode ver de uma vez só. como se fosse a memória da LLM. input dos usuários, raga, histórico, rag e etc.

Como reduzir o custo dos tokens
1) Prompts repetidos no contexto <br>
Uma solução é o Prompt Caching. Essa solução geralmente já vem nos providers. OpenAI não cobra, já a Anthropic cobra.

2) Tokens ocupados pelas tools <br>
A solução é a Tool Search Tool. Ele seria uma tool que busca as outras tool. Apesar se ter uma requisição a mais, aumentando um pouco a latência, vale a pena a estratégia. O aumento do uso das tools aumentaria sob demanda.

3) Entradas com JSON = +Tokens <br>
Serializador chamado TOON.
O JSON gasta mais tokens.

4) Saídas não estruturadas = +Tokens <br>
A saída é mais cara que a entrada. Geralmente, o retorno para o backend precisa ser estruturado, evitando texto adicionais e estruturas não relevantes.
A solução é usar uma structured output.

Pílulas de eficiência:
- LLMLingua (Microsoft): Pega um texto (não estruturado) e reduz sem perder a semântica. Mantém a eficácia. Pode ser ideal para busca de base de conheciment.
- Caveman: força aos coding agents que força o modelo a responder de forma extremamente concisa.
- RTK: filtra e comprime saídas de comandos antes que eles chegem ao contexto da LLM.

Para pesquisar:
- Spring AI
- Artigo da Antropic sobre Tool Search (Effective Context Engineering)
- TOON

### Agents in the Shadows: O Novo Risco da IA | Ben-Hur Ott | Snyk
O MCP pode ser local ou remoto, via API.
Quando um agente de IA faz um request e response para um MCP, ele não diferencia o que é conteúdo ou instrução.
A skill pode fazer uma referência remota também.
Ou seja, coisas podem ser executadas sem o nosso controle

Cuidado:
1) Lethal Trifecta
Ver simon willison artigo.
Acesso a conteúdo privado, habilidade para comunicação externa e exposição em conteúdo não confiável.

2) MCP Toxic FLows
Ver https://invariantlabs.ai/blog/toxic-flow-analysis.
Fluxos modificados no agente pelo hacker, com o objetivo de extrair informações.
Cuidado ao dar muitas permissões para o MCP. 

3) Toxic Skills
https://snyk.io/blog/toxicskills-malicious-ai-agent-skills-clawhub/
"confiança de contexto". ou seja, é levar o llm "na conversa", fazendo ele acreditar que tal comando faz parte do contexto.
Um código malicioso pode te atacar internamente da sua estrutura.

4) Code Generation
O código gerado ainda é muito inseguro.
Ver artigos "You still have to study".

Para pesquisar:
- http://agentskills.io/home
- Claw Hub
- MCP STDIO
- Prompt injection







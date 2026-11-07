# Catarina Rodrigues Gonçalves

**AI Builder · automações com n8n e agentes LLM · fundadora do GradMent**

Estudante de Engenharia de Computação no CEFET-MG (formatura prevista em dezembro de 2028). Construo automações e sistemas com IA a partir de um problema real e meço o resultado: cada projeto abaixo tem um número e um jeito de conferir.

## Para quem avalia em 5 minutos

| O que você procura | Onde ver | O que conferir |
| --- | --- | --- |
| Automação que economiza horas | [Horas Complementares](https://github.com/catarina051/horas-complementares-ia) · [vídeo](https://lnkd.in/p/dp4rEizz) | 21 min 49 s → menos de 2 min por certificado, em piloto na AWS |
| Orquestração de vários LLMs | [PPC → GradMent](https://github.com/catarina051/ppc-gradment-ia) | Extratora, auditora e juíza em Gemini, GPT-OSS e Groq, com fallback; juíza a 92,5% em modelo diferente |
| Automação com n8n | Os dois acima | Workflows de 35 e 42 nós, gerados por script e com Code nodes testados |
| Prompt engineering | [prompts do PPC](https://github.com/catarina051/ppc-gradment-ia/tree/main/prompts) · [prompt v2 das horas](https://github.com/catarina051/horas-complementares-ia/blob/main/prompts/classificacao/v2.md) | JSON Schema estrito, defesa contra *prompt injection*, versões com histórico |
| Dashboard funcionando | [gradment.vercel.app](https://gradment.vercel.app) · [termometro-psi.vercel.app](https://termometro-psi.vercel.app) | Dados lidos por URL dos repositórios, números conferidos contra o JSON |
| Vibe coding | [dashboard do PPC](https://github.com/catarina051/ppc-gradment-dashboard) · [app do Termômetro](https://github.com/catarina051/termometro-semestre-app) | v0 + Claude Code, prompts exatos e quem fez o quê |
| API sem backend próprio | `POST /webhook/converter-ppc` (n8n) · `/api/explicar` (Next.js) | JSON pronto para a API do GradMent, sem mudar o backend PHP |
| Análise de dados com IA | [Termômetro do Semestre](https://github.com/catarina051/termometro-semestre) | 82.690 matrículas, validação por divisão de alunos, LLM que só explica |

**Sobre as datas.** O GradMent existe desde o primeiro semestre de 2026. Os projetos de IA em volta dele foram construídos em sprints curtos em nov/2026: Horas Complementares em 5 dias, PPC → GradMent e o dashboard em 1 dia, Termômetro em 1 dia. O histórico de commits de cada repositório mostra isso, e o `DIARIO.md` dos três projetos de IA conta como foi.

## Projetos em destaque

### [Termômetro do Semestre](https://github.com/catarina051/termometro-semestre) · [site](https://termometro-psi.vercel.app)
Dados abertos da UFRN (2015 a 2019) sobre reprovação e desistência no ciclo básico. Um modelo de linguagem só explica números já calculados; ele nunca calcula.
**82.690 matrículas analisadas; 9 das 12 combinações de disciplinas que pareciam perigosas eram alunos atrasados repetindo uma delas.**
`Python` · `DuckDB` · `Gemini` · `validação por divisão de alunos`

### [PPC → GradMent](https://github.com/catarina051/ppc-gradment-ia) · [execução em GIF](https://github.com/catarina051/ppc-gradment-ia#demo)
Workflow n8n de 42 nós com três LLMs de provedores diferentes (extratora, auditora e juíza) que transforma o PPC de qualquer universidade na matriz curricular do GradMent.
**A juíza acerta 92,5% das divergências quando é um modelo diferente e 66,2% quando é o mesmo; 99 de 99 disciplinas encontradas no PPC real.**
`n8n` · `Gemini` · `OpenRouter` · `Groq` · `JSON Schema` · `prompt engineering`

### [Horas Complementares com IA](https://github.com/catarina051/horas-complementares-ia)
Do certificado ao PDF para o SIGAA, com classificação por IA e cálculo de horas rastreável, em piloto numa VM da AWS.
**Menos de 2 minutos por certificado, contra 21 min 49 s à mão; categoria correta em 5 de 5 certificados (amostra pequena, testes da autora).**
`n8n` · `Gemini` · `Docker` · `Python` · `Tesseract`

### [GradMent](https://github.com/catarina051/gradment)
Planejador de grade curricular em uso por estudantes do CEFET-MG, que avisa quando uma reprovação vai atrasar a formatura. Sou fundadora e gerente de produto, e desenvolvo o front em React e TypeScript e a integração com a API.
**72 alunos cadastrados e 40 com histórico enviado (contagem do banco de produção em 07/11/2026).**
`Next.js` · `React` · `TypeScript` · `Tailwind CSS` · `CodeIgniter 4`

## Experiência

- **Fundadora, gerente de produto e desenvolvedora no GradMent**: levei uma plataforma de planejamento acadêmico da pesquisa com usuários à produção em cinco sprints, priorizo o backlog e desenvolvo o front e a integração com a API REST.
- **Bolsista FAPEMIG no FilaZero**: entrevistei profissionais da atenção primária, modelei o fluxo de atendimento em BPMN, propus uma Clean Architecture por funcionalidade e desenvolvo o aplicativo Flutter multiplataforma com acessibilidade no design system.
- **Desenvolvedora full-stack na Zé do Lead**: implementei endpoints PHP e regras de negócio e integrações React com as APIs do Google e da Meta para consolidar métricas de redes sociais num painel.
- **Pesquisa e reconhecimento**: primeira autora de dois artigos no MOCITEC MG 2026 e quarto lugar no Hackathon Pif Paf, entre várias universidades.

## Como eu trabalho com IA

Eu decido o escopo e o método; a IA executa; outras IAs me criticam. Os três projetos de IA têm um `DIARIO.md` que separa o que foi decisão minha do que foi da IA, inclusive onde ela errou: [Termômetro do Semestre](https://github.com/catarina051/termometro-semestre/blob/main/DIARIO.md), [PPC → GradMent](https://github.com/catarina051/ppc-gradment-ia/blob/main/DIARIO.md) e [Horas Complementares](https://github.com/catarina051/horas-complementares-ia/blob/main/DIARIO.md).

## Mais projetos

- **FilaZero**: pesquisa financiada pela FAPEMIG, em Flutter, com acessibilidade (eMAG 3.1, WCAG 2.1).
- [Skillcord](https://github.com/catarina051/skillcord): protótipo de runtime local para configurar agentes de código de forma reproduzível.
- [C++ Dungeon Crawler](https://github.com/catarina051/cpp-dungeon-crawler): jogo em C++17 e SFML.

## Ferramentas

| Área | Tecnologias e práticas |
| --- | --- |
| IA e automação | n8n, Gemini, OpenRouter, Groq, engenharia de prompts, JSON Schema, avaliação contra gabarito |
| Linguagens | TypeScript, JavaScript, Python, SQL, C++, Dart, PHP |
| Front-end e mobile | React, Next.js, Flutter, Tailwind CSS |
| Back-end e dados | APIs REST, CodeIgniter 4, PostgreSQL, DuckDB, Airflow, dbt |
| Engenharia | Docker, GitHub Actions, pytest, Ruff, mypy, Clean Architecture |

Português nativo; inglês intermediário, focado em leitura e escrita técnica.

## Vamos conversar

- [LinkedIn](https://www.linkedin.com/in/catarina-rodrigues-gon%C3%A7alves-b42011297)
- [E-mail](mailto:catarina.goncalves051@gmail.com)

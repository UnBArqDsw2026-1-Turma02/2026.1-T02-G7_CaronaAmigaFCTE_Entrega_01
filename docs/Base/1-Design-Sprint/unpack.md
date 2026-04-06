# Design Spring – Entender (Unpack)

## Introdução

O **Design Sprint** é uma abordagem estruturada de trabalho em etapas, criada para reduzir incertezas e acelerar decisões sobre produtos, organizando o processo em fases bem definidas (Entender, Esboçar, Decidir, Prototipar e Testar) [[1]](#referências-bibliográficas). Em vez de começar direto na solução, o método prioriza a construção de entendimento compartilhado sobre o problema, o usuário e o contexto, para que as decisões seguintes sejam mais consistentes [[3]](#REF3).

Neste documento, o foco está na etapa **Entender (Unpack)**, que tem como função consolidar o conhecimento inicial do time e alinhar o que será considerado base do projeto antes de avançar para escolhas de solução [[2]](#REF2). Para o **CaronaAmigaFCTE**, essa etapa é especialmente importante porque o domínio do problema envolve variáveis como rotas e horários, além de fatores de confiança e segurança, que precisam estar explícitos e acordados pelo grupo desde o início.

Nesta fase, foram utilizados os artefatos de **[Brainstorming](Base/2-Artefato-Generalista/Brainstorm.md)**, **[5W2H](Base/2-Artefato-Generalista/5W2H.md)** e **[Benchmarking](Base/2-Artefato-Generalista/Benchmarking.md)** para organizar ideias iniciais, estruturar decisões e comparar referências do domínio.

## Contexto e Problema

O projeto **CaronaAmigaFCTE** tem como proposta apoiar o compartilhamento de caronas **da/para a FCTE**, considerando um cenário com deslocamentos recorrentes (aulas, atividades acadêmicas e rotinas de trabalho/estudo).

Problema observado (formulação inicial):
- Dificuldade de encontrar caronas compatíveis com horários e rotas de forma prática.
- Falta de previsibilidade (cancelamentos, atrasos, mudanças de planos).
- Questões de confiança e segurança ao combinar caronas com pessoas desconhecidas.
- Custo e tempo de deslocamento como fatores relevantes para adesão.

Premissas iniciais (ajustar conforme decisão do grupo):
- Público principal: **Estudantes**.
- Plataforma alvo: **Web/Mobile**.
- Escopo geográfico típico: **Brasília/DF-Gama|DF**.
- Restrições: não usar nome de serviço real/proprietário; proposta deve ser original (baseada apenas em referências).

## Ideia Inicial do Projeto

Data de referência: **28/03/2026** 

Ideia inicial:
- Desenvolver uma solução que permita **ofertar e buscar caronas** com origem/destino relacionados à FCTE, facilitando o pareamento entre motoristas e passageiros com base em informações essenciais (rota, horário, pontos de encontro e regras combinadas).

Compreensão inicial do grupo:
- O foco inicial estava em viabilizar o encontro entre pessoas e o registro das combinações de carona.
- Pontos críticos já percebidos desde o início: confiança entre usuários, clareza das informações e redução de “ruído” na comunicação (o combinado precisa ficar explícito).

## Atividades Realizadas na Fase Unpack

A seguir estão as técnicas aplicadas (e planejadas) para levantar informações e organizar o entendimento do grupo. Nesta etapa, o **Brainstorming** foi utilizado como ponto de partida para consolidar a ideia do grupo, e os resultados foram estruturados com **5W2H** e complementados por **Benchmarking**, com o objetivo de reduzir incertezas antes das próximas fases.

## [Brainstorming (ponto de partida)](Base/2-Artefato-Generalista/Brainstorm.md)

- **Objetivo**: Organizar as ideias iniciais do grupo sobre o CaronaAmigaFCTE, levantando possibilidades de funcionalidades, cenários de uso e preocupações relevantes para o domínio do problema.

O artefato completo se encontra em **[Brainstorming](Base/2-Artefato-Generalista/Brainstorm.md)**.

<details>
  <summary size="20"><b>Apresentação do brainstorming</b></summary>

- A atividade foi realizada em reunião do grupo, com registro das ideias e consolidação em um artefato.
- O brainstorming serviu como base para:
  - alinhar a proposta inicial do produto;
  - identificar temas recorrentes (pareamento de horários/rotas, combinados e previsibilidade);
  - levantar pontos de atenção do domínio (confiança, segurança e cancelamentos);
  - orientar a elaboração dos Rich Pictures individuais, a partir dos tópicos discutidos.

---

  <div align="center">
              Figura 1: Brainstorming.
          </div>

![Brainstorm](../assets/Brainstorm.png)

<font size="2"><p style="text-align: center">Fonte: [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS), 2026.</p></font>

</details>

## [5W + 2H](Base/2-Artefato-Generalista/5w2h.md)

- **Objetivo**: Estruturar e registrar o entendimento do projeto por meio de perguntas-guia (What, Why, Where, When, Who, How, How much), explicitando escopo inicial, público e restrições.

O artefato completo se encontra em **[5W2H](Base/2-Artefato-Generalista/5w2h.md)**.

<details>
  <summary size="20"><b>Síntese obtida</b></summary>

- O 5W+2H consolida o entendimento do Unpack e apoia a transição para as próximas fases, deixando claro:
  - o que o produto é (e o que não é);
  - para quem é;
  - em quais cenários será mais útil;
  - quais restrições e custos são relevantes;
  - quais decisões ainda dependem de validação nas etapas seguintes.

  <font size="3"><p style="text-align: center">Tabela 1: 5W2H do Projeto CaronaAmiga</p></font>
  
  | Pergunta | Resposta |
  |----------|----------|
  | **What?** (O que será feito?) | Web App para facilitar a comunicação e conexão entre estudantes da FCTE que necessitam compartilhar deslocamentos, oferecendo e recebendo caronas de forma organizada e segura. |
  | **Why?** (Por que será feito?) | Resolver o desafio de mobilidade enfrentado pela comunidade acadêmica [[3]](#referências-bibliográficas), promovendo economia de recursos financeiros e temporais, melhorando a qualidade de vida dos usuários através de trajetos mais confortáveis e compartilhados, além de contribuir para sustentabilidade ambiental pela redução de veículos em circulação. |
  | **Where?** (Onde será feito?) | Será desenvolvido remotamente e a plataforma final será hospedada em ambiente cloud, acessível via navegadores web em dispositivos mobile e desktop. <br> O time de desenvolvimento terá reuniões presenciais na Universidade de Brasília - Campus Gama, FCTE, sempre que necessário. |
  | **When?** (Quando será feito?) | Semestre letivo 2026.1 da UnB (março a julho), respeitando o cronograma da disciplina de Arquitetura e Desenho de Software, com entregas incrementais conforme as fases definidas. |
  | **Who?** (Quem fará?) | **Público-alvo:** compreende estudantes de graduação e pós-graduação da FCTE com necessidade recorrente de deslocamento. <br>**Equipe responsável:** é composta pelos dez [integrantes do Grupo 07 - CaronaAmiga FCTE](?id=alunos), todos estudantes de Engenharia de Software da Universidade de Brasília. <br> **Observação:** poderão ser adotados outros desenvolvedores ao final do projeto, caso o mesmo extrapole para além da disciplina. O objetivo é que esse projeto seja Open-Source e uma conquista dos próprios estudantes.  |
  | **How?** (Como será feito?) | Metodologia XP (Extreme Programming) [[4]](#referências-bibliográficas) adaptada, combinada com práticas ágeis. Ciclos iterativos curtos com testes automatizados, integração contínua, programação em pares, refatoração contínua e reuniões diárias. <br>**Stack**: Frontend (React/Vue.js), Backend (Node.js/Python), BD (PostgreSQL), Hospedagem (Firebase/AWS), Versionamento (Git/GitHub), Comunicação (WhatsApp/GitHub Projects/Issues/PRs). |
  | **How Much?** (Quanto vai custar?) | **Financeiro**: Infraestrutura acadêmica UnB (sem custos diretos). Ferramentas gratuitas (GitHub, Firebase/AWS free tier, Figma educacional). <br>**Pessoas**: Em média 120h (60h disciplina + 60h extra-classe) por integrante no semestre letivo de 2026.1 englobando estudo, análise, design, desenvolvimento, testes e documentação.<br> **Tecnológico**: Computadores pessoais, cloud computing gratuito e ferramentas colaborativas online. |
  
  <font size="2"><p style="text-align: center">Fonte: [Ana Victória](https://github.com/navicg), [João Marcos](https://github.com/JJOAOMARCOSS) e [Wanjo Christopher](https://github.com/wChrstphr),  2026.</p></font>

</details>

## [Benchmarking](Base/2-Artefato-Generalista/Benchmarking.md) 

- **Objetivo**: Analisar soluções similares para identificar boas práticas e riscos comuns (sem copiar soluções), especialmente em pareamento de rotas/horários, mecanismos de confiança, confirmação de carona e redução de no-show/cancelamentos.

O artefato completo se encontra em **[Benchmarking](Base/2-Artefato-Generalista/Benchmarking.md)**.

<details>
  <summary size="20"><b>Síntese do benchmarking</b></summary>

As referências analisadas foram escolhidas por afinidade com o problema de mobilidade e coordenação de caronas. Entre elas, destacam-se:

- **Marketplaces de carona**: BlaBlaCar (ênfase em perfil, reputação e fluxo de solicitação/aceite).
- **Apps de mobilidade**: Uber e 99 (ênfase em segurança, acompanhamento, notificações e comunicação).
- **Mapas e rotas**: Google Maps e Waze (rota, ETA e suporte a ponto de encontro).
- **Comunicação**: WhatsApp e Telegram (coordenação “manual” via mensagens e envio de localização).

Principais aprendizados extraídos para o contexto do CaronaAmigaFCTE:
- **Confiança e segurança** precisam estar no centro (perfil, avaliações, denúncia/bloqueio e suporte).
- **Previsibilidade operacional** depende de confirmação/atualização de status e regras claras (cancelamento, atrasos, combinados).
- **Apoio por mapa** reduz ruído: rota/ETA e ponto de encontro tornam o combinado mais objetivo.
- **Comunicação contextual** (chat após solicitação/aceite) evita dispersão e melhora rastreabilidade.

Como resultado, a equipe consolidou uma **tabela comparativa** e elicitou **requisitos funcionais e não funcionais iniciais** no artefato de **[Benchmarking](Base/2-Artefato-Generalista/Benchmarking.md)**.

</details>

## Resultados e Direcionamentos

Com base no que foi levantado nesta fase, o projeto segue orientado por:
- Um problema inicial delimitado: facilitar caronas da/para a FCTE considerando compatibilidade de rotas/horários e fatores de confiança.
- Um ponto de partida compartilhado (brainstorming), com estruturação das decisões iniciais (5W2H) e evidências complementares (benchmarking).
- Pontos de atenção para as próximas fases do Design Sprint:
  - reduzir ambiguidade no “combinado” (informações mínimas, confirmações e regras);
  - lidar com previsibilidade (cancelamentos, atrasos e mudanças de planos);
  - considerar confiança e segurança como requisitos centrais do domínio.

---

## Síntese do Entendimento (Objetivos x Evidências)

<font size="3"><p style="text-align: center">Tabela 2: Síntese do entendimento na fase Unpack.</p></font>

<div style="text-align: center;">

| Objetivo da fase Entender (Unpack) | Evidências / Compreensão obtida (artefatos) |
|---|---|
| Consolidar o entendimento inicial do problema de mobilidade na FCTE | O **Brainstorming** reuniu cenários recorrentes (rotas/horários), dores (atrasos/cancelamentos) e preocupações (segurança). |
| Delimitar o escopo inicial e alinhar o que será construído | O **5W2H** estruturou o plano inicial (o quê/por quê/onde/quando/quem/como/quanto), reduzindo ambiguidades sobre escopo e público-alvo. |
| Identificar necessidades e riscos prioritários do usuário | Foram destacados como essenciais: **previsibilidade do combinado**, **comunicação objetiva** e **mecanismos de confiança** (perfil, avaliação e denúncia). |
| Comparar referências e extrair boas práticas aplicáveis ao contexto universitário | O **Benchmarking** reforçou padrões de referência (uso de mapa/ETA/ponto de encontro, confirmação/atualização de status, reputação e suporte). |
| Preparar a transição para a fase Esboçar (Sketch) | A síntese desta etapa orienta a geração de soluções focadas em: pareamento por rota/horário, confirmação, ponto de encontro e segurança. |

</div>

<font size="2"><p style="text-align: center">Fonte: [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS), 2026.</p></font>

---

## Referências Bibliográficas

> <a id="referências-bibliográficas">1.</a> SOUL DIGITAL. Design Sprint: resultados a curto prazo em 5 etapas. Medium, 27 jul. 2018. Disponível em: https://medium.com/@souldigitalbr/design-sprint-resultados-a-curto-prazo-em-5-etapas-44fe9372c47a. Acesso em: 31 mar. 2026.
>
> <a id="REF2">2.</a> WANKHADE, Mayur. What are the 5 Stages of a Design Sprint? Nitor Infotech. Disponível em: https://www.nitorinfotech.com/blog/what-are-the-5-stages-of-a-design-sprint/. Acesso em: 31 mar. 2026.
>
> <a id="REF3">3.</a> 3PM3. O que é Design Sprint e como aplicar o método para testar e validar ideias. PM3, 10 mar. 2025. Disponível em: https://pm3.com.br/blog/design-sprint/. Acesso em: 31 mar. 2026.
> <a id="REF4">4.</a> UnBArqDsw (Turma 02). **Galáxia Conectada — Design Sprint (Entender)**. Disponível em: https://unbarqdsw2025-1-turma02.github.io/2025.1-T02-_G9_GalaxiaConectada_Entrega01/#/Base/DesignSprint/Entender. Acesso em: 03 abr. 2026.

## Histórico de Versões

| Versão | Data | Descrição | Autor(es) | Revisor(es) | Detalhes da revisão |
| :----: | :--: | --------- | ----------- | ------ | :---: |
| 1.0  | 31/03/2026 | Criação do documento [#30](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/issues/30) | [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS) | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | Artefato revisado |
| 1.1  | 03/03/2026 | Arrumando os textos, links e referencias [#30](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/issues/30) | [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS) | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | Artefato revisado e arrumado os links |
| 1.2  | 03/03/2026 | Modificações nas tabelas [#30](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/issues/30) | [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS) | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | Artefato revisado e arrumado as tabelas |
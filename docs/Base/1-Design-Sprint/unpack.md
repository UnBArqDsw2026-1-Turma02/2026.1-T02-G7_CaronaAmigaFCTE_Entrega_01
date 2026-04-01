# Design Spring – Entender (Unpack)

## Introdução

O **Design Sprint** é uma abordagem estruturada de trabalho em etapas, criada para reduzir incertezas e acelerar decisões sobre produtos, organizando o processo em fases bem definidas (Entender, Esboçar, Decidir, Prototipar e Testar) [[1]](#referências-bibliográficas). Em vez de começar direto na solução, o método prioriza a construção de entendimento compartilhado sobre o problema, o usuário e o contexto, para que as decisões seguintes sejam mais consistentes [[3]](#REF3).

Neste documento, o foco está na etapa **Entender (Unpack)**, que tem como função consolidar o conhecimento inicial do time e alinhar o que será considerado base do projeto antes de avançar para escolhas de solução [[2]](#REF2). Para o **CaronaAmigaFCTE**, essa etapa é especialmente importante porque o domínio do problema envolve variáveis como rotas e horários, além de fatores de confiança e segurança, que precisam estar explícitos e acordados pelo grupo desde o início.

## Contexto e Problema

O projeto **CaronaAmigaFCTE** tem como proposta apoiar o compartilhamento de caronas **da/para a FCTE**, considerando um cenário com deslocamentos recorrentes (aulas, atividades acadêmicas e rotinas de trabalho/estudo).

Problema observado (formulação inicial):
- Dificuldade de encontrar caronas compatíveis com horários e rotas de forma prática.
- Falta de previsibilidade (cancelamentos, atrasos, mudanças de planos).
- Questões de confiança e segurança ao combinar caronas com pessoas desconhecidas.
- Custo e tempo de deslocamento como fatores relevantes para adesão.

Premissas iniciais (ajustar conforme decisão do grupo):
- Público principal: **[preencher: estudantes / servidores / comunidade externa]**.
- Plataforma alvo: **[preencher: web / mobile / ambos]**.
- Escopo geográfico típico: **[preencher: Brasília/DF, RAs mais comuns]**.
- Restrições: não usar nome de serviço real/proprietário; proposta deve ser original (baseada apenas em referências).

## Ideia Inicial do Projeto

Data de referência: **28/03/2026** 

Ideia inicial:
- Desenvolver uma solução que permita **ofertar e buscar caronas** com origem/destino relacionados à FCTE, facilitando o pareamento entre motoristas e passageiros com base em informações essenciais (rota, horário, pontos de encontro e regras combinadas).

Compreensão inicial do grupo:
- O foco inicial estava em viabilizar o encontro entre pessoas e o registro das combinações de carona.
- Pontos críticos já percebidos desde o início: confiança entre usuários, clareza das informações e redução de “ruído” na comunicação (o combinado precisa ficar explícito).

## Atividades Realizadas na Fase Unpack

A seguir estão as técnicas aplicadas (e planejadas) para levantar informações e organizar o entendimento do grupo. Nesta etapa, o **Brainstorming** foi utilizado como ponto de partida para consolidar a ideia do grupo e orientar a produção dos **Rich Pictures individuais**, permitindo observar o mesmo problema sob perspectivas diferentes.

### [Brainstorming (ponto de partida)](../Base/2-Artefato-Generalista/Brainstorm.md)

- **Objetivo**: Organizar as ideias iniciais do grupo sobre o CaronaAmigaFCTE, levantando possibilidades de funcionalidades, cenários de uso e preocupações relevantes para o domínio do problema.

O artefato completo se encontra em [Brainstorming](../Base/2-Artefato-Generalista/Brainstorm.md).

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

### Rich Picture (individual)

- **Objetivo**: Representar visualmente os atores, relações, informações e conflitos do contexto de caronas da/para a FCTE, destacando elementos que impactam diretamente o problema (ex.: confiança, atrasos, cancelamentos, pontos de encontro).

Status e evidência:
- Artefato em elaboração/organização pelo grupo: **[inserir link do Rich Picture quando estiver no repositório]**.

<details>
  <summary size="20"><b>Como essa técnica se conectou ao Brainstorming</b></summary>

- Os Rich Pictures foram produzidos individualmente para capturar perspectivas diferentes sobre os mesmos tópicos levantados no brainstorming.
- A comparação entre visões individuais ajuda a identificar:
  - atores que aparecem com frequência (motorista, passageiro, comunidade FCTE e possíveis intermediários);
  - conflitos recorrentes (mudança de planos, no-show, atrasos, insegurança percebida);
  - informações essenciais do “combinado” (rota, horário, ponto de encontro, regras e contato).

</details>

### Questionário

- **Objetivo**: Coletar dados iniciais sobre perfil, rotinas, dores e aceitação de uma solução de caronas no contexto da FCTE, para apoiar decisões de escopo com base em evidências.

Status e evidência:
- Artefato em elaboração/organização pelo grupo: **[inserir link do Questionário quando estiver no repositório]**.

<details>
  <summary size="20"><b>O que será destacado nos resultados</b></summary>

- Perfil dos respondentes (vínculo com a FCTE e frequência de deslocamento).
- Critérios mais importantes para aceitar uma carona (segurança, custo, tempo, flexibilidade).
- Principais dificuldades atuais (encontrar carona compatível, comunicação, cancelamentos).
- Canais atualmente usados para combinar carona (para entender hábitos e expectativas).

</details>

### 5W + 2H

- **Objetivo**: Estruturar e registrar o entendimento do projeto por meio de perguntas-guia (What, Why, Where, When, Who, How, How much), explicitando escopo inicial, público e restrições.

Status e evidência:
- Artefato em elaboração/organização pelo grupo: **[inserir link do 5W+2H quando estiver no repositório]**.

<details>
  <summary size="20"><b>Síntese esperada</b></summary>

- O 5W+2H consolida o entendimento do Unpack e apoia a transição para as próximas fases, deixando claro:
  - o que o produto é (e o que não é);
  - para quem é;
  - em quais cenários será mais útil;
  - quais restrições e custos são relevantes;
  - quais decisões ainda dependem de validação nas etapas seguintes.

</details>

### Benchmarking (planejado)

- **Objetivo**: Analisar soluções similares para identificar boas práticas e riscos comuns (sem copiar soluções), especialmente em pareamento de rotas/horários, mecanismos de confiança, confirmação de carona e redução de no-show/cancelamentos.

Status:
- Atividade prevista; ainda não finalizada.

## Resultados e Direcionamentos

Com base no que foi levantado nesta fase, o projeto segue orientado por:
- Um problema inicial delimitado: facilitar caronas da/para a FCTE considerando compatibilidade de rotas/horários e fatores de confiança.
- Um ponto de partida compartilhado (brainstorming) e aprofundamento do contexto (rich pictures), preparando o grupo para decisões mais seguras nas próximas etapas.
- Pontos de atenção para as próximas fases do Design Sprint:
  - reduzir ambiguidade no “combinado” (informações mínimas, confirmações e regras);
  - lidar com previsibilidade (cancelamentos, atrasos e mudanças de planos);
  - considerar confiança e segurança como requisitos centrais do domínio.

## Síntese do Entendimento (Objetivos x Evidências)

<font size="3"><p style="text-align: center">Tabela 1: Síntese do entendimento.</p></font>

<div style="text-align: center;">

| Objetivo | Evidências/Compreensão obtida |
|---|---|
| Identificar o problema e o contexto | Brainstorming e Rich Pictures ajudaram a mapear cenários típicos, atores e dificuldades recorrentes. |
| Levantar hipóteses de necessidades | Brainstorming gerou hipóteses iniciais; questionário apoia confirmação/ajustes com dados. |
| Mapear atores e impactos | Rich Pictures destacam relações, conflitos e informações essenciais para o “combinado”. |
| Organizar escopo inicial | 5W+2H consolida escopo, público, cenários e restrições do projeto. |
| Preparar comparação com mercado | Benchmarking foi definido como próximo passo para extrair boas práticas e riscos comuns. |

</div>




---

## Referências Bibliográficas

> <a id="referências-bibliográficas">1.</a> SOUL DIGITAL. Design Sprint: resultados a curto prazo em 5 etapas. Medium, 27 jul. 2018. Disponível em: https://medium.com/@souldigitalbr/design-sprint-resultados-a-curto-prazo-em-5-etapas-44fe9372c47a. Acesso em: 31 mar. 2026.

> <a id="REF2">2.</a> WANKHADE, Mayur. What are the 5 Stages of a Design Sprint? Nitor Infotech. Disponível em: https://www.nitorinfotech.com/blog/what-are-the-5-stages-of-a-design-sprint/. Acesso em: 31 mar. 2026.

> <a id="REF3">3.</a> 3PM3. O que é Design Sprint e como aplicar o método para testar e validar ideias. PM3, 10 mar. 2025. Disponível em: https://pm3.com.br/blog/design-sprint/. Acesso em: 31 mar. 2026.

## Histórico de Versões

| Versão | Data | Descrição | Autor(es) | Revisor(es) | Detalhes da revisão |
| :----: | :--: | --------- | ----------- | ------ | :---: |
| 1.0  | 31/03/2026 | Criação do documento [#30](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/issues/30) | [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS) | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | - |
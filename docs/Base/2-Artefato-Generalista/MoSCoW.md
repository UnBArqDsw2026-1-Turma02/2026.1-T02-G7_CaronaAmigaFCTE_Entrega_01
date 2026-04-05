# MoSCoW - Priorização de Requisitos

## Introdução

O artefato MoSCoW é uma técnica de priorização fundamental no gerenciamento de requisitos de software. Seu objetivo é auxiliar a equipe do projeto Carona Amiga FCTE a identificar quais funcionalidades são críticas para o lançamento inicial e quais podem ser desenvolvidas em etapas posteriores, garantindo que o foco permaneça na entrega de valor real para a comunidade acadêmica da UnB Gama.

## Metodologia

A técnica MoSCoW foi utilizada para categorizar os requisitos do sistema de acordo com seu nível de prioridade, considerando o impacto para o negócio e a viabilidade de implementação.
Os requisitos foram organizados em quatro níveis:

- Must Have (Deve ter): Correspondem aos requisitos essenciais, inegociáveis e críticos para o lançamento do sistema. Sem eles, a aplicação de caronas não cumpre sua função principal, não oferece segurança adequada ou não se mostra viável para uso. Esses requisitos compõem o MVP (Produto Mínimo Viável).

- Should Have (Deveria ter): Representam requisitos importantes que agregam valor significativo ao- sistema, embora sua ausência não inviabilize o funcionamento da aplicação no curto prazo. São funcionalidades desejáveis para uma experiência mais completa, mas que não comprometem a operação básica da plataforma.

- Could Have (Poderia ter): Incluem requisitos desejáveis que melhoram a experiência do usuário e enriquecem o sistema, mas que não são essenciais para sua operação principal. Podem ser implementados caso haja tempo e recursos disponíveis, sem comprometer a entrega principal.

- Won't Have (Não terá agora): Englobam requisitos considerados interessantes e potencialmente úteis, mas que ficam fora do escopo da primeira versão do sistema. Esses itens podem ser avaliados e incorporados em versões futuras, conforme a evolução do projeto.

## Requisitos

Durante a construção do [brainstorming](Brainstorm.md) e do [benchmarking](Benchmarking.md), que são ferramentas utilizadas para a elicitação de requisitos, a equipe consolidou as principais necessidades do usuário, identificou funcionalidades e alinhou prioridades para a primeira entrega da disciplina. A partir dessas atividades, surgiram os seguintes itens:

<details>
<summary>Requisitos Funcionais </summary>

### Tabela de Requisitos Funcionais (RF)

<font size="3"><p style="text-align: center">Tabela 1: Requisitos Funcionais - [Brainstorming](Brainstorm.md)</p></font>

|        Código         | Requisito Funcional             | Objetivo                                                      |
| :-------------------: | :------------------------------ | :------------------------------------------------------------ |
| <a id="rf01"></a>RF01 | Cadastrar usuário.              | Aumentar a confiança entre motorista e passageiro.            |
| <a id="rf03"></a>RF03 | Visualizar perfil.              | Apoiar decisão segura na escolha de motoristas e passageiros. |
| <a id="rf04"></a>RF04 | Avaliar viagens.                | Construir reputação e melhorar a qualidade das caronas.       |
| <a id="rf05"></a>RF05 | Favoritar motoristas.           | Facilitar recorrência de caronas confiáveis.                  |
| <a id="rf06"></a>RF06 | Enviar mensagem.                | Melhorar a comunicação antes e durante a viagem.              |
| <a id="rf07"></a>RF07 | Criar grupo de carona.          | Viabilizar caronas fixas na semana.                           |
| <a id="rf08"></a>RF08 | Publicar carona.                | Atender demandas imediatas de deslocamento.                   |
| <a id="rf09"></a>RF09 | Enviar notificações de caronas. | Aumentar chance de correspondência entre oferta e demanda.    |
| <a id="rf10"></a>RF10 | Gerar grade horária de caronas. | Facilitar planejamento de ida e volta.                        |
| <a id="rf13"></a>RF13 | Gerar mapa com caronas.         | Melhorar visualização espacial das opções.                    |
| <a id="rf14"></a>RF14 | Sugerir melhores rotas.         | Reduzir tempo de deslocamento e atrasos.                      |
| <a id="rf17"></a>RF17 | Compartilhar localização.       | Aumentar rastreabilidade e segurança.                         |
| <a id="rf18"></a>RF18 | Detectar desvio da rota.        | Reagir rapidamente a situações de risco.                      |
| <a id="rf19"></a>RF19 | Notificar contatos.             | Oferecer resposta imediata em incidentes.                     |
| <a id="rf20"></a>RF20 | Validar embarque.               | Confirmar identidade e evitar fraudes.                        |
| <a id="rf21"></a>RF21 | Editar perfil.                  | Garantir uma experiência personalizada ao usuário.            |
| <a id="rf24"></a>RF24 | Registrar histórico.            | Permitir auditoria, consulta e transparência para o usuário.  |
| <a id="rf25"></a>RF25 | Recomendar caronas.             | Melhorar pontualidade e aderência às necessidades do usuário. |

<font size="2"><p style="text-align: center">Fonte: [Wanjo Christopher](https://github.com/wChrstphr), 2026.</p></font>

<font size="3"><p style="text-align: center">Tabela 2: Requisitos Funcionais - [Benchmarking](Benchmarking.md)</p></font>

|        Código         | Requisito Funcional   | Objetivo                                                  | Rastreabilidade                                                                                             |
| :-------------------: | :-------------------- | :-------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------- |
| <a id="rf26"></a>RF26 | Cancelar solicitação. | Reduzir ruídos e melhorar rastreabilidade de ocorrências. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/); [BlaBlaCar](https://www.blablacar.com.br/) |
| <a id="rf27"></a>RF27 | Bloquear usuário.     | Reforçar segurança e moderação da plataforma.             | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/)                                             |

<font size="2"><p style="text-align: center">Fonte: [João Marcos](https://github.com/JJOAOMARCOSS), [Luiza da Silva](https://github.com/luizaxx) e [Wanjo Christopher](https://github.com/wChrstphr), 2026.</p></font>

</details>

<details>
<summary>Requisitos Não Funcionais</summary>

> Legenda FURPS+: F = Functionality, U = Usability, R = Reliability, P = Performance, S = Supportability, + = Restrições legais/técnicas ([3](#ref3)).
> <font size="3"><p style="text-align: center">Tabela 3: Requisitos Não-Funcionais - [Brainstorming](Brainstorm.md)</p></font>

|         Código          |        Categoria FURPS+        | Requisito Não Funcional                                                                                                                                                                  | Objetivo                                                                       |
| :---------------------: | :----------------------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------- |
| <a id="rnf01"></a>RNF01 |        Usabilidade (U)         | O sistema deve ser responsivo para desktop padrão (1900x1040 e 1366x768), tablet (768x1024) e mobile (390x844, 414x896 e 360x640).                                                       | Garantir boa usabilidade para estudantes e motoristas em qualquer dispositivo. |
| <a id="rnf02"></a>RNF02 |        Performance (P)         | O sistema deve responder em menos de 2 segundos nas operações principais (buscar carona, publicar carona e abrir mapa), medido em p90 ([4](#ref4)).                                      | Manter navegação fluida para passageiros e motoristas.                         |
| <a id="rnf04"></a>RNF04 |        Reliability (R)         | O sistema deve manter disponibilidade mensal mínima de 99,5% ([6](#ref6)), com monitoramento de uptime ([5](#ref5)), alertas automáticos e plano de contingência para indisponibilidade. | Evitar interrupções no uso diário da plataforma.                               |
| <a id="rnf05"></a>RNF05 |        Usabilidade (U)         | O sistema deve atender à acessibilidade conforme WCAG 2.1 nível AA ([7](#ref7)), incluindo contraste adequado, navegação por teclado, textos alternativos e suporte a leitores de tela.  | Incluir pessoas com deficiência no uso da plataforma.                          |
| <a id="rnf06"></a>RNF06 |        Usabilidade (U)         | O sistema deve apresentar linguagem clara e fluxo organizado ([8](#ref8)) para ações centrais, com validação por testes de usabilidade com novos usuários.                               | Reduzir curva de aprendizado para iniciantes.                                  |
| <a id="rnf07"></a>RNF07 |        Performance (P)         | O sistema deve suportar aumento gradual de usuários por meio de escalabilidade horizontal e cache, mantendo tempo de resposta dentro da meta sob carga concorrente definida.             | Preservar desempenho durante crescimento da base de usuários.                  |
| <a id="rnf09"></a>RNF09 |       Supportability (S)       | O sistema deve funcionar nas duas últimas versões estáveis de Chrome, Firefox, Edge e Safari, com testes de compatibilidade a cada release.                                              | Assegurar acesso para a maioria dos usuários em navegadores modernos.          |
| <a id="rnf10"></a>RNF10 |        Performance (P)         | O sistema deve operar com internet limitada utilizando carregamento progressivo, compressão de recursos e fallback para modo de baixo consumo de dados em rede 3G/4G instável.           | Manter acesso para usuários em conexões lentas ou instáveis.                   |
| <a id="rnf11"></a>RNF11 |        Performance (P)         | O sistema deve entregar notificações críticas (emergência e desvio de rota) com latência de até 5 segundos após o evento, com retentativas automáticas de envio.                         | Permitir reação rápida em situações urgentes de segurança.                     |
| <a id="rnf12"></a>RNF12 | Restrições legais/técnicas (+) | O sistema deve coletar localização e gravações somente com consentimento explícito, registrar finalidade de uso e permitir revogação pelo usuário em conformidade com a LGPD.            | Preservar privacidade e conformidade regulatória para motorista e passageiro.  |
| <a id="rnf13"></a>RNF13 |       Functionality (F)        | O sistema deve registrar trilhas de auditoria para cadastro, avaliação, pagamento, emergência e alteração de perfil, com carimbo de data/hora e retenção por período definido.           | Aumentar rastreabilidade para usuários e equipe administrativa.                |

<font size="2"><p style="text-align: center">Fonte: [Wanjo Christopher](https://github.com/wChrstphr), 2026.</p></font>

<font size="3"><p style="text-align: center">Tabela 4: Requisitos Não Funcionais - [Benchmarking](Benchmarking.md)</p></font>

|         Código          |  Categoria FURPS+   | Requisito Não Funcional                                                                                           | Objetivo                                                 | Rastreabilidade                                                                                             |
| :---------------------: | :-----------------: | :---------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------- |
| <a id="rnf14"></a>RNF14 |   Usabilidade (U)   | O sistema deve ser responsivo para desktop e mobile.                                                              | Garantir uso consistente em diferentes dispositivos.     | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/)                                             |
| <a id="rnf15"></a>RNF15 | Suportabilidade (S) | O sistema deve proteger dados sensíveis com boas práticas de segurança (hash de senha, TLS e controle de acesso). | Preservar privacidade e integridade das contas.          | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/)                                             |
| <a id="rnf16"></a>RNF16 |   Usabilidade (U)   | O sistema deve ter fluxo simples para ações críticas (criar, buscar e aceitar carona em poucos passos).           | Reduzir fricção de uso e tempo para completar tarefas.   | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/); [BlaBlaCar](https://www.blablacar.com.br/) |
| <a id="rnf17"></a>RNF17 | Confiabilidade (R)  | O sistema deve registrar logs de ações relevantes (aceites, cancelamentos e denúncias).                           | Aumentar auditabilidade e suporte a incidentes.          | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/)                                             |
| <a id="rnf18"></a>RNF18 |   Performance (P)   | O sistema deve apresentar rotas e estimativas de tempo de forma consistente.                                      | Melhorar previsibilidade da experiência de deslocamento. | [Google Maps](https://www.google.com/maps)/[Waze](https://www.waze.com/)                                    |

<font size="2"><p style="text-align: center">Fonte: [João Marcos](https://github.com/JJOAOMARCOSS), [Luiza da Silva](https://github.com/luizaxx) e [Wanjo Christopher](https://github.com/wChrstphr), 2026.</p></font>

</details>

## Priorização MoSCoW

## Descrição da Priorização

A priorização de requisitos é uma etapa fundamental no desenvolvimento de software, pois permite organizar e direcionar os esforços da equipe com base no valor entregue ao usuário e na viabilidade de implementação.

A classificação dos requisitos foi realizada com base em critérios como a essencialidade para o funcionamento do sistema, impacto na segurança dos usuários, complexidade de implementação e valor agregado à experiência do usuário. Além disso, foram utilizadas perguntas orientadoras, como: “o sistema funciona sem este requisito?” e “este requisito é necessário para o objetivo principal da aplicação?”.

Essa priorização permite definir claramente o escopo do MVP, reduzir riscos durante o desenvolvimento e garantir que os recursos do projeto sejam direcionados para as funcionalidades de maior impacto.

### Must Have (Deve ter)

<font size="3"><p style="text-align: center">Tabela 5: Must Have</p></font>

| Código          | Requisito                                 | Justificativa                                               |
| --------------- | ----------------------------------------- | ----------------------------------------------------------- |
| [RF01](#rf01)   | Cadastrar usuário                         | Essencial para identificação e acesso ao sistema            |
| [RF03](#rf03)   | Visualizar perfil                         | Necessário para tomada de decisão segura entre usuários     |
| [RF06](#rf06)   | Enviar mensagem                           | Parte central da negociação da carona dentro da plataforma  |
| [RF08](#rf08)   | Publicar carona                           | Funcionalidade principal do sistema                         |
| [RF17](#rf17)   | Compartilhar localização                  | Fundamental para segurança e acompanhamento da viagem       |
| [RF20](#rf20)   | Validar embarque                          | Garante identidade dos usuários e evita fraudes             |
| [RF26](#rf26)   | Cancelar solicitação                      | Necessário para controle básico do fluxo de uso             |
| [RNF01](#rnf01) | Responsividade (webapp mobile-first)      | Essencial devido ao uso predominante em dispositivos móveis |
| [RNF02](#rnf02) | Resposta em menos de 2 segundos nas operações principais | Necessário para garantir usabilidade mínima do sistema      |
| [RNF12](#rnf12) | Conformidade com LGPD                     | Obrigatório para tratamento de dados pessoais               |
| [RNF15](#rnf15) | Segurança (hash, TLS, controle de acesso) | Essencial para proteção de dados e integridade do sistema   |

<font size="2"><p style="text-align: center"> Fonte: Elaborado pelo autor ([Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima), 2026)</p></font>

### Should Have (Deveria ter)

<font size="3"><p style="text-align: center">Tabela 6: Should Have</p></font>

| Código          | Requisito                            | Justificativa                                                         |
| --------------- | ------------------------------------ | --------------------------------------------------------------------- |
| [RF04](#rf04)   | Avaliar viagens                      | Importante para reputação, mas não essencial ao funcionamento         |
| [RF09](#rf09)   | Notificações                         | Melhora engajamento e comunicação, mas não é crítico                  |
| [RF13](#rf13)   | Mapa de caronas                      | Facilita visualização, mas pode ser substituído por lista             |
| [RF14](#rf14)   | Sugestão de rotas                    | Otimiza experiência, mas não impede funcionamento                     |
| [RF24](#rf24)   | Histórico de viagens                 | Útil para consulta, mas não essencial para operação inicial           |
| [RNF04](#rnf04) | Disponibilidade 99,5%                | Importante para confiabilidade, mas pode evoluir com o tempo          |
| [RNF05](#rnf05) | Acessibilidade (WCAG 2.1)            | Relevante para inclusão, mas pode ser aprimorado após MVP             |
| [RNF06](#rnf06) | Usabilidade e fluxo simples          | Melhora experiência, mas sistema pode funcionar sem refinamento total |
| [RNF16](#rnf16) | Fluxo simplificado de ações críticas | Reduz fricção, mas não impede uso inicial                             |

<font size="2"><p style="text-align: center"> Fonte: Elaborado pelo autor ([Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima), 2026)</p></font>

### Could Have (Poderia ter)

<font size="3"><p style="text-align: center">Tabela 7: Could Have</p></font>

| Código          | Requisito                       | Justificativa                                      |
| --------------- | ------------------------------- | -------------------------------------------------- |
| [RF05](#rf05)   | Favoritar motoristas            | Funcionalidade de conveniência                     |
| [RF07](#rf07)   | Grupo de carona                 | Melhoria para uso recorrente                       |
| [RF10](#rf10)   | Grade horária                   | Apoia planejamento, mas não é essencial            |
| [RF25](#rf25)   | Recomendar caronas              | Funcionalidade avançada de personalização          |
| [RNF07](#rnf07) | Escalabilidade                  | Importante para crescimento futuro                 |
| [RNF09](#rnf09) | Compatibilidade com navegadores | Relevante, mas pode ser expandido gradualmente     |
| [RNF10](#rnf10) | Operação em internet limitada   | Melhoria de acessibilidade em cenários específicos |
| [RNF11](#rnf11) | Latência de notificações        | Importante, mas não crítica no MVP                 |

<font size="2"><p style="text-align: center"> Fonte: Elaborado pelo autor ([Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima), 2026)</p></font>

### Won’t Have (Não terá agora)

<font size="3"><p style="text-align: center">Tabela 8: Won't Have </p></font>

| Código          | Requisito                  | Justificativa                                |
| --------------- | -------------------------- | -------------------------------------------- |
| [RF18](#rf18)   | Detectar desvio de rota    | Alta complexidade técnica para o MVP         |
| [RF19](#rf19)   | Notificar contatos         | Funcionalidade avançada de segurança         |
| [RF27](#rf27)   | Bloquear usuário           | Pode ser implementado em versões futuras     |
| [RNF13](#rnf13) | Auditoria completa         | Recurso avançado para versões futuras        |
| [RNF18](#rnf18) | Precisão avançada de rotas | Complexidade elevada e baixo impacto inicial |

<font size="2"><p style="text-align: center"> Fonte: Elaborado pelo autor ([Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima), 2026)</p></font>

## Histórico de Versões

| Versão |    Data    | Descrição                                                                                                                | Autor(es)                                                                                                                                                                                        | Revisor(es)                                                                                   | Detalhes da revisão |
| :----: | :--------: | :----------------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :-------------------------------------------------------------------------------------------- | :-----------------: |
|  1.0   | 04/04/2026 | Criação do Artefato [#21](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/issues/21) | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr), [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharess) e [João Vitor Santos de Oliveira](https://github.com/Jauzimm) | [João Marcos](https://github.com/JJOAOMARCOSS) e [Luiza da Silva](https://github.com/luizaxx) | Artefato revisado e ajustado. |
|  1.1   | 05/04/2026 | Adiciona a priorização dos requisitos   | [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima)  | [João Vitor Santos de Oliveira](https://github.com/Jauzimm) e [Karoline Luz da Conceição](https://github.com/KarolineLuz) | Artefato revisado e ajustado. |

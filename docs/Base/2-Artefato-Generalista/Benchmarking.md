# Benchmarking

## Introdução

O **benchmarking** é uma prática de análise comparativa usada para observar soluções existentes (produtos, serviços e processos), identificar abordagens consolidadas e extrair aprendizados que possam ser **adaptados** ao contexto de um novo projeto. Mais do que “copiar”, a proposta é entender *o que funciona*, *por que funciona* e *em quais condições*, para então tomar decisões de design e requisitos com menos incerteza [[1]](#ref1).

No contexto do **CaronaAmiga FCTE**, o benchmarking foi utilizado para levantar referências sobre: criação e busca de caronas, segurança e confiança entre usuários, comunicação motorista–passageiro, definição de pontos de encontro, uso de rotas/tempo estimado e mecanismos de avaliação.

## Objetivos

- Identificar funcionalidades e padrões de UX comuns em soluções de mobilidade e caronas.
- Levantar práticas de **segurança** (verificação, denúncias, reputação e privacidade).
- Apoiar a definição de requisitos iniciais do CaronaAmiga FCTE a partir de evidências observáveis.
- Mapear oportunidades de diferenciação para o contexto universitário (comunidade restrita e rotas recorrentes).

## Metodologia

A atividade foi conduzida como uma análise exploratória, com seleção de aplicativos ou soluções referência por afinidade com o problema que queremos resolver com o projeto, como mobilidade e coordenação de deslocamentos facilitada por meio de caronas. As soluções foram agrupadas por categoria e avaliadas de forma qualitativa com base em critérios como:

- **Onboarding e verificação** (conta, validação, perfis);
- **Busca/oferta e matching** (filtros, recorrência, sugestões);
- **Planejamento de rota** (mapa, ETA, pontos de encontro);
- **Comunicação** (chat, compartilhamento de local, avisos);
- **Confiança e segurança** (avaliações, denúncias, regras);
- **Custos** (rateio, combinação de valores, transparência).

As observações foram consolidadas em uma tabela comparativa e, ao final, transformadas em requisitos funcionais e não funcionais rastreáveis.

---

## Participantes

<font size="3"><p style="text-align: center">Tabela 1: Participantes</p></font>

<div style="text-align: center;">

| Aluno | Função | Data | Hora |
| :--: | :--: | :--: | :--: |
| [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharess) | Revisão do artefato Benchmarking | 01/04/2026 | 09:55 |
| [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS) | Elaboração do artefato Benchmarking | 31/03/2026 | 23:00 |
| [Luiza da Silva Pugas](https://github.com/luizaxx) | Elaboração do artefato Benchmarking | 31/03/2026 | 23:00 |
| [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | Elaboração do artefato Benchmarking | 31/03/2026 | 23:00 |

</div>

<font size="2"><p style="text-align: center">Fonte: [João Marcos](https://github.com/JJOAOMARCOSS), 2026.</p></font>

---

## Soluções analisadas (por categoria)

<details>
  <summary size="20"><b>Marketplaces de Carona</b></summary>

- [BlaBlaCar](https://www.blablacar.com.br/) — caronas intermunicipais e internacionais, focado nos perfis de usuário e comunicação entre passageiro e motorista.

</details>

<details>
  <summary size="20"><b>Apps de mobilidade sob demanda (padrões de UX e segurança)</b></summary>

- [Uber](https://www.uber.com/br/pt-br/) — fluxo de corrida, segurança, compartilhamento de viagem, preferência por motorista.
- [99](https://99app.com/) — fluxo de corrida, segurança, compartilhamento de viagem, preços mais baixos que Uber.

</details>

<details>
  <summary size="20"><b>Mapas e Rotas</b></summary>

- [Google Maps](https://www.google.com/maps) — rotas, estimativas de tempo e pontos no mapa.
- [Waze](https://www.waze.com/pt-BR/) — tráfego em tempo real, rotas dinâmicas.

</details>

<details>
  <summary size="20"><b>Comunicação em Grupos</b></summary>

- [WhatsApp](https://www.whatsapp.com/?lang=pt_BR) — coordenação feita por grupos, envio de localização e combinações rápidas.
- [Telegram](https://telegram.org/) — mesmas funcionalidades do WhatsApp para caronas.

</details>

---

## Tabela comparativa (síntese)

<font size="3"><p style="text-align: center">Tabela 2: Tabela comparativa</p></font>

| Critério | BlaBlaCar | Uber/99 | Google Maps/Waze | WhatsApp/Telegram |
| :-- | :--: | :--: | :--: | :--: |
| Perfil do usuário | ✅ | ✅ | ⚠️ (conta) | ✅ |
| Verificação/Confiança | ✅ (reputação) | ✅ (recursos de segurança) | ❌ | ❌ |
| Oferta e busca de carona | ✅ | ⚠️ (corrida, não carona) | ❌ | ⚠️ (manual) |
| Matching/sugestão | ✅ | ⚠️ | ❌ | ❌ |
| Definição de rota/ETA | ⚠️ | ✅ | ✅ | ❌ |
| Chat/comunicação | ✅ | ✅ | ❌ | ✅ |
| Ponto de encontro no mapa | ⚠️ | ✅ | ✅ | ⚠️ (manual) |
| Avaliação/reputação | ✅ | ✅ | ❌ | ❌ |
| Rateio/pagamento | ⚠️ (contribuição) | ✅ (pagamento nativo) | ❌ | ⚠️ (manual) |


<p style="text-align: center">Legenda: ✅ presente / ⚠️ parcial / ❌ ausente.</p>

<font size="2"><p style="text-align: center">Fonte: [João Marcos](https://github.com/JJOAOMARCOSS), [Luiza da Silva](https://github.com/luizaxx) e [Wanjo Christopher](https://github.com/wChrstphr), 2026.</p></font>

---

## Requisitos Elicitados

Com base na análise comparativa e nos critérios observados nas plataformas de referência, foram elicitados os seguintes requisitos iniciais para o CaronaAmiga FCTE.

<details>
<summary>Requisitos Funcionais</summary>

#### Tabela de Requisitos Funcionais (RF)

<font size="3"><p style="text-align: center">Tabela 3: Requisitos Funcionais</p></font>

| Código | Requisito Funcional | Objetivo | Rastreabilidade |
| :--: | :-- | :-- | :-- |
| <a id="rf01"></a>RF01 | Gerenciar perfil do usuário. | Aumentar confiança e personalização de uso. | [BlaBlaCar](https://www.blablacar.com.br/); [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| <a id="rf02"></a>RF02 | Criar oferta de carona. | Estruturar a oferta com informações mínimas para decisão. | [BlaBlaCar](https://www.blablacar.com.br/) |
| <a id="rf03"></a>RF03 | Buscar caronas. | Melhorar precisão no encontro entre oferta e demanda. | [BlaBlaCar](https://www.blablacar.com.br/) |
| <a id="rf04"></a>RF04 | Calcular ETA. | Apoiar planejamento e previsibilidade da viagem. | [Google Maps](https://www.google.com/maps)/[Waze](https://www.waze.com/); [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| <a id="rf05"></a>RF05 | Enviar mensagem. | Facilitar alinhamentos antes e durante a viagem. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/); [WhatsApp](https://www.whatsapp.com/?lang=pt_BR) |
| <a id="rf06"></a>RF06 | Solicitar participação. | Dar controle ao motorista e transparência ao passageiro. | [BlaBlaCar](https://www.blablacar.com.br/) |
| <a id="rf07"></a>RF07 | Cancelar solicitação. | Reduzir ruídos e melhorar rastreabilidade de ocorrências. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/); [BlaBlaCar](https://www.blablacar.com.br/) |
| <a id="rf08"></a>RF08 | Avaliar experiência. | Construir reputação e melhorar qualidade da comunidade. | [BlaBlaCar](https://www.blablacar.com.br/); [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| <a id="rf09"></a>RF09 | Bloquear usuário. | Reforçar segurança e moderação da plataforma. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| <a id="rf10"></a>RF10 | Enviar notificações. | Aumentar pontualidade e taxa de correspondência. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/); [WhatsApp](https://www.whatsapp.com/?lang=pt_BR) |

<font size="2"><p style="text-align: center">Fonte: [João Marcos](https://github.com/JJOAOMARCOSS), [Luiza da Silva](https://github.com/luizaxx) e [Wanjo Christopher](https://github.com/wChrstphr), 2026.</p></font>

#### Tabela de Especificações dos Requisitos Funcionais (ERF)

<font size="3"><p style="text-align: center">Tabela 4: Especificação dos Requisitos Funcionais</p></font>

| Código | Especificação | Objetivo |
| :--: | :-- | :-- |
| <a id="erf01"></a>[ERF01](#rf01) | Perfil com nome, curso/vínculo, foto obrigatória e preferências. | Melhorar identificação e confiança entre os usuários. |
| <a id="erf02"></a>[ERF02](#rf02) | Oferta de carona com origem, destino, horário, vagas e observações. | Padronizar publicação e facilitar decisão do passageiro. |
| <a id="erf03"></a>[ERF03](#rf03) | Busca com filtros por origem, destino, horário, recorrência e vagas. | Aumentar relevância dos resultados de carona. |
| <a id="erf04"></a>[ERF04](#rf04) | Visualização de rota, ETA e sugestão de ponto de encontro. | Apoiar coordenação e reduzir atrasos. |
| <a id="erf05"></a>[ERF05](#rf05) | Chat habilitado após solicitação/aceite. | Viabilizar comunicação contextual da viagem. |
| <a id="erf05"></a>[ERF05.1](#rf05) | Disponibilizar chat entre motorista e passageiro. | Viabilizar comunicação rápida entre partes. |
| <a id="erf06"></a>[ERF06](#rf06) | Solicitação de vaga com fluxo de aceite/recusa pelo motorista. | Garantir controle de lotação e segurança de embarque. |
| <a id="erf07"></a>[ERF07](#rf07) | Cancelamento com motivo e aviso automático às partes envolvidas. | Minimizar conflitos e manter histórico de eventos. |
| <a id="erf08"></a>[ERF08](#rf08) | Avaliação com nota e comentário opcional ao fim da carona. | Sustentar mecanismo de reputação. |
| <a id="erf09"></a>[ERF09](#rf09) | Mecanismo de denúncia/bloqueio e canal de suporte. | Permitir resposta a incidentes e condutas inadequadas. |
| <a id="erf10"></a>[ERF10](#rf10) | Notificações para match, aceite, alteração de horário e lembrete. | Aumentar engajamento e previsibilidade operacional. |

<font size="2"><p style="text-align: center">Fonte: [João Marcos](https://github.com/JJOAOMARCOSS), [Luiza da Silva](https://github.com/luizaxx) e [Wanjo Christopher](https://github.com/wChrstphr), 2026.</p></font>

</details>

<details>
<summary>Requisitos Não Funcionais</summary>

#### Tabela de Requisitos Não Funcionais (RNF)

<font size="3"><p style="text-align: center">Tabela 5: Requisitos Não Funcionais</p></font>

| Código | Categoria FURPS+ | Requisito Não Funcional | Objetivo | Rastreabilidade |
| :--: | :--: | :-- | :-- | :-- |
| RNF01 | Usabilidade (U) | O sistema deve ser responsivo para desktop e mobile. | Garantir uso consistente em diferentes dispositivos. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| RNF02 | Suportabilidade (S) | O sistema deve proteger dados sensíveis com boas práticas de segurança (hash de senha, TLS e controle de acesso). | Preservar privacidade e integridade das contas. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| RNF03 | Usabilidade (U) | O sistema deve ter fluxo simples para ações críticas (criar, buscar e aceitar carona em poucos passos). | Reduzir fricção de uso e tempo para completar tarefas. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/); [BlaBlaCar](https://www.blablacar.com.br/) |
| RNF04 | Confiabilidade (R) | O sistema deve registrar logs de ações relevantes (aceites, cancelamentos e denúncias). | Aumentar auditabilidade e suporte a incidentes. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| RNF06 | Performance (P) | O sistema deve apresentar rotas e estimativas de tempo de forma consistente. | Melhorar previsibilidade da experiência de deslocamento. | [Google Maps](https://www.google.com/maps)/[Waze](https://www.waze.com/) |

<font size="2"><p style="text-align: center">Fonte: [João Marcos](https://github.com/JJOAOMARCOSS), [Luiza da Silva](https://github.com/luizaxx) e [Wanjo Christopher](https://github.com/wChrstphr), 2026.</p></font>

</details>

---

## Conclusão

O benchmarking indicou que soluções bem-sucedidas combinam **facilidade de oferta/busca**, **comunicação direta**, **apoio por mapas** e mecanismos de **confiança** (reputação, denúncia e suporte). Para o CaronaAmiga FCTE, os principais aprendizados se concentram em adaptar essas práticas ao cenário universitário, com foco em comunidade restrita, rotas recorrentes e segurança.

---

## Referências Bibliográficas

> <a id="ref1">1.</a> IATA, Cristiane. Benchmarking: muito além de uma simples comparação. Revista Benchmarking, edição 1, dez. 2008. Disponível em: https://pontogp.wordpress.com/2008/12/24/benchmarking-muito-alem-de-uma-simples-comparacao. Acesso em: 6 abr. 2025.

> <a id="ref2">2.</a> BLABLACAR. *Página institucional*. Disponível em: https://www.blablacar.com.br/ride-sharing/services/como-funciona. Acesso em: 31 mar. 2026.

> <a id="ref3">3.</a> UBER. *Página institucional (Brasil)*. Disponível em: https://www.uber.com/br/pt-br/. Acesso em: 31 mar. 2026.

> <a id="ref4">4.</a> 99. *Página institucional*. Disponível em: https://99app.com/. Acesso em: 31 mar. 2026.

> <a id="ref5">5.</a> GOOGLE. *Google Maps*. Disponível em: https://www.google.com/maps. Acesso em: 31 mar. 2026.

> <a id="ref6">6.</a> WAZE. *Waze*. Disponível em: https://www.waze.com/pt-BR/. Acesso em: 31 mar. 2026.

> <a id="ref7">7.</a> WHATSAPP. *WhatsApp*. Disponível em: https://www.whatsapp.com/?lang=pt_BR. Acesso em: 31 mar. 2026.

> <a id="ref8">8.</a> TELEGRAM. *Telegram*. Disponível em: https://telegram.org/. Acesso em: 31 mar. 2026.

## Histórico de Versões

| Versão | Data | Descrição | Autor(es) | Revisor(es) | Detalhes da revisão |
| :----: | :--: | --------- | ----------- | ------ | :---: |
| 1.0  | 31/03/2026 | Criação do documento [#36](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/issues/36) | [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS), [Luiza da Silva](https://github.com/luizaxx) e [Wanjo Christopher](https://github.com/wChrstphr) | [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharess) | - |
| 1.1 | 02/04/2026 | Melhoria dos requisitos funcionais e não-funcionais extraídos no benchmarking | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS) | Artefato revisado |
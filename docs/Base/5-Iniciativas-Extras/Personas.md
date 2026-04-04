# Perfil de Usuário e Personas

## Introdução
Personas são modelos descritivos de usuários arquetípicos derivados de pesquisa com usuários, sintetizando várias pessoas reais em um modelo com metas, motivações e comportamentos compartilhados [[1]](#referências-bibliográficas). Geralmente, entre 1 a 7 personas são desenvolvidas para apoiar um projeto, baseando-se nas diferenças de metas e ações dos usuários em vez de focar apenas em segmentos demográficos [[1]](#referências-bibliográficas).

## Objetivo
Este artefato tem como propósito definir as características dos estudantes da UnB/FCTE, considerando a realidade socioeconômica de baixa e média renda. Para contextualizar o perfil desses jovens no Brasil e sua distribuição demográfica, utilizamos dados estatísticos oficiais [[2]](#referências-bibliográficas) e indicadores de educação e renda [[3]](#referências-bibliográficas). O objetivo final é extrair dados sobre comportamentos de mobilidade e barreiras psicológicas para humanizar o desenvolvimento da plataforma, permitindo que a equipe crie soluções que atendam às necessidades reais de transporte e segurança do campus.

## Metodologia
A elaboração das personas seguiu o processo de personas orientadas por dados (*data-driven*), que prioriza a validade empírica sobre suposições [[1]](#referências-bibliográficas). O processo seguiu estas diretrizes técnicas:
*   **Pesquisa Primária:** Coleta de dados com estudantes para entender hábitos de viagem e o uso de transporte público ou privado [[1]](#referências-bibliográficas).
*   **Fatores de Localização e Sistema:** Análise da densidade da área e da frequência do transporte, fatores que influenciam a propensão ao uso de caronas [[1]](#referências-bibliográficas).
*   **Extração de Factoids:** Identificação de pontos de dados cruciais para criar subcategorias de usuários baseadas em seus objetivos principais [[1]](#referências-bibliográficas).
*   **Desenvolvimento de Personas:** Refinamento de "esqueletos" de usuários em personas completas, com nomes, fotos e perfis comportamentais estáveis [[1]](#referências-bibliográficas).

## Participantes

<div style="text-align: center;">

<font size="3"><p>Tabela 1: Participantes</p></font>


| Aluno | Data | Hora |
| ---| ---| ---|
| [Wanjo Christopher P. Escobar](https://github.com/wChrstphr) | 31/03/2026 | 14:00 |
| [João Marcos M. de Andrade](https://github.com/JJOAOMARCOSS) | 31/03/2026 | 14:30 |

<font size="2"><p>Fonte: [João Marcos](https://github.com/JJOAOMARCOSS) e [Wanjo Christopher P. Escobar](https://github.com/wChrstphr), 2026.</p></font>

</div>


## Perfil de Usuário

### 1. Usuário

<div style="text-align: center;">

<font size="3"><p>Figura 1: Qual sua idade?</p></font>

![Qual sua idade?](../assets/questionario/0_idade.png)

<font size="3"><p>Figura 2: Com qual gênero você se identifica?</p></font>

![Com qual gênero você se identifica?](../assets/questionario/1_generos.png)

<font size="3"><p>Figura 3: Qual a sua situação ocupacional?</p></font>

![Qual a sua situação ocupacional?](../assets/questionario/2_ocupacao.png)

<font size="3"><p>Figura 4: Qual a renda média do seu grupo familiar?</p></font>

![Qual a renda média do seu grupo familiar?](../assets/questionario/3_renda-familiar.png)

<font size="3"><p>Figura 5: Você possui CNH ativa?</p></font>

![Você possui CNH ativa?](../assets/questionario/4_cnh-ativa.png)

<font size="3"><p>Figura 6: Você possui veículo próprio disponível para ir à faculdade?</p></font>

![Você possui veículo próprio disponível para ir à faculdade?](../assets/questionario/5_carro-proprio.png)

<font size="3"><p>Figura 7: Você estaria disposto a compartilhar carona com alguém que não conhece, desde que fosse estudante da UnB?</p></font>

![Você estaria disposto a compartilhar carona com alguém que não conhece, desde que fosse estudante da UnB?](../assets/questionario/6_disposto-dar-carona.png)

<font size="2"><p>Fonte: Questionário aplicado pela equipe do projeto, 2026.</p></font>

</div>

#### Requisitos Elicitados dessa parte

<details>
<summary>Requisitos Funcionais</summary>

<font size="3"><p style="text-align: center">Tabela 2: Requisitos Funcionais - Parte Usuário</p></font>

| Código | Requisito Funcional | Objetivo | Especificação |
| :--: | :-- | :-- | :-- |
| RFU01 | Coletar dados de perfil do usuário (faixa etária, gênero e situação ocupacional). | Caracterizar o público da plataforma e apoiar personalização inicial. | Cadastro e edição de perfil com campos estruturados. |
| RFU02 | Permitir informar disponibilidade de CNH ativa e veículo próprio. | Diferenciar potenciais motoristas e passageiros. | Campos específicos no perfil com atualização pelo usuário. |
| RFU03 | Permitir registrar a disposição para compartilhar carona com estudantes da UnB fora da rede de conhecidos. | Apoiar regras de pareamento e sugestões mais aderentes ao conforto do usuário. | Preferência de pareamento configurável em perfil. |

</details>

<details>
<summary>Requisitos Não Funcionais</summary>

<font size="3"><p style="text-align: center">Tabela 3: Requisitos Não Funcionais - Parte Usuário</p></font>

| Código | Requisito Não Funcional | Objetivo | Especificação |
| :--: | :-- | :-- | :-- |
| RNFU01 | Tratar dados pessoais de perfil com privacidade e segurança. | Evitar exposição indevida de informações pessoais. | Controle de acesso e proteção de dados cadastrais. |
| RNFU02 | Suportar opções de identificação de gênero sem ambiguidade de preenchimento. | Garantir inclusão e consistência dos dados de perfil. | Interface de cadastro clara e consistente para campos de identificação. |

</details>

### 2. Motivação
<div style="text-align: center;">
<font size="3"><p>Figura 8: O que te motivaria a usar um aplicativo de carona entre alunos?</p></font>


![O que te motivaria a usar um aplicativo de carona entre alunos?](../assets/questionario/7_motivacao-alunos.png)

<font size="3"><p>Figura 9: Em quais situações você usaria o app?</p></font>


![Em quais situações você usaria o app?](../assets/questionario/8_situacoes-de-uso.png)

<font size="3"><p>Figura 10: O quanto economizar dinheiro influenciaria sua decisão?</p></font>

![O quanto economizar dinheiro influenciaria sua decisão?](../assets/questionario/9_economizar-dinheiro.png)

<font size="3"><p>Figura 11: O quanto ganhar tempo influenciaria sua decisão?</p></font>

![O quanto ganhar tempo influenciaria sua decisão?](../assets/questionario/10_ganhar-tempo.png)

<font size="2"><p>Fonte: Questionário aplicado pela equipe do projeto, 2026.</p></font>

</div>

#### Requisitos Elicitados dessa parte

<details>
<summary>Requisitos Funcionais</summary>

<font size="3"><p style="text-align: center">Tabela 4: Requisitos Funcionais - Parte Motivação</p></font>

| Código | Requisito Funcional | Objetivo | Especificação |
| :--: | :-- | :-- | :-- |
| RFM01 | Permitir selecionar contexto de uso da carona (ida, volta, ida e volta, eventos/horários específicos). | Atender diferentes rotinas de deslocamento acadêmico. | Filtros de busca e oferta por contexto de uso. |
| RFM02 | Exibir informações de apoio à decisão relacionadas a economia e tempo. | Reforçar os principais motivadores identificados no questionário. | Exibição de estimativa de custo e duração no fluxo de carona. |

</details>

<details>
<summary>Requisitos Não Funcionais</summary>

<font size="3"><p style="text-align: center">Tabela 5: Requisitos Não Funcionais - Parte Motivação</p></font>

| Código | Requisito Não Funcional | Objetivo | Especificação |
| :--: | :-- | :-- | :-- |
| RNFM01 | Disponibilizar interface simples para consulta e solicitação de caronas. | Reduzir fricção de uso e favorecer adoção inicial. | Fluxos com baixa complexidade de navegação. |
| RNFM02 | Garantir desempenho adequado nas consultas de carona. | Preservar a percepção de ganho de tempo no uso da plataforma. | Respostas rápidas em busca e carregamento de resultados. |

</details>

### 3. Segurança

<font size="3"><p style="text-align: center">Figura 12: Quais itens aumentariam sua confiança?</p></font>

![Quais itens aumentariam sua confiança?](../assets/questionario/11_itens-confianca.png)

<font size="2"><p style="text-align: center">Fonte: Questionário aplicado pela equipe do projeto, 2026.</p></font>

#### Requisitos Elicitados dessa parte

<details>
<summary>Requisitos Funcionais</summary>

<font size="3"><p style="text-align: center">Tabela 6: Requisitos Funcionais - Parte Segurança</p></font>

| Código | Requisito Funcional | Objetivo | Especificação |
| :--: | :-- | :-- | :-- |
| RFS01 | Exibir perfil com foto dos usuários. | Aumentar confiança no processo de escolha de carona. | Perfil público com foto visível em oferta e solicitação. |
| RFS02 | Implementar verificação de vínculo institucional por matrícula da UnB. | Reforçar segurança e pertencimento ao contexto universitário. | Validação de identificação institucional no cadastro. |
| RFS03 | Permitir avaliações de usuários e visualização de histórico de viagens. | Apoiar decisão por reputação e experiência anterior. | Sistema de avaliações e histórico acessível no perfil. |
| RFS04 | Exibir informação de amigos em comum quando disponível. | Aumentar percepção de confiança na interação entre usuários. | Indicação de conexão social no perfil/fluxo de escolha. |

</details>

<details>
<summary>Requisitos Não Funcionais</summary>

<font size="3"><p style="text-align: center">Tabela 7: Requisitos Não Funcionais - Parte Segurança</p></font>

| Código | Requisito Não Funcional | Objetivo | Especificação |
| :--: | :-- | :-- | :-- |
| RNFS01 | Garantir integridade e confiabilidade das informações de perfil e avaliação. | Evitar manipulação indevida de sinais de confiança. | Controle de consistência para dados de reputação e verificação. |
| RNFS02 | Proteger dados sensíveis usados para validação institucional. | Preservar privacidade e segurança do usuário. | Tratamento seguro dos dados de identificação acadêmica. |

</details>

### 4. Funcionalidades Desejadas

<div style="text-align: center;">

<font size="3"><p>Figura 13: Quais funcionalidades você considera essenciais?</p></font>

![Quais funcionalidades você considera essenciais?](../assets/questionario/12_funcionaliades-essenciais.png)

<font size="3"><p>Figura 14: Você prefere caronas:</p></font>

![Você prefere caronas:](../assets/questionario/13_tipo-caronas.png)

<font size="3"><p>Figura 15: Você gostaria de definir preferências (ex: só motoristas/caronas mulheres)?</p></font>

![Você gostaria de definir preferências (ex: só motoristas/caronas mulheres)?](../assets/questionario/14_preferencias-caronas-mulheres.png)

<font size="2"><p>Fonte: Questionário aplicado pela equipe do projeto, 2026.</p></font>

</div>

#### Requisitos Elicitados dessa parte

<details>
<summary>Requisitos Funcionais</summary>

<font size="3"><p style="text-align: center">Tabela 8: Requisitos Funcionais - Parte Funcionalidades Desejadas</p></font>

| Código | Requisito Funcional | Objetivo | Especificação |
| :--: | :-- | :-- | :-- |
| RFF01 | Permitir agendamento de caronas. | Atender uso planejado e recorrente da comunidade acadêmica. | Publicação e reserva com data/horário futuro. |
| RFF02 | Disponibilizar divisão de custos da viagem. | Apoiar percepção de justiça e clareza no compartilhamento de despesas. | Campo de rateio no fluxo de criação/aceite da carona. |
| RFF03 | Disponibilizar rastreamento em tempo real da carona. | Melhorar previsibilidade e segurança durante o deslocamento. | Acompanhamento de status/localização durante a viagem. |
| RFF04 | Oferecer canal de chat entre os usuários da carona. | Melhorar comunicação antes e durante a viagem. | Mensageria no contexto da carona criada/aceita. |
| RFF05 | Incluir botão de emergência no contexto da viagem. | Apoiar resposta rápida em situações críticas. | Ação de emergência acessível durante carona em andamento. |
| RFF06 | Permitir configurar preferências de pareamento (ex.: apenas motoristas/caronas mulheres). | Aumentar sensação de conforto e adequação do pareamento. | Filtro de preferência no perfil e na busca de caronas. |
| RFF07 | Permitir escolha de escopo preferencial de caronas (mesmo curso, FCTE, UnB). | Ajustar o nível de proximidade social desejado pelo usuário. | Filtros de escopo na descoberta de caronas. |

</details>

<details>
<summary>Requisitos Não Funcionais</summary>

<font size="3"><p style="text-align: center">Tabela 9: Requisitos Não Funcionais - Parte Funcionalidades Desejadas</p></font>

| Código | Requisito Não Funcional | Objetivo | Especificação |
| :--: | :-- | :-- | :-- |
| RNFF01 | Manter disponibilidade elevada de recursos críticos (chat, rastreamento e emergência). | Evitar falhas em funcionalidades sensíveis à segurança e coordenação da carona. | Confiabilidade operacional durante todo o fluxo da viagem. |
| RNFF02 | Garantir usabilidade em dispositivos móveis para os fluxos principais. | Viabilizar uso cotidiano no contexto de deslocamento. | Interface responsiva e legível em telas móveis. |

</details>

### 5. Aspectos Sociais

<div style="text-align: center;">

<font size="3"><p>Figura 16: Você deixaria de usar o app por:</p></font>

![Você deixaria de usar o app por:](../assets/questionario/15_deixaria-de-usar-por.png)

<font size="3"><p>Figura 17: O que faria você baixar o app?</p></font>

![O que faria você baixar o app?](../assets/questionario/16_faria-usar.png)

<font size="3"><p>Figura 18: Você se sentiria mais confortável com</p></font>

![Você se sentiria mais confortável com](../assets/questionario/17_conforto.png)

<font size="2"><p>Fonte: Questionário aplicado pela equipe do projeto, 2026.</p></font>

</div>

#### Requisitos Elicitados dessa parte

<details>
<summary>Requisitos Funcionais</summary>

<font size="3"><p style="text-align: center">Tabela 10: Requisitos Funcionais - Parte Aspectos Sociais</p></font>

| Código | Requisito Funcional | Objetivo | Especificação |
| :--: | :-- | :-- | :-- |
| RFA01 | Permitir mecanismos sociais de adesão (ex.: indicação entre usuários). | Aumentar confiança inicial e estimular entrada de novos usuários. | Fluxo de convite/indicação integrado ao aplicativo. |
| RFA02 | Permitir configuração de preferências de conforto social no pareamento. | Reduzir barreiras de adesão associadas a desconforto social. | Opções de preferência no perfil e filtros de correspondência. |

</details>

<details>
<summary>Requisitos Não Funcionais</summary>

<font size="3"><p style="text-align: center">Tabela 11: Requisitos Não Funcionais - Parte Aspectos Sociais</p></font>

| Código | Requisito Não Funcional | Objetivo | Especificação |
| :--: | :-- | :-- | :-- |
| RNFA01 | Garantir estabilidade da aplicação para reduzir abandono por problemas de uso. | Diminuir desistência motivada por falhas percebidas no app. | Baixa incidência de erros nos fluxos essenciais. |
| RNFA02 | Sustentar experiência de uso confiável em cenários de baixa oferta de caronas. | Reduzir frustração associada à percepção de pouca disponibilidade. | Respostas claras do sistema quando não houver correspondências. |

</details>

### 6. Pagamento

<font size="3"><p style="text-align: center">Figura 19: O app sugerir preço automático é importante?</p></font>

![O app sugerir preço automático é importante?](../assets/questionario/18_sugerir_preco.png)

<font size="2"><p style="text-align: center">Fonte: Questionário aplicado pela equipe do projeto, 2026.</p></font>

#### Requisitos Elicitados dessa parte

<details>
<summary>Requisitos Funcionais</summary>

<font size="3"><p style="text-align: center">Tabela 12: Requisitos Funcionais - Parte Pagamento</p></font>

| Código | Requisito Funcional | Objetivo | Especificação |
| :--: | :-- | :-- | :-- |
| RFP01 | Sugerir automaticamente o preço da carona. | Apoiar definição de valor com menor esforço para os usuários. | Cálculo de valor sugerido no fluxo de criação da carona. |

</details>

<details>
<summary>Requisitos Não Funcionais</summary>

<font size="3"><p style="text-align: center">Tabela 13: Requisitos Não Funcionais - Parte Pagamento</p></font>

| Código | Requisito Não Funcional | Objetivo | Especificação |
| :--: | :-- | :-- | :-- |
| RNFP01 | Garantir transparência na apresentação do preço sugerido. | Evitar percepção de arbitrariedade no valor recomendado. | Critérios de cálculo exibidos de forma compreensível ao usuário. |

</details>

## Personas


## Gravação da reunião de Personas (Opcional)
[Inserir o embedded link para o YouTube do vídeo publicado.]

---

## Referências Bibliográficas

> <a id="REF1">1.</a> Marshall, R.; Cook, S.; Mitchell, V.; Summerskill, S.; Haines, V.; Maguire, M.; Sims, R.; Gyi, D.; Case, K. (2013) Design and evaluation: end users, user datasets and personas. Applied ergonomics. v. 46 Pt B. p. 311-317. doi: 10.1016/j.apergo.2013.03.008.

> <a id="REF2">2.</a> IBGE. Pirâmide Etária: Conheça o Brasil. Disponível em: [https://educa.ibge.gov.br/jovens/conheca-o-brasil/populacao/18318-piramide-etaria.html](https://educa.ibge.gov.br/jovens/conheca-o-brasil/populacao/18318-piramide-etaria.html). Acesso em: 28 mar. 2026.

> <a id="REF3">3.</a> IBGE. Indicadores Sociais Mínimos. Disponível em: [https://www.ibge.gov.br/estatisticas/sociais/educacao/17374-indicadores-sociais-minimos.html](https://www.ibge.gov.br/estatisticas/sociais/educacao/17374-indicadores-sociais-minimos.html). Acesso em: 28 mar. 2026.

## Histórico de Versões

| Versão | Data | Descrição | Autor(es) | Revisor(es) | Detalhes da revisão |
| :----: | :--: | --------- | ----------- | ------ | :---: |
| 1.0 | 28/03/2026 | Criação do documento | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS) | Aretefato Revisado |
| 1.1 | 31/03/2026 | Atualização de Objetivo e Metodologia com citações em ordem numérica de aparecimento | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS) | Reordenação das referências conforme o fluxo do texto. |
| 1.2 | 31/03/2026 | Arrumando os links |  [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS) | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | - |
| 1.3 | 04/04/2026 | Inclusão das categorias do questionário (0 a 18) com requisitos elicitados por parte | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS) | Estruturação por partes e tabelas RF/RNF |

# Protótipo 

Na fase de Prototipação do Design Sprint, as ideias e esboços validados anteriormente são materializados em um protótipo fiel o suficiente para ser testado, tirando a solução do papel e tornando-a física ou digital.

## Sobre o protótipo 

O protótipo de alta fidelidade, conforme apresentado no artigo [Prototipagem de alta fidelidade: o que é, quando, por que e como usar?](https://medium.com/somos-tera/prototipagem-de-alta-fidelidade-635d745b662b) [2](#ref1), corresponde a uma etapa essencial no processo de design centrado no usuário, uma vez que possibilita simular com grande precisão a experiência final do usuário com a plataforma.

Nesse contexto, esse tipo de protótipo busca representar de forma detalhada a interface, as interações e a navegação do produto, aproximando-se ao máximo da versão final. Por isso, ele se torna fundamental para validações mais realistas e para a condução de testes de usabilidade mais consistentes e aprofundados. [1](#ref1)

## Objetivos 

O desenvolvimento do protótipo de alta fidelidade tem como finalidade principal reproduzir com maior realismo a interface, as interações e a experiência de uso da plataforma Carona Amiga FTCE, permitindo uma percepção bastante próxima do produto final. A partir disso, pretende-se:

- Confirmar as escolhas de design orientadas ao usuário;
- Avaliar a fluidez da navegação;
- Assegurar a consistência visual e funcional das telas;
- Identificar e corrigir possíveis melhorias antes da etapa de desenvolvimento.

## Metodologia

O protótipo de alta fidelidade foi criado utilizando a plataforma [Figma](https://www.figma.com/), uma ferramenta bastante utilizada no desenvolvimento de interfaces e protótipos interativos. Sua construção seguiu os princípios do design centrado no usuário e foi baseada nas referências coletadas durante a etapa de [brainstorming](Base/2-Artefato-Generalista/Brainstorm.md), reuniões realizadas em conjunto com o grupo e nas fase de unpack, scketh e decison.

Com base nessas referências e nas ideias definidas durante a concepção do projeto, foram estabelecidos a estrutura visual, os padrões de navegação e a organização dos principais elementos que compõem a plataforma.

## Ferramentas Utilizadas

A construção do protótipo foi realizada utilizando a ferramenta:

 <img src="https://cdn-icons-png.flaticon.com/512/5968/5968705.png" alt="Logo do Figma" width="40"/> **Figma**: Ferramenta de design colaborativo, ideal para prototipação de interfaces com alta fidelidade, permitindo simulações de cliques, transições e navegação realista.  

## Protótipo de Alta Fidelidade

- **Tela de acesso** 
- **Tela de login - pedir carona** 
- **Tela de login - oferecer carona**
- **Menu lateral** 
- **Telas iniciais** 
- **Telas de carona**
- **Tela de mapas** 
- **Tela de aprovação**
- **Tela de favoritos**
- **Tela de load**
- **Tela de splash**

#### Tabela de Requisitos Funcionais (RF)

<font size="3"><p style="text-align: center">Tabela 1: Requisitos Funcionais</p></font>

| Código | Requisito Funcional | Objetivo | Rastreabilidade |
| :--: | :-- | :-- | :-- |
| <a id="rf01"></a>RF01 | Gerenciar perfil do usuário. | Aumentar confiança e personalização de uso. | [Benchmarking](../2-Artefato-Generalista/Benchmarking.md)|
| <a id="rf02"></a>RF02 | Criar oferta de carona. | Estruturar a oferta com informações mínimas para decisão. | [Benchmarking](../2-Artefato-Generalista/Benchmarking.md) |
| <a id="rf03"></a>RF03 | Buscar caronas. | Melhorar precisão no encontro entre oferta e demanda. |[Benchmarking](../2-Artefato-Generalista/Benchmarking.md) |
| <a id="rf05"></a>RF05 | Enviar mensagem. | Facilitar alinhamentos antes e durante a viagem. |[Benchmarking](../2-Artefato-Generalista/Benchmarking.md) |
| <a id="rf06"></a>RF06 | Solicitar participação. | Dar controle ao motorista e transparência ao passageiro. | [Benchmarking](../2-Artefato-Generalista/Benchmarking.md) |
| <a id="rf07"></a>RF07 | Cancelar solicitação. | Reduzir ruídos e melhorar rastreabilidade de ocorrências. | [Benchmarking](../2-Artefato-Generalista/Benchmarking.md)|
| <a id="rf08"></a>RF08 | Avaliar experiência. | Construir reputação e melhorar qualidade da comunidade. | [Benchmarking](../2-Artefato-Generalista/Benchmarking.md)|
| <a id="rf10"></a>RF10 | Enviar notificações. | Aumentar pontualidade e taxa de correspondência. |  [Benchmarking](../2-Artefato-Generalista/Benchmarking.md)|

#### Tabela de Especificações dos Requisitos Funcionais (ERF)

<font size="3"><p style="text-align: center">Tabela 2: Especificação dos Requisitos Funcionais</p></font>

| Código | Especificação | Objetivo |
| :--: | :-- | :-- |
| <a id="erf01"></a>[ERF01]([Benchmarking](../2-Artefato-Generalista/Benchmarking.md)) | Perfil com nome, curso/vínculo, foto obrigatória e preferências. | Melhorar identificação e confiança entre os usuários. |
| <a id="erf02"></a>[ERF02]([Benchmarking](../2-Artefato-Generalista/Benchmarking.md)) | Oferta de carona com origem, destino, horário, vagas e observações. | Padronizar publicação e facilitar decisão do passageiro. |
| <a id="erf03"></a>[ERF03]([Benchmarking](../2-Artefato-Generalista/Benchmarking.md)) | Busca com filtros por origem, destino, horário, recorrência e vagas. | Aumentar relevância dos resultados de carona. |
| <a id="erf05"></a>[ERF05]([Benchmarking](../2-Artefato-Generalista/Benchmarking.md)) | Chat habilitado após solicitação/aceite. | Viabilizar comunicação contextual da viagem. |
| <a id="erf05"></a>[ERF05.1]([Benchmarking](../2-Artefato-Generalista/Benchmarking.md)) | Disponibilizar chat entre motorista e passageiro. | Viabilizar comunicação rápida entre partes. |
| <a id="erf06"></a>[ERF06]([Benchmarking](../2-Artefato-Generalista/Benchmarking.md)) | Solicitação de vaga com fluxo de aceite/recusa pelo motorista. | Garantir controle de lotação e segurança de embarque. |
| <a id="erf07"></a>[ERF07]([Benchmarking](../2-Artefato-Generalista/Benchmarking.md)) | Cancelamento com motivo e aviso automático às partes envolvidas. | Minimizar conflitos e manter histórico de eventos. |
| <a id="erf10"></a>[ERF10]([Benchmarking](../2-Artefato-Generalista/Benchmarking.md)) | Notificações para match, aceite, alteração de horário e lembrete. | Aumentar engajamento e previsibilidade operacional. |



## Funcionalidades Simuladas

Para uma experiência mais realista, o protótipo simula interações como:

- Cliques nos menus e cards;
- Feedback visual individual para ações do usuário;
- Estrutura de comentários no chat (não funcional, mas visualmente representada);
- Mudança de páginas.


<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://embed.figma.com/proto/ujPAQzypxGliC9h0f9o8dl/Carona-Amiga---FCTE?node-id=72-1423&p=f&scaling=scale-down&content-scaling=fixed&page-id=72%3A1405&starting-point-node-id=72%3A1413&embed-host=share" allowfullscreen></iframe>

##  Explicação do Protótipo

Para a apresentação e validação do protótipo de alta fidelidade do projeto, optou-se pela gravação de um vídeo demonstrativo, com o objetivo de tornar a comunicação das ideias mais clara, dinâmica e envolvente. 

Por meio desse recurso, é possível percorrer a interface enquanto são explicadas, em tempo real, as decisões relacionadas ao design, à usabilidade e à acessibilidade que nortearam o desenvolvimento da plataforma.

Dessa forma, o vídeo permite evidenciar com maior precisão as funcionalidades interativas do protótipo, como menus, fluxos de navegação, transições entre telas e simulações do uso por parte dos usuários.

<iframe width="1321" height="743" src="" title="Validação e Explicação do protótipo" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Referência bibliográfica

> <a name="ref1"></a> [1] ROSA, Ângela. Protótipo: entenda o que é, tipos, exemplos e como fazer na prática! SoftDesign, 20 dez. 2024. Disponível em: https://softdesign.com.br/blog/prototipo-baixa-e-alta-fidelidade/#O-que-e-um-prototipo-nbsp. Acesso em: 02 abr. 2026.


> <a name="ref2"></a> [2] TERA. Prototipagem de alta fidelidade: o que é, quando, por que e como usar? Medium, 23 mar. 2020. Disponível em: https://medium.com/somos-tera/prototipagem-de-alta-fidelidade-635d745b662b. Acesso em: 02 abr. 2026.

> <a name="ref2"></a> [3] [Repositório Galáxia Conectada 2025.1](https://unbarqdsw2025-1-turma02.github.io/2025.1-T02-_G9_GalaxiaConectada_Entrega01/#/Base/DesignSprint/Prototipo?id=prot%c3%b3tipo-de-alta-fidelidade). Acesso em: 02 abr. 2026

## Histórico de versão 

| Versão | Data | Descrição | Autor(es) | Revisor(es) | Detalhes da revisão |
| :----: | :--: | --------- | ----------- | ------ | :---: |
| 1.0  | 02/04/2026 | Criação do documento [#20](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/issues/20) | [Luiza da S. Pugas](https://github.com/Luizaxx) | [Ana Victória Guedes da Costa](https://github.com/navicg)  | - |
| 1.1  | 02/04/2026 | Criação do protótipo  | [Ana Victória Guedes da Costa](https://github.com/navicg), [Gabriel Henrique Rodrigues de Lima](https://github.com/gabrielhrlima),[Gustavo Ribeiro Linhares](https://github.com/GustavoLinharess), [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS), [João Vitor Santos de Oliveira](https://github.com/Jauzimm),[Karoline Luz da Conceição](https://github.com/KarolineLuz), [Luiza da Silva Pugas](https://github.com/Luizaxx), [Nicolas Bomfim Dias Bandeira](https://github.com/NickGehjk),[Pedro Henrique Faria da Mota](https://github.com/PhFariaa), [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr), | [Ana Victória Guedes da Costa](https://github.com/navicg)  | - |


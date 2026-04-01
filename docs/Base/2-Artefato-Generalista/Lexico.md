# Léxico

## Introdução

O Léxico Ampliado da Linguagem (LAL) é uma técnica de Engenharia de Requisitos voltada para identificar e descrever termos peculiares ao domínio do problema. Essa abordagem busca reduzir ambiguidades de comunicação e alinhar o entendimento entre as partes interessadas por meio da definição de símbolos do contexto da aplicação.

No LAL, cada símbolo é descrito por dois elementos centrais: **Noção** (o que o termo significa no domínio) e **Impacto** (como o termo é usado, quais efeitos provoca ou sofre na aplicação). Assim, o artefato contribui para consolidar uma linguagem comum da equipe e apoiar etapas posteriores de modelagem e decisão.
<a href="#/Base/2-Artefato-Generalista/Lexico?id=referencias-bibliograficas">[1]</a>

## Metodologia

A construção do Léxico foi realizada utilizando o Brainstorm e o Rich Picture construídos nas etapas de `Unpack` e `Sketch`, por meio de discussão orientada ao domínio da solução Carona Amiga FCTE. O processo foi estruturado nas seguintes etapas:

1. Levantamento inicial de termos recorrentes no contexto do projeto (atores, objetos, ações e estados).
2. Classificação dos termos por tipo de símbolo do LAL: **Verbo**, **Objeto** e **Estado**.
3. Definição da **Noção** de cada símbolo, descrevendo significado e contexto de ocorrência.
4. Definição do **Impacto** de cada símbolo, registrando efeitos, usos e desdobramentos no sistema.
5. Revisão coletiva para remover ambiguidades, consolidar sinônimos e padronizar nomenclatura.

Regras gerais aplicadas no artefato:

- Cada símbolo pode possuir zero ou mais sinônimos.
- Cada símbolo deve possuir uma ou mais noções.
- Cada símbolo deve possuir um ou mais impactos.

Critérios de descrição por tipo:

| Tipo <<sujeito>> | Noção <<Quem é o sujeito?>> | Impacto <<Quais ações executa?>> |
| :-- | :-- | :-- |
| VERBO | Quem realiza, quando acontece e quais os procedimentos envolvidos. | Quais os reflexos da ação no ambiente e quais novos estados decorrem dela. |
| OBJETO | Definição do objeto e identificação de outros objetos com os quais se relaciona. | Ações que podem ser aplicadas ao objeto. |
| ESTADO | Significado do estado e quais ações levaram a esse estado. | Identificação de outros estados e ações que podem ocorrer a partir dele. |

## Participantes

<font size="3"><p style="text-align: center">Tabela 1: Participantes</p></font>

<div style="text-align: center;">

| Aluno | Função | Data | Hora |
| :--: | :--: | :--: | :--: |
| [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | Elaboração do artefato Léxico | 31/03/2026 | 20:00 |
[Pedro Henrique Faria da Mota](https://github.com/phfariaa) | Elaboração do artefatos Léxico | 01/04/2026 | 16:00  

</div>

<font size="2"><p style="text-align: center">Fonte: [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) , 2026.</p></font>


## Léxico do Projeto

<a id="termo-motorista"></a>
### Termo: Motorista

| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Objeto | - Estudante da FCTE que oferece [caronas](#termo-carona) na plataforma.<br>- Responsável por informar rota, horário, número de vagas no carro e combinar o valor da corrida com os [caronas](#termo-carona). | - Realiza as tarefas: [criar carona](#termo-criar-carona), [fechar carona](#termo-fechar-carona), [editar carona](#termo-editar-carona), [aceitar solicitacao de carona](#termo-aceitar-solicitacao-de-carona), [concluir carona](#termo-concluir-carona) e [editar perfil](#termo-editar-perfil). |

<a id="termo-passageiro"></a>
### Termo: Passageiro
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Objeto | - Estudante da FCTE que busca [caronas](#termo-carona) disponiveis para seu trajeto.<br>- Responsavel pelo envio de [solicitacao de carona](#termo-solicitar-carona) ao [motorista](#termo-motorista), com base em origem, destino, horario e disponibilidade. Tambem deve combinar os valores com o [motorista](#termo-motorista). | - Realiza as tarefas: [solicitar carona](#termo-solicitar-carona), [editar perfil](#termo-editar-perfil), [cancelar carona](#termo-cancelar-carona) e [avaliar motorista](#termo-avaliar-motorista). |


<a id="termo-carona"></a>
### Termo: Carona
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Objeto |- Deslocamento compartilhado entre [motorista](#termo-motorista) e um ou mais [passageiros](#termo-passageiro).<br> - Possui origem, destino, horário, vagas e status associados. | - Pode ser consultada, [solicitada](#termo-solicitar-carona) e [cancelada pelo passageiro](#termo-cancelar-carona).<br> - Pode ser [criada](#termo-criar-carona), [modificada](#termo-editar-carona), excluída, confirmada, iniciada, [finalizada](#termo-concluir-carona) ou [cancelada pelo motorista](#termo-fechar-carona). |

<a id="termo-criar-carona"></a>
### Termo: Criar carona
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Verbo | - Tarefa realizada pelo [motorista](#termo-motorista).<br>- Acontece quando o [motorista](#termo-motorista) se disponibiliza a dar uma [carona](#termo-carona) e segue o fluxo de criacao de vagas no aplicativo informando aos [passageiros](#termo-passageiro) o destino e caminho. | - O [motorista](#termo-motorista) cria a [carona](#termo-carona).<br>- A [carona](#termo-carona) fica disponivel para consulta.<br>- As vagas da [carona](#termo-carona) ficam disponiveis para os [passageiros](#termo-passageiro) enviarem solicitacoes.<br>- O sistema registra a disponibilidade de vagas. |

<a id="termo-concluir-carona"></a>
### Termo: Concluir carona
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Verbo | - Tarefa realizada pelo [motorista](#termo-motorista).<br>- Acontece quando o [motorista](#termo-motorista) deixa o(s) [passageiro(s)](#termo-passageiro) no destino, avalia de 1 a 5 estrelas cada [passageiro](#termo-passageiro) e conclui a [carona](#termo-carona) no aplicativo. | - O [motorista](#termo-motorista) conclui a [carona](#termo-carona).<br>- A [carona](#termo-carona) deixa de aceitar interacoes.<br>- O sistema registra a conclusao da viagem.<br>- [Passageiros](#termo-passageiro) podem [avaliar motorista](#termo-avaliar-motorista).<br>- O [passageiro](#termo-passageiro) nao tem mais interacao direta com a [carona](#termo-carona). |

<a id="termo-editar-carona"></a>
### Termo: Editar carona
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Verbo | - Tarefa realizada pelo [motorista](#termo-motorista).<br>- Acontece quando o [motorista](#termo-motorista) precisa mudar rota, horario ou a quantidade de vagas da [carona](#termo-carona). | - O [motorista](#termo-motorista) edita a [carona](#termo-carona).<br>- As informacoes da [carona](#termo-carona) sao atualizadas no sistema.<br>- [Passageiros](#termo-passageiro) associados sao notificados sobre alteracoes relevantes.<br>- Novas condicoes podem afetar solicitacoes existentes. |

<a id="termo-solicitar-carona"></a>
### Termo: Solicitar carona
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Verbo | - Tarefa realizada pelo [passageiro](#termo-passageiro).<br>- Acontece quando o [passageiro](#termo-passageiro) ve uma [carona](#termo-carona) com vagas disponiveis e se candidata para preencher uma vaga. | - O [passageiro](#termo-passageiro) solicita [carona](#termo-carona).<br>- Uma solicitacao de participacao e registrada para a [carona](#termo-carona).<br>- O [motorista](#termo-motorista) pode avaliar e decidir sobre a solicitacao.<br>- A vaga permanece reservada ate decisao do [motorista](#termo-motorista). |

<a id="termo-editar-perfil"></a>
### Termo: Editar perfil
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Verbo | - Tarefa realizada pelo [passageiro](#termo-passageiro) e pelo [motorista](#termo-motorista).<br>- Acontece quando o [passageiro](#termo-passageiro) ou [motorista](#termo-motorista) precisa atualizar dados pessoais e preferencias de uso no aplicativo. | - O [passageiro](#termo-passageiro)/[motorista](#termo-motorista) edita o perfil.<br>- As informacoes cadastrais ficam atualizadas no sistema.<br>- Os dados podem influenciar combinacao de [carona](#termo-carona) e contato entre [passageiros](#termo-passageiro) e [motoristas](#termo-motorista). |

<a id="termo-cancelar-carona"></a>
### Termo: Cancelar carona
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Verbo | - Tarefa realizada pelo [passageiro](#termo-passageiro) ao desistir de uma participacao em [carona](#termo-carona).<br>- Acontece antes do inicio da viagem ou quando o [passageiro](#termo-passageiro) nao pode comparecer. | - A solicitacao ou participacao em [carona](#termo-carona) e cancelada.<br>- A vaga volta a ficar disponivel para outros [passageiros](#termo-passageiro).<br>- O [motorista](#termo-motorista) e notificado sobre o cancelamento. |

<a id="termo-avaliar-motorista"></a>
### Termo: Avaliar motorista
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Verbo | - Tarefa realizada pelo [passageiro](#termo-passageiro) ao final da viagem.<br>- Acontece apos a [carona concluida](#termo-carona-concluida), registrando uma nota e comentario sobre a experiencia. | - A avaliacao do [motorista](#termo-motorista) e registrada no sistema.<br>- O historico de reputacao do [motorista](#termo-motorista) e atualizado.<br>- A avaliacao apoia a tomada de decisao de futuros [passageiros](#termo-passageiro). |


<a id="termo-aceitar-solicitacao-de-carona"></a>
### Termo: Aceitar solicitação de carona
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Verbo | - Tarefa realizada pelo [motorista](#termo-motorista).<br>- Acontece quando o [motorista](#termo-motorista) recebe uma solicitacao de [carona](#termo-carona) de um [passageiro](#termo-passageiro) e decide aceitar ou nao. | - O [motorista](#termo-motorista) aceita a solicitacao de [carona](#termo-carona) do [passageiro](#termo-passageiro).<br>- O [passageiro](#termo-passageiro) passa a ocupar uma vaga na [carona](#termo-carona).<br>- O numero de vagas da [carona](#termo-carona) disponiveis e atualizado.<br>- O [passageiro](#termo-passageiro) e notificado da decisao. |

<a id="termo-fechar-carona"></a>
### Termo: Fechar carona
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Verbo | - Tarefa realizada pelo [motorista](#termo-motorista) ou pelo sistema de forma automatica.<br>- Acontece quando o [motorista](#termo-motorista) decide fechar a [carona](#termo-carona) para novas vagas, mesmo sem preenchimento total.<br>- Tambem acontece quando o numero maximo de vagas da [carona](#termo-carona) e preenchido. | - O [motorista](#termo-motorista) ou o sistema fecham a [carona](#termo-carona).<br>- A [carona](#termo-carona) deixa de aceitar novas solicitacoes.<br>- [Passageiros](#termo-passageiro) ainda podem participar caso ja tenham sido aceitos.<br>- O sistema impede novas solicitacoes ou reservas de vagas. |

<a id="termo-carona-aberta"></a>
### Termo: Carona aberta
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Estado | - Estado da [carona](#termo-carona) em que ainda existem vagas disponiveis.<br>- Permite que [passageiros](#termo-passageiro) visualizem e solicitem participacao. | - A [carona](#termo-carona) esta aberta.<br>- [Passageiros](#termo-passageiro) podem enviar [solicitacoes](#termo-solicitar-carona).<br>- O [motorista](#termo-motorista) pode [editar carona](#termo-editar-carona) ou [fechar carona](#termo-fechar-carona).<br>- O sistema mantem controle das vagas disponiveis. |

<a id="termo-carona-fechada"></a>
### Termo: Carona fechada
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Estado | - Estado da [carona](#termo-carona) em que nao sao aceitas novas solicitacoes.<br>- Pode ocorrer por decisao do [motorista](#termo-motorista) ou por preenchimento total das vagas. | - A [carona](#termo-carona) esta fechada.<br>- [Passageiros](#termo-passageiro) nao podem mais [solicitar carona](#termo-solicitar-carona).<br>- O [motorista](#termo-motorista) pode iniciar ou [cancelar carona](#termo-cancelar-carona).<br>- O sistema bloqueia novas reservas de vagas. |

<a id="termo-carona-em-andamento"></a>
### Termo: Carona em andamento
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Estado | - Estado da [carona](#termo-carona) em que o trajeto ja foi iniciado pelo [motorista](#termo-motorista) com os [passageiros](#termo-passageiro). | - A [carona](#termo-carona) esta em andamento.<br>- Nao e possivel adicionar ou remover [passageiros](#termo-passageiro).<br>- O [motorista](#termo-motorista) nao pode mais [editar carona](#termo-editar-carona).<br>- O sistema registra o progresso da viagem. |

<a id="termo-carona-concluida"></a>
### Termo: Carona concluída
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Estado | - Estado da [carona](#termo-carona) apos a finalizacao do trajeto e chegada ao destino. | - A [carona](#termo-carona) foi concluida.<br>- Nenhuma acao operacional pode ser realizada na [carona](#termo-carona).<br>- O sistema registra o historico da viagem.<br>- Os participantes podem visualizar os dados da [carona concluida](#termo-carona-concluida). |


## Referências Bibliográficas

> <a id="referencias-bibliograficas">1.</a> LAL - Léxico Ampliado da Linguagem. Material de apoio da disciplina de Engenharia de Requisitos. Acesso em: 31 mar. 2026.

> <a id="REF2">2.</a> Brainstorm. Disponível em: [https://unbarqdsw2024-2.github.io/2024.2_G5_Turismo_Entrega_01/#/Base/Brainstorm?id=metodologia](https://unbarqdsw2024-2.github.io/2024.2_G5_Turismo_Entrega_01/#/Base/Brainstorm?id=metodologia). Acesso em: 31 mar. 2026.

## Histórico de Versões

| Versão | Data | Descrição | Autor(es) | Revisor(es) | Detalhes da revisão |
| :----: | :--: | --------- | ----------- | ------ | :---: |
| 1.0  | 31/03/2026 | Criação do documento do artefato Léxico [#34](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/issues/34) | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS) | Documento revisado |
| 1.1 | 01/04/2026 | Alterando documentação do artefato Léxico [#34](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/issues/34) | [Pedro Henrique Faria da Mota](https://github.com/phfariaa) |[Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr)  | Artefato revisado |
| 1.2  | 01/03/2026 | Complementação do artefato Léxico, inclusão de terminologias do passageiro e adição de rastreabilidade cruzada entre termos [#34](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/issues/34) | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | [Pedro Henrique Faria da Mota](https://github.com/phfariaa)| - |

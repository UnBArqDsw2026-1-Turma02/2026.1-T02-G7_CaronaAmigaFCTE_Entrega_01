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

### Termo: Motorista [1]

| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Objeto | - Estudante da FCTE que oferece caronas na plataforma.<br>- Responsável por informar rota, horário, número de vagas no carro e combinar o valor da corrida com os caronas. | - Realiza as tarefas: criar carona, fechar carona, editar carona, aceitar solicitação de carona. |

### Termo: Passageiro [2]
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Objeto | - Estudante da FCTE que busca caronas disponíveis para seu trajeto.<br>- Responsável pelo envio de solicitação de carona ao motorista [1], com base em origem, destino, horário e disponibilidade. Também deve combinar os valores com o motorista. | - Realiza as tarefas: solicitar carona, editar perfil |


### Termo: Carona [3]
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Objeto |- Deslocamento compartilhado entre motorista e um ou mais passageiros.<br> - Possui origem, destino, horário, vagas e status associados. | - Pode ser consultada, solicitada e cancelada pelo passageiro.<br> - Pode ser criada, modificada, excluída, confirmada, iniciada, finalizada ou cancelada pelo motorista. |

### Termo: Criar carona [4]
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Verbo | - Tarefa realizada pelo motorista. [1] <br> - Acontece quando o motorista [1] se disponibiliza a dar uma carona [3] e segue o fluxo de criação de vagas no aplicativo informando aos passageiros [2] o destino e caminho. | - O motorista cria a carona. <br>- A carona [3] está disponível para consulta. <br> - As vagas estão disponíveis para os passageiros enviarem solicitações. <br> - O sistema registra a disponibilidade de vagas.

### Termo: Concluir carona [5]
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Verbo | - Tarefa realizada pelo motorista. [1] <br> - Acontece quando o motorista [1] deixa o(s) passageiro(s) [2] no destino, avalia de 1 a 5 estrelas cada passageiro e conclui a carona no aplicativo. <br>  | - O motorista conclui a carona. <br>- A carona [3] deixa de aceitar interações. <br> - O sistema registra a conclusão da viagem. <br> - Passageiros [2] podem avaliar o motorista[1] <br> - Passageiro [2] não tem mais interação com a carona diretamente.

### Termo: Editar carona [6]
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Verbo | - Tarefa realizada pelo motorista. [1] <br> - Acontece quando o motorista [1] precisa mudar a rota,<br> horário ou a quantidade de vagas da carona. | - O motorista edita a carona. <br>- As informações da carona [3] são atualizadas no sistema. <br> - Passageiros [2] associados são notificados sobre alterações relevantes. <br> - Novas condições podem afetar solicitações existentes.

### Termo: Solicitar carona [7]
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Verbo | - Tarefa realizada pelo [passageiro](2). <br> - Acontece quando o passageiro vê uma [carona criada](4) com <br> vagas disponíveis e se candidata para preencher uma vaga. | - O passageiro solicita carona. <br>- Uma solicitação de participação é registrada para a carona [3]. <br> - O motorista [1] pode avaliar e decidir sobre a solicitação do passageiro . <br> - A vaga permanece reservada até decisão do motorista.


### Termo: Aceitar solicitação de Carona [8]
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Verbo | - Tarefa realizada pelo motorista [1]. <br> - Acontece quando o motorista [1] recebe uma solicitação de carona [3] <br> de um passageiro [2] e decide se quer aceitar ou não. | -O motorista aceita a solicitação de carona do passageiro. <br> - O passageiro [2] passa a ocupar uma vaga na carona [3]. <br>- O número de vagas disponíveis é atualizado. <br> - O passageiro [2] é notificado da decisão.

### Termo: Fechar carona [9]
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Verbo | - Tarefa realizada pelo motorista ou pelo sistema de forma automática[1]. <br>- Acontece quando o motorista [1] tem o desejo de fechar a carona [3] <br> para novas vagas mesmo que não estejam todas preenchidas.<br> - Acontece quando o número máximo de vagas da carona [3] foi preenchido. | - O motorista ou o sistema fecham a carona. [3]<br>- A carona [3] deixa de aceitar novas solicitações. <br> - Passageiros [2] ainda podem participar caso já tenham sido aceitos. <br> - O sistema impede novas solicitações ou reservas de vagas.

### Termo: Carona aberta [10]
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Estado | - Estado da carona [3] em que ainda existem vagas disponíveis.<br>- Permite que passageiros [2] visualizem e solicitem participação. | - A carona está aberta. <br> - Passageiros [2] podem enviar solicitações.<br>- O motorista [1] pode editar ou fechar a carona.<br>- O sistema mantém controle das vagas disponíveis. |

### Termo: Carona fechada [11]
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Estado | - Estado da carona [3] em que não são aceitas novas solicitações.<br>- Pode ocorrer por decisão do motorista [1] ou por preenchimento total das vagas. | - A carona está fechada. <br>- Passageiros [2] não podem mais solicitar participação.<br>- O motorista [1] pode iniciar ou cancelar a carona.<br>- O sistema bloqueia novas reservas de vagas. |

### Termo: Carona em andamento [12]
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Estado | - Estado da carona [3] em que o trajeto já foi iniciado pelo motorista [1] com os passageiros [2]. | - A carona está em andamento.<br>- Não é possível adicionar ou remover passageiros.<br>- O motorista [1] não pode mais editar informações da carona.<br>- O sistema registra o progresso da viagem. |

### Termo: Carona concluída [13]
| Tipo | Noção | Impacto |
| :--: | :--: | :--: |
| Estado | - Estado da carona [3] após a finalização do trajeto e chegada ao destino. | - A carona foi concluída.<br>- Nenhuma ação operacional pode ser realizada na carona.<br>- O sistema registra o histórico da viagem.<br>- Os participantes podem visualizar os dados da carona concluída. |


## Gravação da reunião de Léxico (Opcional)

Não houve gravação da reunião de elaboração deste artefato.

## Referências Bibliográficas

> <a id="referencias-bibliograficas">1.</a> LAL - Léxico Ampliado da Linguagem. Material de apoio da disciplina de Engenharia de Requisitos. Acesso em: 31 mar. 2026.

> <a id="REF2">2.</a> Brainstorm. Disponível em: [https://unbarqdsw2024-2.github.io/2024.2_G5_Turismo_Entrega_01/#/Base/Brainstorm?id=metodologia](https://unbarqdsw2024-2.github.io/2024.2_G5_Turismo_Entrega_01/#/Base/Brainstorm?id=metodologia). Acesso em: 31 mar. 2026.

## Histórico de Versões

| Versão | Data | Descrição | Autor(es) | Revisor(es) | Detalhes da revisão |
| :----: | :--: | --------- | ----------- | ------ | :---: |
| 1.0  | 31/03/2026 | Criação do documento do artefato Léxico [#34](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/issues/34) | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS) | Documento revisado |
| 1.1 | 01/04/2026 | Alterando documentação do artefato Léxico [#34](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/issues/34) | [Pedro Henrique Faria da Mota](https://github.com/phfariaa) |[Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr)  | Artefato revisado |
| 1.2  | 01/03/2026 | Complementação do artefato Léxico [#34](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/issues/34) | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | [Pedro Henrique Faria da Mota](https://github.com/phfariaa)| - |

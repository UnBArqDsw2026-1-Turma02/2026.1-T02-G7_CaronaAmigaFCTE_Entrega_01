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

</div>

<font size="2"><p style="text-align: center">Fonte: [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr)   , 2026.</p></font>


## Léxico do Projeto

### Termo: Motorista [1]
- **Tipo**: Objeto
- **Noção**:
	- Estudante da FCTE que oferece caronas na plataforma.
	- Responsável por informar rota, horário, número de vagas no carro e combinar o valor da corrida com os caronas.
- **Impacto**:
	- Realiza as tarefas: criar carona, fechar carona, editar carona, aceitar solicitação de carona.

### Termo: Passageiro [2]
- **Tipo**: Objeto
- **Noção**:
	- Estudante da FCTE que busca caronas disponíveis para seu trajeto.
	- Responsável pelo envio de solicitação de carona ao motorista [1], com base em origem, destino, horário e disponibilidade. Também deve combinar os valores com o motorista.
- **Impacto**:
	- Realiza as tarefas: solicitar carona, editar perfil

### Termo: Carona
- **Tipo**: Objeto
- **Noção**:
	- Deslocamento compartilhado entre motorista e um ou mais passageiros.
	- Possui origem, destino, horário, vagas e status associados.
- **Impacto**:
    - Pode ser consultada, solicitada e cancelada pelo passageiro.
    - Pode ser criada, modificada, excluída, confirmada, iniciada, finalizada ou cancelada pelo motorista.

### Termo: Criar Carona

### Termo: Fechar Carona

### Termo: Editar Carona

### Termo: Aceitar Solicitação de Carona

## Gravação da reunião de Léxico (Opcional)

Não houve gravação da reunião de elaboração deste artefato.

## Referências Bibliográficas

> <a id="referencias-bibliograficas">1.</a> LAL - Léxico Ampliado da Linguagem. Material de apoio da disciplina de Engenharia de Requisitos. Acesso em: 31 mar. 2026.

> <a id="REF2">2.</a> Brainstorm. Disponível em: [https://unbarqdsw2024-2.github.io/2024.2_G5_Turismo_Entrega_01/#/Base/Brainstorm?id=metodologia](https://unbarqdsw2024-2.github.io/2024.2_G5_Turismo_Entrega_01/#/Base/Brainstorm?id=metodologia). Acesso em: 31 mar. 2026.

## Histórico de Versões

| Versão | Data | Descrição | Autor(es) | Revisor(es) | Detalhes da revisão |
| :----: | :--: | --------- | ----------- | ------ | :---: |
| 1.0  | 31/03/2026 | Criação do documento de Léxico [#34](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/issues/34) | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS) | - |
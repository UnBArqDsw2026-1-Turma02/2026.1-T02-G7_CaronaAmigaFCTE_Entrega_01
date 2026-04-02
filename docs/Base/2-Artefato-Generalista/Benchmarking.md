# Benchmarking

## Introdução

O **benchmarking** é uma prática de análise comparativa usada para observar soluções existentes (produtos, serviços e processos), identificar abordagens consolidadas e extrair aprendizados que possam ser **adaptados** ao contexto de um novo projeto. Mais do que “copiar”, a proposta é entender *o que funciona*, *por que funciona* e *em quais condições*, para então tomar decisões de design e requisitos com menos incerteza [[1]](#referências-bibliográficas).

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

## Requisitos elicitados

### Requisitos Funcionais (RF)

<font size="3"><p style="text-align: center">Tabela 3: Requisitos Funcionais</p></font>

| Código | Requisito Funcional | Rastreabilidade |
| :--: | -- | -- |
| RF01 | Cadastrar usuário e gerenciamento de perfil do usuário (nome, curso/vínculo, foto obrigatória, preferências). | [BlaBlaCar](https://www.blablacar.com.br/); [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| Especificação RF01 | Com gerenciamento de perfil do usuário (nome, curso/vínculo, foto obrigatória, preferências). | [BlaBlaCar](https://www.blablacar.com.br/); [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| RF02 | Criar caronaPermitir criação de oferta de carona com origem, destino, horário, vagas e observações. | [BlaBlaCar](https://www.blablacar.com.br/) |
| Especificação RF02 | Criação de oferta de carona com origem, destino, horário, vagas e observações. | [BlaBlaCar](https://www.blablacar.com.br/) |
| RF03 | Buscar caronasPermitir busca de caronas com filtros (origem/destino, horário, recorrência, vagas). | [BlaBlaCar](https://www.blablacar.com.br/) |
| Especificação RF03 | Busca de caronas com filtros (origem/destino, horário, recorrência, vagas). | [BlaBlaCar](https://www.blablacar.com.br/) |
| RF04 | Exibir rota. | [Google Maps](https://www.google.com/maps)/[Waze](https://www.waze.com/); [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| Especificação RF04 | No mapa com tempo estimado e alternativa de ponto de encontro. | [Google Maps](https://www.google.com/maps)/[Waze](https://www.waze.com/); [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| RF05 | Enviar mensagemDisponibilizar chat entre motorista e passageiro após solicitação/aceite. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/); [WhatsApp](https://www.whatsapp.com/?lang=pt_BR) |
| Especificação RF05 | Disponibilizar chat entre motorista e passageiro após solicitação/aceite. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/); [WhatsApp](https://www.whatsapp.com/?lang=pt_BR) |
| RF06 | Solicitar participação. | [BlaBlaCar](https://www.blablacar.com.br/) |
| Especificação RF06 | Permitir solicitar participação em uma carona e permitir aceite/recusa pelo motorista. | [BlaBlaCar](https://www.blablacar.com.br/) |
| RF07 | Cancelar carona. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/); [BlaBlaCar](https://www.blablacar.com.br/) |
| Especificação RF07 | Permitir cancelamento com registro de motivo e notificação às partes. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/); [BlaBlaCar](https://www.blablacar.com.br/) |
| RF08 | Avaliar corrida. | [BlaBlaCar](https://www.blablacar.com.br/); [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| Especificação RF08 | Implementar sistema de avaliação pós-corrida/caronas (nota e comentário opcional). | [BlaBlaCar](https://www.blablacar.com.br/); [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| RF09 | Fazer denúnciaPermitir denúncia/bloqueio de usuário e canal de suporte. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| Especificação RF09 | De usuário, seja motorista ou passageiro. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| RF11 | Bloquear usuário | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| RF10 | Enviar notificações (match, aceite, alteração de horário, lembrete). | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/); [WhatsApp](https://www.whatsapp.com/?lang=pt_BR) |
| Especificação RF10 | (match, aceite, alteração de horário, lembrete). | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/); [WhatsApp](https://www.whatsapp.com/?lang=pt_BR) |

<font size="2"><p style="text-align: center">Fonte: [João Marcos](https://github.com/JJOAOMARCOSS), [Luiza da Silva](https://github.com/luizaxx) e [Wanjo Christopher](https://github.com/wChrstphr), 2026.</p></font>

### Requisitos Não Funcionais (RNF)

<font size="3"><p style="text-align: center">Tabela 4: Requisitos Não Funcionais</p></font>

| Código | Requisito Não Funcional | Rastreabilidade |
| :--: | -- | -- |
| RNF01 | O sistema deve ser responsivo (desktop e mobile). | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| RNF02 | O sistema deve proteger dados sensíveis. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| RNF03 | O sistema deve ter usabilidade simples para ações críticas (criar/buscar/aceitar carona em poucos passos). | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/); [BlaBlaCar](https://www.blablacar.com.br/) |
| RNF04 | O sistema deve registrar logs de ações relevantes (aceites, cancelamentos, denúncias) para auditoria. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| RNF06 | O sistema deve apresentar rotas e estimativas de tempo de forma consistente. | [Google Maps](https://www.google.com/maps)/[Waze](https://www.waze.com/) |

<font size="2"><p style="text-align: center">Fonte: [João Marcos](https://github.com/JJOAOMARCOSS), [Luiza da Silva](https://github.com/luizaxx) e [Wanjo Christopher](https://github.com/wChrstphr), 2026.</p></font>

---

## Conclusão

O benchmarking indicou que soluções bem-sucedidas combinam **facilidade de oferta/busca**, **comunicação direta**, **apoio por mapas** e mecanismos de **confiança** (reputação, denúncia e suporte). Para o CaronaAmiga FCTE, os principais aprendizados se concentram em adaptar essas práticas ao cenário universitário, com foco em comunidade restrita, rotas recorrentes e segurança.

---

## Referências Bibliográficas

> <a id="ref1">1.</a> IATA, Cristiane. Benchmarking: muito além de uma simples comparação. Revista Benchmarking, edição 1, dez. 2008. Disponível em: https://pontogp.wordpress.com/2008/12/24/benchmarking-muito-alem-de-uma-simples-comparacao. Acesso em 6 de abril de 2025.
> <a id="ref1">2.</a> BLABLACAR. *Página institucional*. Disponível em: https://www.blablacar.com.br/ride-sharing/services/como-funciona. Acesso em: 31 mar. 2026.  
> <a id="ref1">3.</a> UBER. *Página institucional (Brasil)*. Disponível em: https://www.uber.com/br/pt-br/. Acesso em: 31 mar. 2026.  
> <a id="ref1">4.</a> 99. *Página institucional*. Disponível em: https://99app.com/. Acesso em: 31 mar. 2026.  
> <a id="ref1">5.</a> GOOGLE. *Google Maps*. Disponível em: https://www.google.com/maps. Acesso em: 31 mar. 2026.  
> <a id="ref1">6.</a> WAZE. *Waze*. Disponível em: https://www.waze.com/pt-BR/. Acesso em: 31 mar. 2026.  
> <a id="ref1">7.</a> WHATSAPP. *WhatsApp*. Disponível em: https://www.whatsapp.com/?lang=pt_BR. Acesso em: 31 mar. 2026.  
> <a id="ref1">8.</a> TELEGRAM. *Telegram*. Disponível em: https://telegram.org/. Acesso em: 31 mar. 2026.  



## Histórico de Versões

| Versão | Data | Descrição | Autor(es) | Revisor(es) | Detalhes da revisão |
| :----: | :--: | --------- | ----------- | ------ | :---: |
| 1.0  | 31/03/2026 | Criação do documento [#36](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/issues/36) | [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS), [Luiza da Silva](https://github.com/luizaxx) e [Wanjo Christopher](https://github.com/wChrstphr) | [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharess) | - |
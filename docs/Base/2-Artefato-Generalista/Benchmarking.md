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

A atividade foi conduzida como uma análise exploratória, com seleção de referências por afinidade com o problema do projeto (mobilidade, caronas e coordenação de deslocamentos). As soluções foram agrupadas por categoria e avaliadas de forma qualitativa com base em critérios como:

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
  <summary size="20"><b>Marketplaces de carona</b></summary>

- [BlaBlaCar](https://www.blablacar.com.br/) — referência em caronas intermunicipais, com foco em confiança e perfis.
- [Liftango](https://www.liftango.com/) — caronas organizadas/empresariais (benchmark de operação com grupos fechados).

</details>

<details>
  <summary size="20"><b>Apps de mobilidade sob demanda (padrões de UX e segurança)</b></summary>

- [Uber](https://www.uber.com/br/pt-br/) — fluxo de corrida, segurança, compartilhamento de viagem e suporte.
- [99](https://99app.com/) — padrões similares para acompanhamento e comunicação.

</details>

<details>
  <summary size="20"><b>Mapas e rotas (apoio ao matching e pontos de encontro)</b></summary>

- [Google Maps](https://www.google.com/maps) — rotas, estimativas de tempo e pontos no mapa.
- [Waze](https://www.waze.com/pt-BR/) — tráfego em tempo real e rotas.

</details>

<details>
  <summary size="20"><b>Comunicação em grupos (coordenação prática de caronas)</b></summary>

- [WhatsApp](https://www.whatsapp.com/?lang=pt_BR) — coordenação por grupos, envio de localização e combinações rápidas.
- [Telegram](https://telegram.org/) — grupos/canais e organização de tópicos (quando habilitado).

</details>

---

## Tabela comparativa (síntese)

<font size="3"><p style="text-align: center">Tabela 2: Tabela comparativa</p></font>

| Critério | BlaBlaCar | Liftango | Uber/99 | Google Maps/Waze | WhatsApp/Telegram |
| :-- | :--: | :--: | :--: | :--: | :--: |
| Perfil do usuário | ✅ | ✅ | ✅ | ⚠️ (conta) | ✅ |
| Verificação/Confiança | ✅ (reputação) | ✅ (ambiente controlado) | ✅ (recursos de segurança) | ❌ | ❌ |
| Oferta e busca de carona | ✅ | ✅ | ⚠️ (corrida, não carona) | ❌ | ⚠️ (manual) |
| Matching/sugestão | ✅ | ✅ | ⚠️ | ❌ | ❌ |
| Definição de rota/ETA | ⚠️ | ✅ | ✅ | ✅ | ❌ |
| Chat/comunicação | ✅ | ✅ | ✅ | ❌ | ✅ |
| Ponto de encontro no mapa | ⚠️ | ✅ | ✅ | ✅ | ⚠️ |
| Avaliação/reputação | ✅ | ⚠️ | ✅ | ❌ | ❌ |
| Rateio/pagamento | ⚠️ (contribuição) | ⚠️ (depende) | ✅ (pagamento nativo) | ❌ | ⚠️ (manual) |


<p style="text-align: center">Legenda: ✅ presente / ⚠️ parcial / ❌ ausente.</p>

<font size="2"><p style="text-align: center">Fonte: [João Marcos](https://github.com/JJOAOMARCOSS), [Luiza da Silva](https://github.com/luizaxx) e [Wanjo Christopher](https://github.com/wChrstphr), 2026.</p></font>

---

## Requisitos elicitados

### Requisitos Funcionais (RF)

<font size="3"><p style="text-align: center">Tabela 3: Requisitos Funcionais</p></font>

| Código | Requisito Funcional | Rastreabilidade |
| :--: | -- | -- |
| RF01 | Permitir cadastro e gerenciamento de perfil do usuário (nome, curso/vínculo, foto opcional, preferências). | [BlaBlaCar](https://www.blablacar.com.br/); [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| RF02 | Permitir criação de oferta de carona com origem, destino, horário, vagas e observações. | [BlaBlaCar](https://www.blablacar.com.br/); [Liftango](https://www.liftango.com/) |
| RF03 | Permitir busca de caronas com filtros (origem/destino, horário, recorrência, vagas). | [BlaBlaCar](https://www.blablacar.com.br/); [Liftango](https://www.liftango.com/) |
| RF04 | Exibir rota no mapa com tempo estimado e alternativa de ponto de encontro. | [Google Maps](https://www.google.com/maps)/[Waze](https://www.waze.com/); [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| RF05 | Disponibilizar chat entre motorista e passageiro após solicitação/aceite. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/); [WhatsApp](https://www.whatsapp.com/?lang=pt_BR) |
| RF06 | Permitir solicitar participação em uma carona e permitir aceite/recusa pelo motorista. | [BlaBlaCar](https://www.blablacar.com.br/) |
| RF07 | Permitir cancelamento com registro de motivo e notificação às partes. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/); [BlaBlaCar](https://www.blablacar.com.br/) |
| RF08 | Implementar sistema de avaliação pós-corrida/caronas (nota e comentário opcional). | [BlaBlaCar](https://www.blablacar.com.br/); [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| RF09 | Permitir denúncia/bloqueio de usuário e canal de suporte. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| RF10 | Enviar notificações (match, aceite, alteração de horário, lembrete). | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/); [WhatsApp](https://www.whatsapp.com/?lang=pt_BR) |

<font size="2"><p style="text-align: center">Fonte: [João Marcos](https://github.com/JJOAOMARCOSS), [Luiza da Silva](https://github.com/luizaxx) e [Wanjo Christopher](https://github.com/wChrstphr), 2026.</p></font>

### Requisitos Não Funcionais (RNF)

<font size="3"><p style="text-align: center">Tabela 4: Requisitos Não Funcionais</p></font>

| Código | Requisito Não Funcional | Rastreabilidade |
| :--: | -- | -- |
| RNF01 | O sistema deve ser responsivo (desktop e mobile). | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| RNF02 | O sistema deve proteger dados sensíveis (hash de senha, TLS, controle de acesso). | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| RNF03 | O sistema deve ter usabilidade simples para ações críticas (criar/buscar/aceitar carona em poucos passos). | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/); [BlaBlaCar](https://www.blablacar.com.br/) |
| RNF04 | O sistema deve registrar logs de ações relevantes (aceites, cancelamentos, denúncias) para auditoria. | [Uber](https://www.uber.com/br/pt-br/)/[99](https://99app.com/) |
| RNF05 | O sistema deve manter disponibilidade adequada para uso em horários de pico (saída/entrada do campus). | [Liftango](https://www.liftango.com/) (contexto de operação) |
| RNF06 | O sistema deve apresentar rotas e estimativas de tempo de forma consistente. | [Google Maps](https://www.google.com/maps)/[Waze](https://www.waze.com/) |

<font size="2"><p style="text-align: center">Fonte: [João Marcos](https://github.com/JJOAOMARCOSS), [Luiza da Silva](https://github.com/luizaxx) e [Wanjo Christopher](https://github.com/wChrstphr), 2026.</p></font>

---

## Conclusão

O benchmarking indicou que soluções bem-sucedidas combinam **facilidade de oferta/busca**, **comunicação direta**, **apoio por mapas** e mecanismos de **confiança** (reputação, denúncia e suporte). Para o CaronaAmiga FCTE, os principais aprendizados se concentram em adaptar essas práticas ao cenário universitário, com foco em comunidade restrita, rotas recorrentes e segurança.

---

## Referências Bibliográficas

> <a id="referências-bibliográficas">1.</a> IATA, Cristiane. Benchmarking: muito além de uma simples comparação. Revista Benchmarking, edição 1, dez. 2008. Disponível em: https://pontogp.wordpress.com/2008/12/24/benchmarking-muito-alem-de-uma-simples-comparacao. Acesso em 6 de abril de 2025.
> 2. BLABLACAR. *Página institucional*. Disponível em: https://www.blablacar.com.br/. Acesso em: 31 mar. 2026.  
> 3. UBER. *Página institucional (Brasil)*. Disponível em: https://www.uber.com/br/pt-br/. Acesso em: 31 mar. 2026.  
> 4. 99. *Página institucional*. Disponível em: https://99app.com/. Acesso em: 31 mar. 2026.  
> 5. GOOGLE. *Google Maps*. Disponível em: https://www.google.com/maps. Acesso em: 31 mar. 2026.  
> 6. WAZE. *Waze*. Disponível em: https://www.waze.com/pt-BR/. Acesso em: 31 mar. 2026.  
> 7. WHATSAPP. *WhatsApp*. Disponível em: https://www.whatsapp.com/?lang=pt_BR. Acesso em: 31 mar. 2026.  
> 8. TELEGRAM. *Telegram*. Disponível em: https://telegram.org/. Acesso em: 31 mar. 2026.  
> 9. LIFTANGO. *Liftango*. Disponível em: https://www.liftango.com/. Acesso em: 31 mar. 2026.



## Histórico de Versões

| Versão | Data | Descrição | Autor(es) | Revisor(es) | Detalhes da revisão |
| :----: | :--: | --------- | ----------- | ------ | :---: |
| 1.0  | 31/03/2026 | Criação do documento [#36](https://github.com/UnBArqDsw2026-1-Turma02/2026.1-T02-G7_CaronaAmigaFCTE_Entrega_01/issues/36) | [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS), [Luiza da Silva](https://github.com/luizaxx) e [Wanjo Christopher](https://github.com/wChrstphr) | [Gustavo Ribeiro Linhares](https://github.com/GustavoLinharess) | - |
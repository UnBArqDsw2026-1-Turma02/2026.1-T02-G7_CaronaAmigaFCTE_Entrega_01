# Contribuindo

Este documento define os tópicos que devem orientar contribuições no projeto, para manter o time alinhado e reduzir retrabalho.

## Índice
1. [Fundamentação do Guia](#fundamentação-do-guia)
2. [Código de Conduta](#código-de-conduta)
3. [Canais de Comunicação](#canais-de-comunicação)
4. [Fluxo de Trabalho com Git](#fluxo-de-trabalho-com-git)
5. [Padrão de Commit](#padrão-de-commit)
6. [Padrão de Pull Request](#padrão-de-pull-request)
7. [Padrão de branch](#padrão-de-branch)
8. [Padrão de Issues](#padrão-de-issues)
9. [Padrão de Pull Request / Merge Request](#padrão-de-pull-request--merge-request)
10. [Qualidade, Testes e Revisão](#qualidade-testes-e-revisão)
11. [Definition of Done](#definition-of-done)
12. [Segurança e Dados Sensíveis](#segurança-e-dados-sensíveis)
13. [Referências](#referências)
14. [Histórico de Versões](#histórico-de-versões)

## Fundamentação do Guia [↑](#)
Este guia também se baseia em evidências empíricas de que a criação e, principalmente, a atualização ativa do arquivo `CONTRIBUTING.md` aumentam a chance de aceitação de contribuições de novos colaboradores e podem reduzir o tempo de análise de pull requests (GONÇALVES, 2025).

Por isso, este documento deve ser tratado como um artefato vivo do projeto.

## Código de Conduta [↑](#)
Antes de contribuir, leia [nossas diretrizes](/CODE_OF_CONDUCT.md).

## Canais de Comunicação [↑](#)
Os principais canais de comunicação são as Issues e Pull Requests. Prefira centralizar a comunicação por lá.

## Fluxo de Trabalho com Git [↑](#)
Utilizaremos o [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) para guiar o desenvolvimento e padronizar estilos, garantindo legibilidade e alinhamento do que está sendo feito.

Crie sempre a branch a partir da `main`.
### Padrão de Commit:
````md
<tipo>(escopo): <descrição>

<descrição longa> (opcional)

<Co-authored-by: Co-author Name <co-author-email@example.com>"> (opcional) 
````

#### Ex:
 ````md
feat(api-notificacao): adiciona envio automático de notificação de carona

Co-authored-by: Christopher <222037620@aluno.unb.br>
````

### Padrão de Pull Request:
````md
<tipo>(escopo ou nome da U.S.): <descrição>
````

#### Ex:
Título:
````
feat(compartilhar-carona): Adiciona envio de notificação automática
````

### Padrão de branch:

````
git checkout -b <tipo>/<escopo>
````

#### Ex:

```` bash
$ git checkout -b feat/compartilhar-carona
$ git add .
$ git commit -m "feat(notificacao): adiciona envio automático de notificação ao compartilhar carona"
$ git push
````

## Padrão de Issues [↑](#)
Para criação de novas Issues, siga os modelos específicos para `Artefatos`, `Features` e `Bugs`.

## Padrão de Pull Request / Merge Request [↑](#)
Para criação de novos Pull Requests, siga o template criado no repositório.

## Qualidade, Testes e Revisão [↑](#)
- Padrões de qualidade: passar no Sonar com `xyz%` de qualidade.
- Testes e validação: seguir os critérios descritos na Issue e no Pull Request.
- Processo de revisão: todo PR será revisado por, no mínimo, outro desenvolvedor para ser validado e mergeado na branch principal.

## Definition of Done [↑](#)
- [x] Issue atualizada
- [x] Revisão feita por outro desenvolvedor
- [x] Testes realizados
- [x] Pull Request preenchido e enviado
- [x] Documentação ajustada

## Segurança e Dados Sensíveis [↑](#)
Nunca publique senhas ou dados pessoais. Tudo que for sensível deve ser adicionado ao `.env.example` e armazenado no Teams do projeto.

## Referências [↑](#)
- GITHUB DOCS. **Setting guidelines for repository contributors**: GitHub. Disponível em: https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/setting-guidelines-for-repository-contributors. Acesso em: 29 mar. 2026.
- ATOM. **Contributing to Atom**: GitHub. Disponível em: https://github.com/atom/atom/blob/master/CONTRIBUTING.md. Acesso em: 29 mar. 2026.
- CONTRIBUTING.MD. **CONTRIBUTING.MD Example**: contributing.md. Disponível em: https://contributing.md/example/. Acesso em: 29 mar. 2026.
- THE GOOD DOCS PROJECT. **Template contributing guide**: GitLab. Disponível em: https://gitlab.com/tgdp/templates/-/blob/main/CONTRIBUTING.md. Acesso em: 29 mar. 2026.
- GONÇALVES, Silvana de Andrade; PLASTINO, Alexandre; SOARES, Daricélio Moreira. **Avaliando a Importância do Arquivo contributing.md em Projetos de Código Aberto**. In: SEMINÁRIO INTEGRADO DE SOFTWARE E HARDWARE (SEMISH), 52. , 2025, Maceió/AL. Anais [...]. Porto Alegre: Sociedade Brasileira de Computação, 2025 . p. 13-24. ISSN 2595-6205. DOI: https://doi.org/10.5753/semish.2025.6870.

## Histórico de Versões [↑](#)

| Versão | Data | Descrição | Autor(es) | Revisor(es) | Detalhes da revisão |
| :----: | :--: | --------- | ----------- | ------ | :---: |
| 1.0  | 29/03/2026 | Criação do documento | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS) | Artefato criado. |
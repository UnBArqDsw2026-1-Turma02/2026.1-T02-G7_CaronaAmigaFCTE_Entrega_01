# <a id ="ref0"> Contribuindo </a>

Este documento define os tópicos que devem orientar contribuições no projeto, para manter o time alinhado e reduzir retrabalho.

## Índice
1. [Fundamentação do Guia](#ref1)
2. [Código de Conduta](#ref2)
3. [Canais de Comunicação](#ref3)
4. [Fluxo de Trabalho com Git](#ref4)
5. [Padrão de Commit](#ref5)
6. [Padrão de Pull Request](#ref6)
7. [Padrão de branch](#ref7)
8. [Padrão de Issues](#ref8)
9. [Padrão de Pull Request / Merge Request](#ref9)
10. [Qualidade, Testes e Revisão](#ref10)
11. [Definition of Done](#ref11)
12. [Segurança e Dados Sensíveis](#ref12)
13. [Referências](#ref13)
14. [Histórico de Versões](#ref14)

## <a id="ref1"> Fundamentação do Guia </a> [↑](#ref0)
Este guia também se baseia em evidências empíricas de que a criação e, principalmente, a atualização ativa do arquivo `CONTRIBUTING.md` aumentam a chance de aceitação de contribuições de novos colaboradores e podem reduzir o tempo de análise de pull requests (GONÇALVES, 2025).

Por isso, este documento deve ser tratado como um artefato vivo do projeto.

## <a id="ref2"> Código de Conduta </a> [↑](#ref0)
Antes de contribuir, leia [nossas diretrizes](/CODE_OF_CONDUCT.md).

## <a id="ref3"> Canais de Comunicação </a> [↑](#ref0)
Os principais canais de comunicação são as Issues e Pull Requests. Prefira centralizar a comunicação por lá.

## <a id="ref4"> Fluxo de Trabalho com Git </a> [↑](#ref0)
Utilizaremos o [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) para guiar o desenvolvimento e padronizar estilos, garantindo legibilidade e alinhamento do que está sendo feito.

Crie sempre a branch a partir da `main`.
### <a id="ref5"> Padrão de Commit </a>:
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

### <a id="ref6"> Padrão de Pull Request </a>:
````md
<tipo>(escopo ou nome da U.S.): <descrição>
````

#### Ex:
Título:
````
feat(compartilhar-carona): Adiciona envio de notificação automática
````

### <a id="ref7"> Padrão de branch </a>:
Para criar sua branch automaticamente linkada à Issue e facilitar o desenvolvimento, faça o seguinte:
1. Navegue até a Issue que deseja trabalhar
2. Na aba direita, role para baixo até encontrar "Development" ou "Desenvolvimento"
3. Clique na engrenagem e clique em 'create a branch' ou 'criar uma branch'
4. Crie a branch e dê checkout localmente
![tela-de-criacao-branch-github](/docs/assets/criando_branch.png)

#### Ex:

```` bash
$ git checkout 20-docs-criação-do-protótipo-de-alta-fidelidade
$ git add .
$ git commit -m "docs(design-sprint): adiciona protótipos da tela de compartilhar carona"
$ git push
````

## <a id="ref8"> Padrão de Issues </a> [↑](#ref0)
Para criação de novas Issues, siga os modelos específicos para `Artefatos`, `Features` e `Bugs`.

## <a id="ref9"> Padrão de Pull Request / Merge Request </a> [↑](#ref0)
Para criação de novos Pull Requests, siga o template criado no repositório.

## <a id="ref10"> Qualidade, Testes e Revisão </a> [↑](#ref0)
- Padrões de qualidade: passar no Sonar com `xyz%` de qualidade.
- Testes e validação: seguir os critérios descritos na Issue e no Pull Request.
- Processo de revisão: todo PR será revisado por, no mínimo, outro desenvolvedor para ser validado e mergeado na branch principal.

## <a id="ref11"> Definition of Done </a> [↑](#ref0)
- [x] Issue atualizada
- [x] Revisão feita por outro desenvolvedor
- [x] Testes realizados
- [x] Pull Request preenchido e enviado
- [x] Documentação ajustada

## <a id="ref12"> Segurança e Dados Sensíveis </a> [↑](#ref0)
Nunca publique senhas ou dados pessoais. Tudo que for sensível deve ser adicionado ao `.env.example` e armazenado no Teams do projeto.

## <a id="ref13"> Referências </a> [↑](#ref0)
> GITHUB DOCS. **Setting guidelines for repository contributors**: GitHub. Disponível em: https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/setting-guidelines-for-repository-contributors. Acesso em: 29 mar. 2026.

> ATOM. **Contributing to Atom**: GitHub. Disponível em: https://github.com/atom/atom/blob/master/CONTRIBUTING.md. Acesso em: 29 mar. 2026.

> CONTRIBUTING.MD. **CONTRIBUTING.MD Example**: contributing.md. Disponível em: https://contributing.md/example/. Acesso em: 29 mar. 2026.

> THE GOOD DOCS PROJECT. **Template contributing guide**: GitLab. Disponível em: https://gitlab.com/tgdp/templates/-/blob/main/CONTRIBUTING.md. Acesso em: 29 mar. 2026.

> GONÇALVES, Silvana de Andrade; PLASTINO, Alexandre; SOARES, Daricélio Moreira. **Avaliando a Importância do Arquivo contributing.md em Projetos de Código Aberto**. In: SEMINÁRIO INTEGRADO DE SOFTWARE E HARDWARE (SEMISH), 52. , 2025, Maceió/AL. Anais [...]. Porto Alegre: Sociedade Brasileira de Computação, 2025 . p. 13-24. ISSN 2595-6205. DOI: https://doi.org/10.5753/semish.2025.6870.

## <a id="ref14"> Histórico de Versões </a> [↑](#ref0)

| Versão | Data | Descrição | Autor(es) | Revisor(es) | Detalhes da revisão |
| :----: | :--: | --------- | ----------- | ------ | :---: |
| 1.0  | 29/03/2026 | Criação do documento | [Wanjo Christopher Paraizo Escobar](https://github.com/wChrstphr) | [João Marcos Moraes de Andrade](https://github.com/JJOAOMARCOSS) | Artefato criado. |
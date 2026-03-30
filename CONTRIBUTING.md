# Contribuindo

Este documento define os tópicos que devem orientar contribuições no projeto, para manter o time alinhado e reduzir retrabalho.

## 1. Fundamentação do Guia
Este guia também se baseia em evidências empíricas de que a criação e, principalmente, a atualização ativa do arquivo `CONTRIBUTING.md` aumentam a chance de aceitação de contribuições de novos colaboradores e podem reduzir o tempo de análise de pull requests (GONÇALVES, 2025). Reforçando que este documento deve ser tratado como um artefato vivo do projeto.

## 2. Código de Conduta
Antes de entender como contribuir, compreenda [nossas diretrizes](/CODE_OF_CONDUCT.md). 

## 3. Canais de Comunicação
O principal canal de comunicação serão as Issues e Pull Requests, prefira se comunicar por lá.

## 5. Fluxo de Trabalho com Git
Utilizaremos o [Convetional Commits](https://www.conventionalcommits.org/en/v1.0.0/) para guiar o desenvolvimento e padronizar estilos, garantindo legibilidade e alinhamento do que está sendo feito.

Padrão de Commit:
````md
<tipo>(/escopo opcional): <descrição>

<descrição longa> (opcional)

<Co-authored-by: Co-author Name <co-author-email@example.com>"> (opcional) 
````

Ex:
 ````md
feat(api-notificacao): adiciona envio automático de notificação de carona

Co-authored-by: Christopher <222037620@aluno.unb.br>
````

Padrão de PR:


Padronizar criação de branch, commits, sincronização com a branch principal e abertura de PR/MR para manter histórico limpo.

## 6. Padrão de Issues
Especificar o que uma issue deve conter (contexto, problema, passos para reproduzir quando aplicável, comportamento esperado vs. atual, critérios de aceite e prioridade) para facilitar planejamento e execução.

## 7. Padrão de Pull Request / Merge Request
Definir checklist de PR (descrição, issue vinculada, evidências e impactos, instruções de validação e atualização de documentação), garantindo revisões mais rápidas e objetivas.

## 8. Convenções de Commits
Indicar formato de mensagem de commit (ex.: Conventional Commits) para melhorar rastreabilidade e organização do histórico.

## 9. Padrões de Qualidade
Consolidar critérios de qualidade para código e documentação (estilo, estrutura e consistência), reduzindo correções posteriores.

## 10. Testes e Validação
Estabelecer como validar alterações antes do merge (testes automatizados ou validação manual), garantindo maior confiança nas entregas.

## 11. Processo de Revisão
Definir quantidade mínima de aprovadores, papéis de revisão e tratamento de feedback para manter qualidade e colaboração. Sempre exigir aprovação por pares e status checks verdes antes do merge.

## 12. Definition of Done
Listar critérios para considerar uma tarefa concluída (issue atualizada, revisão aprovada, testes feitos, documentação ajustada e versionamento atualizado quando aplicável).

## 13. Segurança e Dados Sensíveis
Orientar sobre não publicar segredos, tokens ou dados pessoais e como reportar falhas sensíveis de forma privada.

## 14. Papéis e Organização da Equipe
Explicar responsabilidades do grupo (manutenção, revisão, documentação e coordenação), importante para um time privado com 10 pessoas.

## 15. Priorização e Planejamento
Definir como priorizar tarefas e mudanças de escopo durante as sprints para manter previsibilidade das entregas.

## 16. Licença e Direitos Autorais
Registrar que cada contribuição deve ser de autoria própria e compatível com a licença adotada no projeto.

## 17. Reconhecimento de Contribuições
Descrever como o time registra participação e evolução das entregas, promovendo transparência e motivação.

## Referências
- GITHUB DOCS. **Setting guidelines for repository contributors**: GitHub. Disponível em: https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/setting-guidelines-for-repository-contributors. Acesso em: 29 mar. 2026.
- ATOM. **Contributing to Atom**: GitHub. Disponível em: https://github.com/atom/atom/blob/master/CONTRIBUTING.md. Acesso em: 29 mar. 2026.
- CONTRIBUTING.MD. **CONTRIBUTING.MD Example**: contributing.md. Disponível em: https://contributing.md/example/. Acesso em: 29 mar. 2026.
- THE GOOD DOCS PROJECT. **Template contributing guide**: GitLab. Disponível em: https://gitlab.com/tgdp/templates/-/blob/main/CONTRIBUTING.md. Acesso em: 29 mar. 2026.
- GONÇALVES, Silvana de Andrade; PLASTINO, Alexandre; SOARES, Daricélio Moreira. **Avaliando a Importância do Arquivo contributing.md em Projetos de Código Aberto**. In: SEMINÁRIO INTEGRADO DE SOFTWARE E HARDWARE (SEMISH), 52. , 2025, Maceió/AL. Anais [...]. Porto Alegre: Sociedade Brasileira de Computação, 2025 . p. 13-24. ISSN 2595-6205. DOI: https://doi.org/10.5753/semish.2025.6870.
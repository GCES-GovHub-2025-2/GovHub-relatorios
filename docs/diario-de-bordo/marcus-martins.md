# Diário de Bordo – \[Marcus Martins]

**Disciplina:** \[GCES]

**Equipe:** \[GovHub]

**Comunidade/Projeto de Software Livre:** \[GovHub-br]

---

## Sprint 0 – \[01/09/2025 – 10/09/2025]

### Resumo da Sprint

Durante a sprint 0, foquei na documentação inicial das práticas de Gerência de Configuração e Evolução de Software (GCES) para o projeto GovHub. Criei um documento no Google Docs que serviu como base para alinhar a equipe sobre os processos de contribuição e a futura migração do GitLab para o Github. A documentação também inclui o mapeamento dos membros da equipe, anotações para possíveis issues e a criação do Git Pages para facilitar a transparência do progresso de atividades.

### Atividades Realizadas

| Data  | Atividade                                   | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status    |
| ----- | ------------------------------------------- | --------------------------------- | --------------- | --------- |
| 01/09 | Anotações no grupo de possíveis issues com base na reunião com a professora Carla | Discussão/Documentação | – | Concluído |
| 01/09 | Criação do documento de GCES e organização das informações da equipe | Documentação | [Google Docs](https://docs.google.com/document/d/1gwo-WKB09nKjJ5ghYFihoAGSMAReoC442PUmTbsKAY0/edit?usp=sharing) | Concluído |
| 03/09 | Análise e documentação do fluxo de contribuição | Documentação | [Google Docs](https://docs.google.com/document/d/1gwo-WKB09nKjJ5ghYFihoAGSMAReoC442PUmTbsKAY0/edit?usp=sharing) | Concluído |
| 09/09 | Criação e estruturação do Git Pages dos relatórios de contribuição | Documentação | [Relatórios](https://gces-govhub-2025-2.github.io/GovHub-relatorios/) | Concluído |
| 09/09 | Organização de pipeline do Git Pages | Documentação | [Relatórios](https://gces-govhub-2025-2.github.io/GovHub-relatorios/) | Concluído |


### Maiores Avanços

- **Centralização das informações da equipe:** O Docs criado centraliza o contato dos membros do time (Github e Telegram), facilitando a comunicação e a colaboração.
- **Documentação inicial de GCES:** A análise e documentação das práticas atuais de Gerência de Configuração e Evolução forneceu um ponto de partida para a padronização do fluxo de trabalho.
- **Mapeamento de issues:** A anotação de possíveis issues durante a reunião ajudou a identificar pontos de melhoria no projeto, preparando o caminho para as próximas contribuições.

<!--
* \[Exemplo] Aprendi a rodar a aplicação localmente.
* \[Exemplo] Entendi melhor a organização do repositório.
-->

### Maiores Dificuldades

- A principal dificuldade foi a duplicidade de repositórios (GitLab e Github), que causa fragmentação da documentação e dificulta a padronização dos processos de contribuição e o entendimento do projeto como um todo.

### Aprendizados

- Entendimento do projeto GovHub e seus objetivos.

- Noções sobre Gerência de Configuração e Evolução no contexto de projetos de software livre.

### Plano Pessoal para a Próxima Sprint

- [X] Contribuir com pelo menos 1 PR.
- [X] Transformar as anotações feitas em issues concretas.

---

## Sprint 1 – \[11/09/2025 – 24/09/2025]

### Resumo da Sprint

Durante a Sprint 1, o foco principal foi na migração do pipeline de CI/CD do GitLab para o GitHub Actions, incluindo a transcrição dos scripts e a migração das variáveis de ambiente. Submeti um pull request com essa implementação e configurei o SonarCloud no novo ambiente. Também participei de discussões de gestão com a equipe e continuei a aprofundar meu conhecimento sobre o projeto por meio do livro do GovHub e do evento de lançamento.

### Atividades Realizadas

| Data  | Atividade                                   | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status    |
| ----- | ------------------------------------------- | --------------------------------- | --------------- | --------- |
| 17/09 | Discussão com Davi Aguiar e Mateus de Castro sobre gestão da equipe e definição de possíveis de issues | Discussão | – | Concluído |
| 18/09 | Reunião com a equipe para alinhamento sobre a estrutura, documentação e objetivos | Discussão | – | Concluído |
| 18/09 | Criação de arquivo de pipelines transcrito do GitLab CI para o Github Actions | Código | – | Concluído |
| 19/09 | Migração de variáveis de ambiente do GitLab para o Github e configuração do SonarCloud | Código | – | Concluído |
| 19/09 | Pull Request da pipeline | Código | [Pull request](https://github.com/GovHub-br/data-application-gov-hub/pull/11) | Esperando aprovação |
| 23/09 | Participação no evento do GovHub | Discussão | – | Concluído |
| 23/09 | Leitura do livro do GovHub | Discussão | – | Em progresso |

### Maiores Avanços

- **Migração do pipeline de CI/CD:** A criação e configuração do pipeline no GitHub Actions vai garantir que as práticas de automação e qualidade do código sejam mantidas após a transição do GitLab.

- **Primeira contribuição de código (PR):** A abertura do pull request da pipeline, cumprindo com o plano da sprint anterior.

- **Alinhamento com a comunidade:** A participação nas discussões sobre gestão e o evento do GovHub fortaleceu meu alinhamento com os objetivos do projeto.

### Maiores Dificuldades

- A principal dificuldade foi a tradução dos scripts e ter de ir atrás dos mantenedores dos projetos para obter acesso às plataformas necessárias para configurar a pipeline. Pois, além de entender e transpilar a pipeline, tive que buscar os valores das variáveis de ambiente e criar novas chaves para o SonarCloud

### Aprendizados

- **Criação de pipelines:** Aprendi a sintaxe e o fluxo de trabalho tanto do Github Actions quanto do GitLab CI, incluindo a configuração de jobs, steps e variáveis de ambiente.

- **Ferramentas de qualidade de código:** Entendi o processo de integração do SonarCloud com o GitHub para análise estática e verificação de qualidade do código.

- **Dinâmica do projeto:** O evento e a leitura do livro do GovHub aprofundaram meu entendimento sobre a proposta do projeto e as ferramentas utilizadas.

### Plano Pessoal para a Próxima Sprint

- [] Submeter um novo pull request que contribua com o código do projeto.
- [] Participar da revisão de código de um colega.
- [] Concluir a leitura do livro do GovHub.

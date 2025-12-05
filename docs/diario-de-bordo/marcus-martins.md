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

Durante a Sprint 3, meu foco foi a construção de uma pipeline de ingestão de dados para o endpoint `/deputados` da API da Câmara dos Deputados. Desenvolvi toda a lógica de extração, incluindo a orquestração no Airflow para buscar dados históricos e o tratamento de paginação. Além disso, refatorei o código para um padrão mais limpo e manutenível, abstraindo a lógica da API para uma classe cliente, seguindo o padrão do projeto. No final da sprint, uma falha de comunicação foi identificada: eu estava commitando no repositório principal do GovHub em vez de no fork da disciplina, o que invalidou o meu código mas me fez ter uma ideia melhor do funcionamento do Airflow. Apesar da perda do trabalho inicial, a experiência permitiu um aprofundamento técnico no problema, o que facilitará o desenvolvimento da próxima tarefa, a ingestão de /deputados/{id}.

https://github.com/GovHub-br/data-application-gov-hub/pull/23

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
- [X] Participar da revisão de código de um colega.
- [X] Concluir a leitura do livro do GovHub.

---

## Sprint 2 – \[25/09/2025 – 08/10/2025]

### Resumo da Sprint

Nesta sprint, o foco principal foi garantir a integridade do código antes mesmo dele chegar ao repositório remoto ("Shift Left"). Para isso, trabalhei em Pair Programming com o Arthur, onde configuramos e corrigimos os hooks de git (pré-commit e pré-push). O objetivo era padronizar o ambiente de desenvolvimento local para espelhar as verificações que implementei na pipeline de CI na sprint anterior. Além disso, realizamos ajustes finos na pipeline de análise estática para reduzir falsos positivos e bloquear a entrada de "code smells".

### Atividades Realizadas

| Data  | Atividade                                   | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status    |
| ----- | ------------------------------------------- | --------------------------------- | --------------- | --------- |
| 25/10 | Reunião de alinhamento com Arthur para definir estratégia dos Git Hooks | Discussão | – | Concluído |
| 30/10 | Configurações do framework pre-commit no repositório | Código | – | Concluído |
| 05/10 | Pareamento com Arthur: Correção de erros de linting bloqueando o commit | Código | – | Concluído |
| 07/10 | Refinamento das regras do SonarCloud (Quality Gates) | Configuração | – | Concluído |

### Maiores Avanços

- **Título:** Inserir avanços

- **Padronização do Ambiente Local:** Com a implementação do pre-commit e pre-push, garantimos que todos os desenvolvedores rodem as mesmas verificações de estilo e testes básicos antes de submeter código, reduzindo falhas na CI remota.

- **Fortalecimento da Cultura de DevOps:** O pareamento com o Arthur permitiu a transmissão de conhecimento sobre a infraestrutura de testes e análise estática dentro da equipe.

- **Qualidade de Código:** A pipeline de análise estática agora está mais rigorosa, mas justa, ignorando arquivos gerados automaticamente que "sujavam" as métricas do SonarCloud.

### Maiores Dificuldades

- **Configuração de Hooks em Diferentes SOs:** Tivemos problemas para fazer os scripts de pre-push rodarem consistentemente tanto no Linux (meu ambiente) quanto no Mac (ambiente de outros membros), exigindo ajustes nos scripts de shell.

### Aprendizados

- **Título:** Inserir aprendizados

- **Framework Pre-commit:** Aprofundei meu conhecimento na ferramenta pre-commit, aprendendo a criar ganchos personalizados além dos padrões da comunidade.

- **Pair Programming:** A experiência de codificar simultaneamente com o Arthur melhorou a velocidade de resolução de problemas complexos de configuração, além de reduzir o tempo de code review posterior.

- **Conceito de Shift-Left:** Entendi na prática como trazer as verificações de qualidade para o início do ciclo de desenvolvimento economiza recursos computacionais da CI e tempo dos desenvolvedores.

### Plano Pessoal para a Próxima Sprint

- [X] Pegar uma issue relacionada a pipeline de dados

...

## Sprint 3 – \[09/10/2025 – 22/10/2025]

### Resumo da Sprint

O foco foi na criação da DAG ingestão de /deputados, no entanto por falta de comunicação eu estava commitando no repositório principal e não no fork da disciplina, o que foi um problema pois já havia outro estudante trabalhando na mesma issue, o que apesar de me fazer ter feito perder o que eu já havia trabalhado, me fez entender melhor o escopo para poder trabalhar na ingestão de /deputados/id.

Nesta sprint, dediquei-me ao desenvolvimento da pipeline de ingestão de dados para o endpoint `/deputados` da API da Câmara dos Deputados. Implementei uma DAG no Airflow utilizando _dynamic task mapping_ para lidar com a paginação e a lógica de deduplicação de dados.

Contudo, houve um desalinhamento no fluxo de contribuição: realizei o desenvolvimento e abri o PR no repositório _upstream_ (GovHub oficial) ao invés do fork da disciplina (GCES), pois, até o momento, me confundi pois estava trabalhando no _upstream_ e em ferramentas externas. Como resultado, o trabalho colidiu com o de outro membro (Leonardo Bonetti), que teve seu código mergeado corretamente no fork. Apesar do meu código não ter sido aproveitado diretamente, o processo foi importante para entender a arquitetura de plugins do projeto e receber feedbacks técnicos sobre separação de responsabilidades (Cliente vs. DAG), o que me prepara para a próxima tarefa: a ingestão de detalhes dos deputados (`/deputados/{id}`).

### Atividades Realizadas

| Data  | Atividade                                   | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status    |
| ----- | ------------------------------------------- | --------------------------------- | --------------- | --------- |
| 10/10 | Estudo da documentação do Airflow (Task Mapping e XComs) | Estudo | – | Concluído |
| 14/10 | Implementação da lógica de paginação e extração da API /deputados | Código | – | Concluído |
| 18/10 | Desenvolvimento da DAG deputados_ingest_dag com lógica de upsert | Código | – | Concluído |
| 20/10 | Abertura do PR #23 (Repositório _upstream_) | Código | [PR #23](https://github.com/GovHub-br/data-application-gov-hub/pull/23) | – |
| 20/10 | Revisão de código: Discussão sobre refatoração do Cliente API (feedback do João Egewarth) | Discussão | – | Concluído |
| 21/10 | Encerramento do PR devido ao merge da issue no fork da disciplina | Gestão | – | Concluído |
| 21/10 | Auto-atribuição da issue [#5](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/5) (Ingestão de detalhes `/deputados/{id}`) | Tipo | – | [Issue #5](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/5) |

### Maiores Avanços

- **Compreensão do Funcionamento do Airflow:** Implementei uma DAG com dynamic task mapping, lidando com paginação e consolidação de dados brutos (raw layer).

- **Qualidade de Código:** Através do feedback do Copilot e do membro Egewarth, entendi a importância de desacoplar a lógica de requisição HTTP (que deve ficar em um plugins/cliente_*.py) da lógica de orquestração da DAG.

### Maiores Dificuldades

- **Gestão de Configuração (Repositórios):** A confusão entre o repositório oficial do GovHub e o fork da disciplina de GCES causou retrabalho e invalidou o PR.

- **Concorrência de Trabalho:** Não ter verificado o andamento das atividades no fork da disciplina fez com que eu trabalhasse em uma issue que já estava sendo resolvida paralelamente por outro colega.

### Aprendizados

- **Arquitetura do Projeto:** Aprendi o padrão de projeto utilizado pelo GovHub, onde a DAG deve apenas orquestrar, e a lógica de negócio/extração deve residir em classes "Cliente" separadas.

- **Fluxo de Contribuição GCES:** A importância de verificar o upstream e trabalhar estritamente no fork da disciplina para garantir que o trabalho seja computado e não haja conflitos.

- **Revisão de Código:** Valorizei o processo de Code Review (mesmo em um PR fechado), pois as sugestões de melhoria na estrutura do código serão aplicadas diretamente na minha próxima tarefa.

### Plano Pessoal para a Próxima Sprint

- [] Implementar a DAG para o endpoint /deputados/{id}

- [] Criar a classe cliente_deputados_id.py seguindo o padrão aprendido, abstraindo a lógica da API.

- [] Garantir que o PR seja aberto no repositório correto (GCES-GovHub-2025-2).

## Sprint 4 – 23/10/2025 – 05/11/2025

Nesta sprint, dediquei-me inteiramente à implementação da ingestão de detalhes dos deputados (`/deputados/{id}`). A lógica de negócio, a DAG utilizando _dynamic task mapping_ e os testes unitários foram desenvolvidos com sucesso. No entanto, enfrentei um bloqueio técnico no fluxo de contribuição: os _hooks_ de _pre-push_ estavam rejeitando meus commits devido a erros de linting e importação que não ocorriam durante a execução dos testes locais ou no _pre-commit_. Passei a segunda metade da _sprint_ num ciclo de refatoração e ajustes de configuração (`Makefile`, `pyproject.toml`, `mypy`) para tentar alinhar o ambiente local com as exigências do _hook_, mas não consegui subir o código para o repositório remoto antes do fim da _sprint_.

### Atividades Realizadas

| Data  | Atividade                                   | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status    |
| ----- | ------------------------------------------- | --------------------------------- | --------------- | --------- |
| 24/10 | Estudo do endpoint `/deputados/{id}` e planejamento da estrutura da DAG | Estudo | – | Concluído |
| 27/10 | Implementação do método `get_deputados_id` no `ClienteDeputados` | Código | – | Concluído (Local) |
| 29/10 | Criação da DAG `deputados_id_ingest_dag` usando `.expand()` para tarefas dinâmicas | Código | – | Concluído (Local) |
| 31/10 | Escrita de testes unitários para o novo Cliente e DAG | Código | – | Concluído (Local) |
| 03/10 | Tentativa de Push: Falha no `mypy` acusando erros de importação | Configuração | – | Falhou |
| 04/10 | Refatoração das importações e ajustes no `pyproject.toml` para satisfazer o _linter_ | Código | – | Em andamento |
| 05/10 | Tentativas de ajuste no `Makefile` para corrigir o `AIRFLOW_HOME` nos _hooks_ | Configuração | – | Em andamento |

### Maiores Avanços

- **Implementação da DAG Dinâmica:** Finalizei localmente a lógica da DAG que lê IDs do banco e dispara tarefas paralelas para buscar detalhes, utilizando o recurso expand do Airflow.

- **Cobertura de Testes:** Criei uma suíte de testes, mockando tanto a API da Câmara quanto o banco Postgres, garantindo que a lógica de _upsert_ e tratamento de erros estivesse correta.

- **Evolução dos Clientes:** Aprimorei o `ClienteEmendas` com tipagem correta para os parâmetros de busca e padronizei o `ClienteDeputados`.

### Maiores Dificuldades

- **Inconsistência de Ambiente (Local vs Hooks):** A maior frustração foi que `poetry run pytest` passava com sucesso, mas o script de _pre-push_ falhava. O linter acusava que não encontrava os módulos locais (`airflow_lappis`), sugerindo um erro de `PYTHONPATH` ou configuração do `mypy`.

- **Configuração de Tooling:** Tive que entender a configuração do `Makefile` para descobrir que a variável `AIRFLOW_HOME` precisava ser setada explicitamente para que as importações funcionassem dentro do ambiente isolado dos _hooks_.

- **Impossibilidade de Push:** Apesar de ter o código funcional, fiquei preso sem conseguir compartilhar o progresso no GitHub, o que gerou ansiedade sobre a visibilidade do meu trabalho.

### Aprendizados

- **Arquitetura do Projeto:** Aprendi o padrão de projeto utilizado pelo GovHub, onde a DAG deve apenas orquestrar, e a lógica de negócio/extração deve residir em classes "Cliente" separadas.

- **Linting Rigoroso:** Aprendi (da maneira difícil) que linters como o `mypy` são extremamente sensíveis a caminhos de importação e configurações de projeto (`pyproject.toml`), exigindo exclusões explícitas ou configurações de _path_ corretas.

- **Gestão de Dependências:** Entendi a necessidade de incluir bibliotecas como `python-dotenv` explicitamente nas dependências do projeto para garantir que variáveis de ambiente sejam carregadas corretamente nos scripts de automação.

- **Scripts de Make:** Aprofundei meu conhecimento em `Makefiles`, especificamente em como injetar variáveis de ambiente antes da execução de comandos Python.

### Plano Pessoal para a Próxima Sprint

- [] Finalizar a configuração do Makefile para passar no pre-push.
- [] Realizar o push do código acumulado (DAG de detalhes + Correções de Emendas).
- [] Abrir o Pull Request e solicitar revisão imediata para compensar o atraso.

## Sprint 5 – 06/11/2025 – 19/11/2025

Esta sprint foi marcada por uma intensa batalha contra as ferramentas de linting e configuração do projeto. Continuei as tentativas de subir o código desenvolvido na sprint anterior, mas o hook de pre-push continuou bloqueando o envio com erros que, muitas vezes, pareciam inconsistentes ou falsos positivos. Em um momento de frustração, cheguei a reescrever todo o código do zero para garantir que não havia "sujeira" oculta. Busquei ajuda com o Professor Renato, que me orientou sobre a prática de commits atômicos: enviar pequenas alterações isoladas em vez de tentar subir tudo de uma vez. Tentei aplicar essa estratégia, separando configurações de infraestrutura (Makefile, pyproject.toml) das mudanças de lógica (DAGs, Clientes), mas mesmo assim, o pipeline local insistia em rejeitar as alterações, tornando o processo exaustivo.

### Atividades Realizadas

| Data  | Atividade                                   | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status    |
| ----- | ------------------------------------------- | --------------------------------- | --------------- | --------- |
| 06/11 | Tentativa de commit geral com correções no `Makefile` e `pyproject.toml` | Configuração | – | Bloqueado |
| 08/11 | Refatoração completa: reescrita dos arquivos para tentar limpar o lint | Código | – | Concluído |
| 11/11 | Sessão de debug dos erros de importação apontados pelo `mypy` | Análise | – | Concluído |
| 13/11 | Mentoria com Professor Renato: Discussão sobre granularidade de commits | Discussão | – | Concluído |
| 14/11 | Separação das alterações em commits mais atômicos ainda | Gestão de Configuração | – | Concluído |
| 17/11 | Ajustes nas regras de ignore do `pyproject.toml` para contornar falsos positivos | Configuração | – | Falhow |
| 19/11 | Nova bateria de testes locais (passaram) vs. tentativa de push (falhou) | Teste | – | Bloqueado |

### Maiores Avanços

- **Implementação da DAG Dinâmica:** Finalizei localmente a lógica da DAG que lê IDs do banco e dispara tarefas paralelas para buscar detalhes, utilizando o recurso expand do Airflow.

- **Mentoria Técnica:** A conversa com o Professor Renato me fez repensar a forma como eu estava commitando. Entendi que, como os commits em tamanho normal não estavam passando, deveria atômizar ao extremo, facilitando o debug e isolando problemas.

- **Aprofundamento em Tooling:** Devido aos erros, fui obrigado a entender a fundo como o `Makefile` interage com o `pytest` e como as variáveis de ambiente (`AIRFLOW_HOME`)  afetam a descoberta de módulos no Python.

- **Configuração de Linters:** Aprendi a configurar exceções específicas no `pyproject.toml` para o `mypy`, tentando criar um meio-termo entre rigor e produtividade.

### Maiores Dificuldades

- **Inconsistência de Ambiente (Local vs Hooks):** A maior frustração foi que `poetry run pytest` passava com sucesso, mas o script de _pre-push_ falhava. O linter acusava que não encontrava os módulos locais (`airflow_lappis`), sugerindo um erro de `PYTHONPATH` ou configuração do `mypy`.

- **Linting:** A ferramenta apontava erros de importação que não existiam funcionalmente (o código rodava, os testes o pré-commit passavam), criando uma barreira artificial que impedia o progresso.

- **Rejeição Persistente:** A sensação de "nadar e morrer na praia", onde horas de ajustes finos resultavam na mesma mensagem de erro do hook de pre-push, foi desmotivadora.

### Aprendizados

- **Commits Atômicos:** A vivência de bloqueios no fluxo de contribuição reforçou a importância da atomicidade.

- **Paciência e Persistência:** O exercício de reescrever o código e tentar múltiplas abordagens de configuração testou minha resiliência como desenvolvedor.

### Plano Pessoal para a Próxima Sprint

- [] Conseguir, finalmente, realizar o push.
- [] Abrir o PR da ingestão de detalhes de deputados.

## Sprint 6 – 20/11/2025 – 03/12/2025

O esforço desproporcional gasto em tooling em vez de lógica de negócio gerou frustração e estagnação. Após conversar com a equipe e avaliar o custo-benefício, tomei a decisão de desistir dessa issue específica para não comprometer meu progresso na disciplina. O código foi arquivado localmente e decidi buscar um novo escopo de trabalho para recuperar o ritmo.

Para virar a página após a sprint anterior, aceitei o convite do Davi Aguiar para contribuir diretamente no repositório oficial do GovHub (fora do fork da disciplina), assumindo a Issue #42. O objetivo era implementar a ingestão de "Planos de Trabalho Especial" do TransfereGov.

O desenvolvimento da lógica fluiu muito bem, mas o processo de revisão (PR #47) foi uma verdadeira escola sobre escopo e padrões de projeto. Cometi erros ao tentar refatorar códigos alheios à minha tarefa (o que gerou conflitos) e tive que lidar com correções de qualidade apontadas pelo SonarCloud.

### Atividades Realizadas

| Data  | Atividade                                   | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status    |
| ----- | ------------------------------------------- | --------------------------------- | --------------- | --------- |
| 03/12 | Aceite da Issue #42 e estudo do Swagger do TransfereGov | Estudo | [Issue #42](https://github.com/GovHub-br/data-application-gov-hub/issues/42) | Concluído |
| 03/12 | Implementação do ClienteTransfereGov com paginação automática (`get_all_...`) | Código | – | Concluído |
| 04/12 | Criação da DAG `ingest_transferegov_plano_trabalho_especial` com Dynamic Task Mapping | Código | – | Concluído |
| 04/12 | Tentativa de correção geral: Ajustes em helpers e renomeação de tabelas | Código | – | Concluído |
| 04/12 | Correção de bug no `insert_data` (argumentos invertidos) apontado pelo Sonar | Código | – | Concluído |
| 03/12 | Revisão de Davi para alinhar reversão de arquivos fora do escopo | Discussão | [PR #47](https://github.com/GovHub-br/data-application-gov-hub/pull/47) | Em correção |

### Maiores Avanços

- **Ingestão Complexa:** Implementei com sucesso a coleta de dados da API TransfereGov, criando métodos que iteram automaticamente por todas as páginas de resultados.

- **Dynamic Task Mapping:** Utilizei o recurso `.expand()` do Airflow para criar uma tarefa de ingestão para cada plano de ação listado, paralelizando o processo de coleta em lotes.

### Maiores dificuldades

- **Escopo do PR:** Na tentativa de fazer minha DAG rodar localmente, alterei arquivos globais (`postgres_helpers`) e renomeei tabelas em DAGs vizinhas. Isso foi vetado na revisão de código pois poderia quebrar pipelines em produção.

- **Confusão de Schemas:** Perdi tempo tentando buscar dados na tabela errada. O projeto usa schemas distintos (`transferegov` e `transferegov_emendas`), e eu não estava encontrando as chaves estrangeiras necessárias para rodar minha pipeline.

### Aprendizados

- **Respeito Estrito ao Escopo:** Aprendi na prática que um PR deve conter apenas as mudanças daquela issue. Se encontrei um erro no helper de conexão do banco, devo abrir um PR separado para corrigir isso, e não embutir na minha feature.

- **Argumentos Nomeados:** O erro de inversão de parâmetros (`data` e `table_name`) me ensinou a sempre usar argumentos nomeados em Python (func(data=x, table=y)) para evitar bugs silenciosos.

- **Review como Aprendizado:** Encarei os comentários do Davi pedindo reversão de arquivos não como uma crítica negativa, mas como uma proteção para a estabilidade do projeto oficial.

### Plano Pessoal para a futuro

- [] Reverter as alterações nos arquivos fora do escopo (`postgres_helpers`, outras DAGs).
- [] Garantir o merge do PR #47.
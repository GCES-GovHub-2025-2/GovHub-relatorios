# Diário de Bordo – Lude Ribeiro

**Disciplina:** Gestão de Configuração e Evolução de Software (GCES)  
**Equipe:** GovHub  
**Projeto de Software Livre:** GovHub-br

---

## Sprint 0 – 01/09/2025 a 10/09/2025

### Resumo da Sprint (S0)

A Sprint inicial foi dedicada à compreensão do projeto GovHub-br, com foco na análise de sua proposta, estudo das tecnologias empregadas e configuração completa do ambiente de desenvolvimento.

### Atividades Realizadas (S0)

| Data  | Atividade                                 | Categoria     | Referência                                              | Status       |
| ----- | ----------------------------------------- | ------------- | ------------------------------------------------------- | ------------ |
| 02/09 | Análise inicial do repositório GovHub-br  | Estudo        | <https://github.com/GovHub-br/data-application-gov-hub> | ✅ Concluído |
| 03/09 | Estudo da documentação oficial do projeto | Estudo        | README.md e documentação oficial                        | ✅ Concluído |
| 06/09 | Configuração do ambiente via Docker       | Implementação | docker-compose.yml                                      | ✅ Concluído |

### Principais Avanços (S0)

-   Configuração e execução bem-sucedida do ambiente local.
-   Entendimento preliminar da proposta do GovHub-br e de seu potencial impacto.

### Principais Desafios (S0)

-   A variedade de tecnologias utilizadas (Airflow, dbt, Superset) demandou tempo adicional para assimilação.
-   Compreensão inicial do escopo e aplicabilidade do projeto.

### Conhecimentos Adquiridos (S0)

-   Introdução prática ao Apache Airflow e suas aplicações.
-   Consolidação do entendimento sobre manipulação e fluxo de dados no contexto do projeto.

### Planejamento Pessoal para a Próxima Sprint (S0)

-   [ ] Realizar uma análise de GCES aplicada ao projeto GovHub.
-   [ ] Assumir uma _issue_ relacionada à melhoria de parâmetros de GCES no repositório.
-   [ ] Trabalhar em uma _pipeline_ para aprofundar o conhecimento em GitHub Actions.
-   [ ] Aprofundar a compreensão do funcionamento geral do GovHub e de sua proposta.

### Considerações Finais (S0)

O projeto se apresenta como uma oportunidade desafiadora e promissora, capaz de ampliar tanto a experiência técnica quanto a visão prática sobre software livre e governança de dados.

---

## Sprint 1 – 11/09/2025 a 20/09/2025

### Resumo da Sprint (S1)

Nesta sprint, executei todas as atividades planejadas anteriormente, com foco em aplicar conceitos de GCES ao projeto GovHub-br, assumir responsabilidades em _issues_ e pipelines, além de aprofundar a compreensão sobre o funcionamento e proposta do sistema.

### Atividades Realizadas (S1)

| Data  | Atividade                                                         | Categoria      | Referência                                                                | Status       |
| ----- | ----------------------------------------------------------------- | -------------- | ------------------------------------------------------------------------- | ------------ |
| 12/09 | Análise de GCES aplicada ao projeto GovHub-br                     | Estudo/Análise | [Documento](../GCES/checklist.md)                                         | ✅ Concluído |
| 14/09 | Assumi a _issue_ para aprimorar parâmetros de GCES (documentação) | Documentação   | [Issue](https://github.com/GCES-GovHub-2025-2/GovHub-relatorios/issues/6) | ✅ Concluído |
| 16/09 | Contribuição em uma _pipeline_ com GitHub Actions                 | Implementação  | workflows/.github                                                         | ✅ Concluído |
| 18/09 | Estudo aprofundado do funcionamento e proposta do GovHub-br       | Estudo         | Documentação oficial e exploração do código                               | ✅ Concluído |

### Principais Avanços (S1)

-   Conduzi uma análise prática dos aspectos de GCES no projeto, juntamente com a [Leticia Aires](https://github.com/LeticiaAires)
-   Contribuí diretamente para a melhoria do repositório por meio da criação de _issues_ para alcançar os parâmetros necessários para GCES.
-   Comecei a estudar e implementar a configuração e utilização de pipelines com GitHub Actions.
-   Ampliei o entendimento sobre os objetivos do GovHub-br e sua aplicabilidade.

### Principais Desafios (S1)

-   Adaptação às práticas de contribuição em comunidade de software livre.
-   Necessidade de aprender e compreender as pipelines e o Github Actions.

### Conhecimentos Adquiridos (S1)

-   Aplicação prática de princípios de GCES em um projeto real.
-   Experiência inicial com GitHub Actions para integração contínua.
-   Maior clareza sobre a proposta de valor do GovHub-br.

### Planejamento Pessoal para a Próxima Sprint (S1)

-   [ ] Assumir novas _issues_ de maior complexidade.
-   [ ] Aprimorar práticas de documentação no repositório.
-   [ ] Aprofundar conhecimentos em dbt e Superset dentro do contexto do GovHub-br.
-   [ ] Explorar métricas de qualidade de software e sua aplicação ao projeto.

### Considerações Finais (S1)

Esta sprint marcou a transição entre o estudo inicial e as primeiras contribuições práticas. A experiência trouxe segurança para avançar em atividades mais complexas e contribuiu para uma visão mais clara do papel do GovHub-br no ecossistema de dados públicos.

---

## Sprint 2 – 21/09/2025 a 05/10/2025

### Resumo da Sprint (S2)

Nesta sprint, o foco foi a implementação prática dos parâmetros de **Gerência de Configuração de Software (GCES)** no projeto **GovHub-br**, com a criação de um **checklist de conformidade**, integração de automações e início da padronização de práticas de versionamento e entrega contínua.

### Atividades Realizadas (S2)

| Data  | Atividade                                            | Categoria     | Referência                                   | Status       |
| ----- | ---------------------------------------------------- | ------------- | -------------------------------------------- | ------------ |
| 23/09 | Elaboração do checklist de GCES para o projeto       | Documentação  | [Checklist GCES](../GCES/checklist.md)       | ✅ Concluído |
| 25/09 | Análise e ajustes na estrutura de versionamento      | Implementação | git log / tags                               | ✅ Concluído |
| 27/09 | Configuração de workflows de CI com GitHub Actions   | Implementação | .github/workflows                            | ✅ Concluído |
| 02/10 | Integração do SonarQube e testes automatizados       | Implementação | sonar-project.properties / workflows         | ✅ Concluído |
| 04/10 | Validação dos arquivos de ambiente e containerização | Implementação | Dockerfile, docker-compose.yml, .env.example | ✅ Concluído |

### Principais Avanços (S2)

-   Estruturação inicial da **automação de build, testes e linting** via GitHub Actions.
-   Integração com **SonarQube** para análise de qualidade do código.
-   Criação do **checklist de conformidade GCES**, garantindo rastreabilidade e padronização.
-   Definição das práticas de versionamento e estrutura de repositório.

### Principais Desafios (S2)

-   Configuração detalhada das ferramentas de CI/CD e integração com SonarQube.
-   Adaptação das práticas teóricas de GCES à estrutura real do GovHub-br.

### Conhecimentos Adquiridos (S2)

-   Aplicação prática dos princípios de **CI/CD e GCES**.
-   Uso de **SonarQube** para análise contínua de qualidade.
-   Definição de pipelines e versionamento semântico.

### Planejamento Pessoal para a Próxima Sprint (S2)

-   [ ] Implementar templates de issues e PRs.
-   [ ] Documentar os padrões de código e estrutura do projeto.
-   [ ] Automatizar o versionamento e releases.
-   [ ] Realizar limpeza e padronização completa do repositório.

### Considerações Finais (S2)

A sprint consolidou a base da gerência de configuração e pavimentou o caminho para a automatização e padronização completa do projeto GovHub-br.

---

## Sprint 3 – 06/10/2025 a 20/10/2025

### Resumo da Sprint (S3)

Esta sprint representou a conclusão integral da **Gerência de Configuração e Evolução de Software** do projeto. Foram implementados templates, padrões, guias de contribuição, automações e validações, atingindo 100% dos critérios de GCES e garantindo um repositório profissional, limpo e sustentável.

### Atividades Realizadas (S3)

| Data  | Atividade                                       | Categoria     | Referência                                               | Status       |
| ----- | ----------------------------------------------- | ------------- | -------------------------------------------------------- | ------------ |
| 08/10 | Criação dos templates de Issues e PRs (YAML)    | Documentação  | .github/ISSUE_TEMPLATE/\*.yml / PULL_REQUEST_TEMPLATE.md | ✅ Concluído |
| 10/10 | Criação dos guias de padrões de código          | Documentação  | docs/standards/\*                                        | ✅ Concluído |
| 12/10 | Documentação da estrutura e fluxo do projeto    | Documentação  | docs/structure.md / docs/architecture.md                 | ✅ Concluído |
| 14/10 | Implementação de Dependabot e CodeQL            | Implementação | .github/dependabot.yml / .github/workflows/codeql.yml    | ✅ Concluído |
| 17/10 | Limpeza de arquivos temporários e revisão final | Manutenção    | .gitignore / limpeza de arquivos temporários             | ✅ Concluído |
| 19/10 | Preparação do PR final                          | Integração    | feature/gerencia-configuracao → develop                  | ✅ Concluído |

### Principais Avanços (S3)

-   Implementação completa da **Gerência de Configuração**, cobrindo versionamento, automação, segurança e padrões.
-   Criação de **templates de issues, PRs e documentação**, promovendo padronização colaborativa.
-   Estabelecimento de **boas práticas de código**, documentação e controle de qualidade.
-   Limpeza e reestruturação do repositório, com eliminação de arquivos temporários e redundantes.

### Principais Desafios (S3)

-   Garantir consistência entre documentação, automação e versionamento.
-   Conciliar clareza técnica com acessibilidade para contribuidores futuros.

### Conhecimentos Adquiridos (S3)

-   Criação de **templates YAML estruturados** para issues e PRs.
-   Configuração de **análises automatizadas de segurança (CodeQL, Dependabot)**.
-   Estruturação de documentação modular e manutenível.
-   Aplicação completa dos princípios de **GCES** em um projeto real.

### Planejamento Pessoal Pós-Sprint (S3)

-   [ ] Criar PR final e solicitar aprovação.
-   [ ] Configurar proteção de branches.
-   [ ] Aplicar as práticas consolidadas em outros repositórios.

### Considerações Finais (S3)

A sprint final marcou a **entrega completa da gerência de configuração do GovHub-br**, atingindo todos os requisitos definidos. O repositório agora reflete maturidade técnica, automação robusta e documentação exemplar — uma base sólida para evolução contínua e contribuições da comunidade.

---

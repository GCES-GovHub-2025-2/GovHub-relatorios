# Diário de Bordo – \[Mateus Henrique Queiroz Magalhães Sousa]

**Disciplina:** \[Gestão de Confinguração e Evolução de Software]
**Equipe:** \[GovHub]
**Comunidade/Projeto de Software Livre:** \[GovHubbr – Análise de Gastos Públicos com Inteligência Artificial]

---
    
## Sprint 0 – \[01/09 - 15/09]

### Resumo da Sprint

Essa sprint foi focada em organizar a equipe, criar o fork e o repositório, além de estudar as políticas de contribuição e práticas de GCES do GovHub. Realizamos a configuração do ambiente local, documentando os problemas e aprendizados. O projeto mostrou-se ser uma solução moderna para gestão de dados públicos, utilizando tecnologias como Apache Airflow, dbt, Jupyter e Superset.

### Atividades Realizadas

| Data  | Atividade                                   | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status    |
| ----- | ------------------------------------------- | --------------------------------- | --------------- | --------- |
| 01/09 | Configuração inicial do ambiente            | Código                            | [Link](http://gov-hub.io/documentacao/instalacao/)               | Concluído |
| 03/09 | Leitura e estudo da documentação do projeto | Estudo                            | [Link](http://gov-hub.io/documentacao/instalacao/)    | Concluído |
| 09/09 | Estudo do CI/CD do GovHub     | Estudo                         | [Link](https://gitlab.com/lappis-unb/gest-odadosipea/app-lappis-ipea/-/blob/main/.gitlab-ci.yml?ref_type=heads)   | Concluído |
| 09/09 | Documentação do GCS relacionado ao pipeline do GovHub     | Doc                         | [Link](https://docs.google.com/document/d/1gwo-WKB09nKjJ5ghYFihoAGSMAReoC442PUmTbsKAY0/edit?tab=t.0)   | Concluído |

### Maiores Avanços

* Consegui rodar o ambiente.
* Organização inicial da equipe e do repositório acadêmico.
* Entedimento maior sobre CI/CD
* Aprendi sobre a arquitetura de dados moderna com Airflow para orquestração, dbt para transformação, e Superset para visualização.
### Maiores Dificuldades

* Demorei um pouco para configurar o ambiente pela falta das variáveis ambientes.
* O projeto envolve diversas tecnologias integradas, o que dificultou a compreensão e o entendimento completo de sua estrutura.

### Aprendizados

* Ganhei conhecimento sobre o funcionamento e organização de pipelines no GitLab CI/CD e como isso pode ser migrado/adaptado para o GitHub Actions.
* Importância de boas práticas de GCES, como padronização de contribuições, e automação de qualidade.
* Entendi os conceitos de camadas Bronze, Silver e Gold para organização de dados.

### Plano Pessoal para a Próxima Sprint

* [x] Contribuir com alguma documentação.
* [x] Participar da revisão de código de um colega, garantindo a aplicação das boas práticas de GCES.
* [ ] Estudar mais sobre Github Actions para replicar/melhorar as etapas do pipeline.
* [x] Estudar mais sobre as ferramentas Jupyter, Superset e Airflow para análise e visualização.

---

## Sprint 1 – [11/09 - 24/09]

### Resumo da Sprint

Inicialmente, o objetivo era contribuir com issues relacionadas a pipelines. No entanto, como já havia pessoas trabalhando nessas tarefas, assumi a issue relacionada à criação de uma DAG no Airflow. Durante a sprint, estudei sobre DAGs, a arquitetura do Airflow e participei da separação das tarefas que cada membro da equipe deveria realizar. O foco foi no aprendizado prático sobre orquestração de tarefas e ingestão de dados.  

### Atividades Realizadas

| Data  | Atividade                                        | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status    |
| ----- | ------------------------------------------------ | --------------------------------- | --------------- | --------- |
| 12/09 | Estudo sobre DAGs e funcionamento do Airflow     | Estudo                            | [Link](https://airflow.apache.org/docs/apache-airflow/stable/core-concepts/dags.html) | Concluído |
| 18/09 | Discussão e divisão das tarefas da equipe        | Discussão                         | -               | Concluído |
| 23/09 | Criação inicial da DAG de ingestão de emendas parlamentares | Código | [Link](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/blob/feat/dag-ingestao-emendas/airflow_lappis/dags/data_ingest/portal_transparencia/emendas_parlamentares_dag.py) | Em andamento |

### Maiores Avanços

* Consegui criar uma DAG em conjunto com membros da equipe para ingestão de dados de emendas parlamentares, ainda que ela não esteja completamente finalizada.  
* Aprofundei o entendimento sobre DAGs no Airflow e como elas estruturam workflows de dados.  
* Ganhei mais experiência prática com o desenvolvimento em Python integrado ao Airflow.  

### Maiores Dificuldades

* Foi complicado compreender o funcionamento completo de uma DAG, especialmente o fluxo de dependências entre as tasks.  
* Tive dificuldade em entender melhor como os **operators** do Airflow funcionam e como integrá-los de forma adequada com funções Python.  

### Aprendizados

* Entendi a importância da modularização para manter o código da DAG limpo e escalável.  
* Tive contato prático com a ingestão de dados externos (API) e inserção em banco de dados com Postgres.  
* Percebi a importância de padronizar as DAGs com a arquitetura do projeto para facilitar manutenção e colaboração.  

### Plano Pessoal para a Próxima Sprint

* [x] Lapidar a DAG criada, deixando-a mais modular e integrada ao restante do projeto.  
* [x] Documentar o processo de criação da DAG, descrevendo as decisões tomadas e os aprendizados.  

---

## Sprint 2 – [25/09 - 08/10]

### Resumo da Sprint

A sprint foi dedicada ao desenvolvimento e refatoração da DAG de ingestão de dados de emendas parlamentares. A DAG foi modularizada e adaptada para seguir o padrão e arquitetura do código já existente no projeto. Durante o processo, também foi necessário integrar o cliente da API com a DAG, garantindo que a ingestão ocorresse de forma compatível com os componentes da aplicação.

---

### Atividades Realizadas

| Data    | Atividade                                                  | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status     |
|---------|------------------------------------------------------------|-----------------------------------|-----------------|------------|
| 03/10   | Refatoração da DAG de ingestão de emendas parlamentares    | Código                            | [Commit](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/commit/c63196c204357ed05b835e4e6bc31d12b98ca654) | Em andamento |
| 04/10   | Refatoração da DAG de ingestão de emendas parlamentares    | Código                            | [Commit](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/commit/c63196c204357ed05b835e4e6bc31d12b98ca654) | Em andamento 
| 06/10   | Finalização da DAG de ingestão de emendas parlamentares    | Código                            | [Commit](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/commit/4ff07ddc1c59c555e7f1b2523aa2b4983ddeed95) | Concluída

---

### Maiores Avanços

* Modularizei a DAG para integrá-la ao padrão de organização do projeto, tornando o código mais limpo e reutilizável.  
* Realizei a integração do cliente da API com a DAG.
* Estabeleci uma base sólida para facilitar a manutenção e evolução futura da DAG, com estrutura de pastas e funções coerentes com o restante do repositório.

---

### Maiores Dificuldades

* A API de emendas parlamentares retornava dados duplicados, o que causava problemas na consistência dos dados durante a inserção no banco de dados.  
* A integração do cliente da API com a DAG exigiu ajustes e entendimento detalhado tanto do cliente quanto da arquitetura atual da ingestão.  

---

### Aprendizados

* Aprendi como a modularização contribui para a escalabilidade de DAGs no Airflow, facilitando a manutenção e leitura do código.  
* Compreendi melhor os desafios reais de integração entre componentes distintos em pipelines de dados (API + DAG + banco).  

---

### Plano Pessoal para a Próxima Sprint

* [ ] Iniciar o tratamento de dados, colocando os dados no modelo bronze  
* [ ] Criar testes unitários para as DAGs.
* [ ] Documentar o funcionamento da DAG, incluindo possíveis erros da API e formas de tratá-los.  

## Sprint 3 – [09/10 - 22/10]

### Resumo da Sprint

A sprint foi dedicada ao desenvolvimento do modelo Bronze de Emendas Parlamentares no DBT, estruturando todo o fluxo necessário para ingestão, padronização e documentação dos dados provenientes do Portal da Transparência.
Os testes foram estruturados, mas serão concluídos e executados apenas na Sprint 4, conforme planejamento.

---

### Atividades Realizadas

| Data    | Atividade                                                  | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status     |
|---------|------------------------------------------------------------|-----------------------------------|-----------------|------------|
| 22/10   | Atualização do sources.yml com a nova fonte portal_transparencia    | Modelagem                           | [Commit](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/commit/a3ea2e4f25ffc7290588dcfd6f6e8d41ed54ee6d) | Concluído |
| 22/10   | Criação do modelo Bronze emendas.sql com cast, limpeza e normalização    | Modelagem/DBT                          | [Commit](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/commit/d5a4aae032e41a54417d8fa8275805b789117860) | Concluído 
| 22/10   | Estrutura inicial de testes unitários para Sprint 4 (não concluídos ainda)    | Testes                           | [Commit]() | Em andamento
| 22/10   | Criação da documentação detalhada do modelo bronze    | Doc                           | [Commit](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/commit/9ca9c829fe765b0766885ce6831179607f97996a) | Concluído

---

### Maiores Avanços

* Construção completa do modelo Bronze com tipagens, normalização e tratamento de valores financeiros brasileiros.
* Documentação DBT altamente detalhada, incluindo descrições e testes declarativos.
* Inclusão estruturada da nova fonte no projeto DBT.

---

### Maiores Dificuldades

* Interpretar dados complexos da API do Portal da Transparência, especialmente campos financeiros em formato BR.
* Garantir precisão numérica (numeric(15,2)) e consistência entre valores empenhados, liquidados e pagos.
* Estruturar corretamente a documentação para que ficasse clara e completa sem redundância.
* Mapear todos os nomes originais para nomes padronizados DBT com consistência.

---

### Aprendizados

* O uso de modelos Bronze e padronizações iniciais fortalece significativamente a governança de dados.
* A limpeza de valores financeiros exige cuidados extras para evitar.
* Uma documentação bem escrita facilita o onboard de qualquer pessoa que venha trabalhar nos modelos.


---

### Plano Pessoal para a Próxima Sprint

* [x] Finalizar e validar os testes que foram planejados.
* [x] Criar documentação complementar sobre execução local e fluxo de ingestão.
* [] Ajudar na definição das próximas camadas Silver/Gold para emendas parlamentares. 


## Sprint 4 – [23/10 - 19/11]

### Resumo da Sprint

A sprint foi dedicada a implementação e validação completa da camada de testes relacionada ao modelo DBT de emendas parlamentares. Após a finalização do modelo bronze e sua documentação estruturada

---

### Atividades Realizadas

| Data    | Atividade                                                  | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status     |
|---------|------------------------------------------------------------|-----------------------------------|-----------------|------------|
| 05/11   | Desenvolvimento da suíte com 12 testes para o modelo bronze   | Testes                           | [Commit](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/commit/ceee0b02cccb3b9bebe2c4bcd0a1b2707a1510f9) | Concluído |


---

### Maiores Avanços

* Criação de uma suíte de testes altamente completa, cobrindo toda a lógica do modelo.
* Inclusão estruturada da nova fonte no projeto DBT.

---

### Maiores Dificuldades

* Garantir precisão e limites de numeric(15,2) nos testes.
* Simular múltiplos cenários em testes unitários para cobrir casos reais da API do Portal da Transparência.
---

### Aprendizados

* A construção de uma suíte sólida de testes é essencial para garantir a confiabilidade de um pipeline de dados.
* A combinação entre teste unitário + lógica simulada + revisão de esquema aumenta a maturidade do projeto.


---

### Plano Pessoal para a Próxima Sprint

* [ ] Apoiar a criação das camadas Silver de Emendas parlamentares
* [ ] Expandir a cobertura de testes

# Sprint 5 – [20/12 – 03/12]

## Resumo da Sprint

Nesta sprint, desenvolvi a DAG `api_executor_especial_dag` no Airflow para automatizar a ingestão de executores especiais a partir da API do TransfereGov. As atividades envolveram integração com Postgres, paralelização via chunking e tratamento de dados com deduplicação e timestamp. A issue relacionado a ingestão é : [Issue #41](https://github.com/GovHub-br/data-application-gov-hub/issues/41)
do repositório principal.
## Atividades Realizadas

| Data  | Atividade                                                            | Tipo  | Link/Referência | Status   |
|-------|----------------------------------------------------------------------|-------|-----------------|----------|
| 01/12 | Desenvolvimento do cliente `ClienteTransfereGov` para extração`api_executor_especial_dag`                            | Código| [Commit 2c4fe9b](https://github.com/GovHub-br/data-application-gov-hub/commit/2c4fe9b299d00aac2df460576728ebaae2da191a)            | Concluído|
| 01/12 | Desenvolvimento da DAG de executor especial para extração        | Código|    [Commit 7ce4e5e](https://github.com/GovHub-br/data-application-gov-hub/commit/7ce4e5e3c1b7216f6ac7e60f64d2e647d4a64fdd)            | Concluído|
| 02/12 | Abertura do PR para das alterações feitas               | Código| [PR-46](https://github.com/GovHub-br/data-application-gov-hub/pull/46)            | Concluído|



## Maiores Avanços

- DAG totalmente funcional com ingestão paralela de executores especiais.
- Superação do Gargalo de Performance: Implementação bem-sucedida da estratégia de paralelismo (fan-out do Airflow) para processar os ~48.000 IDs de Planos de Ação. A divisão em chunks de 200 e a execução paralela de cada chunk reduziram drasticamente o tempo total de execução.


## Maiores Dificuldades

- A complexidade da API TransfereGov exigiu o desenvolvimento de funções de cliente personalizadas para lidar com paginação da entidade executor_especial.
- Paginação correta da API para garantir que todos os executores fossem buscados.
- Superar o problema do gargalo na hora de fazer as consultas -> requisições -> inserções na dag.

## Aprendizados

- Importância de dividir grandes volumes de dados em chunks para processamento eficiente.
- Como enriquecer dados com timestamps e deduplicar antes da inserção.
- Uso de logging detalhado para rastrear falhas em pipelines automáticos.

### Plano Pessoal para a Próxima Sprint

* [] Começar a desenvolvimento da camada bronze de Executor Especial
* [] Desenvolver a camada prata para emendas parlamentares

### Resumo das Contribuições Individuais 

| Sprint   | Contribuição / Descrição                                                         | Link do Commit / PR                                                                 |
|----------|----------------------------------------------------------------------------------|-------------------------------------------------------------------------------------|
| Sprint 1 | Planejamento inicial da DAG de ingestão de emendas parlamentares                | (sem commits nesta sprint)                                                         |
| Sprint 2 | Implementação inicial da DAG de ingestão de emendas parlamentares                | [Commit 1](https://github.com/GovHub-br/data-application-gov-hub/commit/b8f6a04e0dd583f7c98509b7ff2f07b2200b7880) |
| Sprint 2 | Refatoração da DAG de emendas parlamentares – melhorias estruturais              | [Commit 2](https://github.com/GovHub-br/data-application-gov-hub/commit/ecaf6bbb331819cbffe1ad47fb15a0d92c99b93d) |
| Sprint 2 | Refatoração final e ajustes da DAG de emendas parlamentares                      | [Commit 3](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/commit/4ff07ddc1c59c555e7f1b2523aa2b4983ddeed95) |
| Sprint 3 | Atualização do arquivo sources.yml com nova fonte do Portal da Transparência    | [Commit 4](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/commit/a3ea2e4f25ffc7290588dcfd6f6e8d41ed54ee6d) |
| Sprint 3 | Criação completa do modelo DBT Bronze para emendas (emendas.sql)                 | [Commit 5](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/commit/d5a4aae032e41a54417d8fa8275805b789117860) |
| Sprint 3 | Documentação detalhada do modelo Bronze                                          | [Commit 6](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/commit/9ca9c829fe765b0766885ce6831179607f97996a) |
| Sprint 4 | Suíte de 12 testes unitários para o modelo Bronze                                | [Commit 7](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/commit/ceee0b02cccb3b9bebe2c4bcd0a1b2707a1510f9) |
| Sprint 4 | Abertura do Pull Request com melhorias e ajustes no modelo de testes e DAG     | [PR 12](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/12)      |
| Sprint 5 | Implementação do cliente ClienteTransfereGov para ingestão de executores especiais | [Commit 8](https://github.com/GovHub-br/data-application-gov-hub/commit/2c4fe9b299d00aac2df460576728ebaae2da191a) |
| Sprint 5 | Desenvolvimento completo da DAG api_executor_especial_dag                        | [Commit 9](https://github.com/GovHub-br/data-application-gov-hub/commit/7ce4e5e3c1b7216f6ac7e60f64d2e647d4a64fdd) |
| Sprint 5 | Abertura do Pull Request com todas as implementações da Sprint                   | [PR 46](https://github.com/GovHub-br/data-application-gov-hub/pull/46)              |

### Com exceção dos commits/PRs da Sprint 5 foram feitos no repositório de equipe, enquanto os da sprint 5 foram feitos no repositório Oficial do Github
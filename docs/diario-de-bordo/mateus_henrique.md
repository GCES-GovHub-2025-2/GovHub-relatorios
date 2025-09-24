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

* [ ] Contribuir com alguma documentação.
* [ ] Participar da revisão de código de um colega, garantindo a aplicação das boas práticas de GCES.
* [ ] Estudar mais sobre Github Actions para replicar/melhorar as etapas do pipeline.
* [ ] Estudar mais sobre as ferramentas Jupyter, Superset e Airflow para análise e visualização.

---

## Sprint 1 – [11/09 - 24/09]

### Resumo da Sprint

Inicialmente, o objetivo era contribuir com issues relacionadas a pipelines. No entanto, como já havia pessoas trabalhando nessas tarefas, assumi a issue relacionada à criação de uma DAG no Airflow. Durante a sprint, estudei sobre DAGs, a arquitetura do Airflow e participei da separação das tarefas que cada membro da equipe deveria realizar. O foco foi no aprendizado prático sobre orquestração de tarefas e ingestão de dados.  

### Atividades Realizadas

| Data  | Atividade                                        | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status    |
| ----- | ------------------------------------------------ | --------------------------------- | --------------- | --------- |
| 12/09 | Estudo sobre DAGs e funcionamento do Airflow     | Estudo                            | [Link](https://airflow.apache.org/docs/apache-airflow/stable/core-concepts/dags.html) | Concluído |
| 18/09 | Discussão e divisão das tarefas da equipe        | Discussão                         | -               | Concluído |
| 23/09 | Criação inicial da DAG de ingestão de emendas parlamentares | Código | [Link](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/blob/feat/dag-ingestao-emendas/airflow_lappis/dags/data_ingest/emendas_parlamentares/emendas_parlamentares_dag.py) | Em andamento |

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

* [ ] Lapidar a DAG criada, deixando-a mais modular e integrada ao restante do projeto.  
* [ ] Documentar o processo de criação da DAG, descrevendo as decisões tomadas e os aprendizados.  
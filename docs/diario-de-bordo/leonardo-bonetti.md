# Diário de Bordo – Leonardo Bonetti

**Disciplina:** GCES

**Equipe:** GovHub

**Comunidade/Projeto de Software Livre:** GovHub-br

---

## Sprint 0 – 01/09/2025 – 10/09/2025

### Resumo da Sprint

Durante a Sprint 0 me dediquei a estudar o GovHub, suas tecnolgias e documentação já que não estva familiarizado com o mesmo ou o que usava. E também gastei um tempo para executar o ambiente de desenvolvimento para se preprara para atividades futuras.

### Atividades Realizadas

| Data | Atividade | Tipo | Link/Referência | Status |
|------|-----------|------|-----------------|---------|
| 04/09 | Primeira verificação do repositório | Estudo | [Link](https://github.com/GovHub-br/data-application-gov-hub) | Concluído |
| 05/09 | Estudo da documentação disponível | Estudo | README.md | Concluído |
| 05/09 | Execução do ambiente de desenvolvimento | Código | - | Concluído |
| 08/09 | Estudo do Apache AirFlow | Estudo | [Link](https://airflow.apache.org/docs/) | Concluído |

### Maiores Avanços

* Entendi melhor sobre o GovBrHub e seu funcionamento.
* Tenho na maquina o ambiente da aplicação para desenvolver
* Consegui melhorar o meu entendimento das ferramentas usadas, principalmente do apache Airflow.

### Maiores Dificuldades

* Algumas partes do código ainda exigem um olhar mais dedicado por serem mais complexas
* Como há muitas coisas a quais não estou familiriazado, a execução ficou mais complexa de se entender.

### Aprendizados

* Aprendi a organização e execulção de um volume imenso de dados pode ser feita
* Vi como fazer uma contribuição de um projeto open-source de qqcordo com as políticas definidas

### Plano Pessoal para a Próxima Sprint

* [ ] Verificar pontos a serem melhorados da documentação
* [ ] Fazer uma contribuição ao projeto
* [ ] Estudar mais api´s publicas para a extração de dados e como lidar com os mesmo.

## Sprint 1 – 11/09/2025 – 24/09/2025

### Resumo da Sprint

Nesta sprint, meu foco foi realizar minha primeira contribuição de código para o projeto. Estudei a API de dados abertos da Câmara dos Deputados e, com base nisso, desenvolvi uma nova DAG no Airflow para a ingestão de dados de deputados. O trabalho foi realizado em uma branch separada para garantir a organização do versionamento.

### Atividades Realizadas

| Data | Atividade | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status |
| --- | --- | --- | --- | --- |
| 20/09 | Criação de DAG exemplo para praticar o Airflow | Estudo | - | Concluído |
| 22/09 | Estudo da API de dados públicos da Câmara dos Deputados | Estudo | [API Câmara](https://dadosabertos.camara.leg.br/swagger/api.html) | Concluído |
| 23/09 | Desenvolvimento da DAG de ingestão de dados de deputados | Código | [Branch específica](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/tree/dag_deputados) | Concluído |
| 24/09 | Revisão do código para melhoria do DAG e depois Merge Request | Código | - | Pendente |

### Maiores Avanços

* **Primeira contribuição de código:** Consegui aplicar os conhecimentos de Airflow para criar um pipeline de dados funcional, o que representa um avanço significativo no meu envolvimento com o projeto.
* **Compreensão prática do fluxo de dados:** Desenvolver a DAG me deu uma visão clara de como os dados são extraídos de uma fonte externa e preparados para as próximas etapas do pipeline no GovHub.

### Maiores Dificuldades

* **Entender a estrutura das DAGs:** A princípio, tive dificuldade para compreender a estrutura e as melhores práticas para a criação de DAGs no Airflow, exigindo mais tempo de estudo.

### Aprendizados

* **Desenvolvimento de pipelines com Airflow:** Aprendi na prática a criar, organizar e testar uma DAG para orquestração de dados.
* **Versionamento de código em projetos colaborativos:** A criação de uma branch separada para a nova funcionalidade reforçou a importância de um fluxo de trabalho organizado com Git.

### Plano Pessoal para a Próxima Sprint

* [ ] Submeter um Pull Request com a DAG desenvolvida para revisão dos colegas.
* [ ] Criar testes para a nova DAG de ingestão.
* [ ] Iniciar o estudo de uma nova fonte de dados para uma futura contribuição.


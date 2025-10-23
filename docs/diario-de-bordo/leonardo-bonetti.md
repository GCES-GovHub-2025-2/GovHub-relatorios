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

## Sprint 2– 24/09/2025 – 07/10/2025

### Resumo da Sprint

Nesta sprint, meu foco foi tentar fazer o PR da DAG de deputados e resolver um bug que impedia salvar corretamente os dados e implementar os testes

### Atividades Realizadas

| Data | Atividade | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status |
| --- | --- | --- | --- | --- |
| 29/09 | Estudo dos testes em python | Estudo | - | Concluído |
| 02/10 | Implementação de testes na DAG de deputados | Código | - | Concluído |
| 01/10-08/10 | Tentaiva de consertar o bug no salvamento de deputados em diferentes tempos de legislaturas | Código | [Branch específica](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/tree/dag_deputados) | Em andamento |

### Maiores Avanços

### Maiores Dificuldades

* **Garantir a integridade dos dados** A princípio, tive dificuldadde resolver os problemas de manter os deputados salvos pela DAG

### Aprendizados

* **Teste em Python:** Consegui implementar teste que passaram usando jester, o que melhorou a minha rapidez de realiza-os para outras sprints

### Plano Pessoal para a Próxima Sprint

* [ ] Resolver o bug no salvamento
* [ ] Começar a implementação do modelo bronze para a tabela deputados

## Sprint 3 – 08/10/2025 – 21/10/2025

### Resumo da Sprint

Nesta sprint, o foco principal foi a resolução definitiva do bug que impedia o salvamento correto dos dados de deputados de diferentes legislaturas. Após corrigir o problema e refatorar o código, todo o trabalho desenvolvido na DAG de deputados foi submetido para revisão através de um Pull Request, marcando um passo importante na contribuição para o projeto.

### Atividades Realizadas

| Data | Atividade | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status |
| --- | --- | --- | --- | --- |
| 10/10 | Análise e correção final do bug no salvamento de dados das legislaturas | Código | [Branch específica](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/tree/dag_deputados) | Concluído |
| 17/10 | Refatoração e limpeza do código da DAG para adequação aos padrões do projeto | Código | [Branch específica](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/tree/dag_deputados) | Concluído |
| 18/10 | Revisão final dos testes e preparação para o Pull Request | Código | [Branch específica](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/tree/dag_deputados) | Concluído |
| 19/10 | Abertura e submissão do Pull Request para a DAG de deputados | Código/Discussão | [Pull Request #11](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/11) | Concluído |
| 20/10 | Início do planejamento da tabela bronze para deputados | Código/Discussão | [Pull Request #11](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/11) | Concluído |

### Maiores Avanços

* **Resolução de bug complexo:** Consegui identificar e corrigir a falha na lógica de salvamento de dados, garantindo a integridade e a correta persistência das informações coletadas pela DAG.
* **Submissão do primeiro Pull Request:** A finalização e submissão da DAG de deputados para revisão pela equipe representa a conclusão de um ciclo de desenvolvimento completo, desde o estudo até a entrega da funcionalidade.

### Maiores Dificuldades

* **Depuração do fluxo de dados:** Entender exatamente em que ponto do pipeline os dados estavam sendo sobrescritos ou perdidos exigiu um esforço considerável de depuração e testes incrementais.

### Aprendizados

* **Processo de Code Review:** Aprendi na prática como funciona o processo de submeter um PR em um projeto colaborativo, incluindo a importância de descrever claramente as mudanças.
* **Técnicas de depuração em pipelines de dados:** A dificuldade com o bug me forçou a aprimorar minhas habilidades de debugging em Python e Airflow para rastrear problemas em fluxos de dados.

### Plano Pessoal para a Próxima Sprint

* [ ] Iniciar a implementação do modelo na camada bronze para a tabela de deputados.
* [ ] Discutir com o par sobre a implementação do código.


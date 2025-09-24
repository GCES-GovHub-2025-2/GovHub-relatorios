# Diário de Bordo – Gabriel Scheidt

**Disciplina:** GCES

**Equipe:** GovHub

**Comunidade/Projeto de Software Livre:** GovHub-br

---

## Sprint 0 – 01/09/2025 – 10/09/2025

### Resumo da Sprint

Durante esta sprint inicial, estudei o GovHub-br, uma iniciativa brasileira de integração de dados governamentais. Dediquei tempo significativo à compreensão da arquitetura do sistema, exploração das tecnologias utilizadas e preparação do ambiente de desenvolvimento. 

### Atividades Realizadas

| Data | Atividade | Tipo | Link/Referência | Status |
|------|-----------|------|-----------------|---------|
| 01/09 | Análise inicial do repositório GovHub-br | Estudo | https://github.com/GovHub-br/data-application-gov-hub | ✅ Concluído |
| 02/09 | Estudo aprofundado da documentação | Estudo | README.md e e-book oficial | ✅ Concluído |
| 03/09 | Investigação da arquitetura Medallion | Estudo | Documentação técnica do projeto | ✅ Concluído |
| 05/09 | Setup completo do ambiente Docker | Implementação | docker-compose.yml | ✅ Concluído |

### Maiores Avanços

* **Domínio conceitual do projeto**: Desenvolvi uma compreensão sólida do GovHub-br.
* **Ambiente completamente funcional**: Estabeleci com sucesso toda a infraestrutura de desenvolvimento local utilizando containerização Docker.
* **Apropriação do stack tecnológico**: Me familiarizei com ferramentas de ponta para engenharia de dados, incluindo Airflow, dbt e Superset.

### Maiores Dificuldades

* **Densidade informacional**: O volume extenso de documentação técnica e conceitual exigiu organização cuidadosa do estudo.
* **Complexidade arquitetural**: Entender como os diferentes componentes se comunicam na prática requer experiência hands-on adicional.

### Aprendizados

* **DevOps para dados**: Aprendi como containerização simplifica deployment de stacks de dados complexos.
* **Governança de dados públicos**: Compreendi questões de transparência, privacidade e democratização de informações governamentais.

### Plano Pessoal para a Próxima Sprint

* [ ] Implementar melhorias na documentação ou resolver issues identificados
* [ ] Fazer deep dive nos modelos dbt para entender transformações específicas
* [ ] Mapear detalhadamente o fluxo de dados entre os sistemas governamentais

### Reflexões Pessoais

Este primeiro contato com o GovHub-br foi revelador sobre o potencial transformador da tecnologia no setor público. A possibilidade de contribuir para um projeto que pode impactar milhões de brasileiros através de maior transparência e eficiência governamental é motivadora. Vejo grande oportunidade de aprendizado técnico e de impacto social nesta jornada.


---

## Sprint 1 – [11/09 - 24/09]

### Resumo da Sprint

Dando continuidade ao trabalho iniciado na Sprint 0, onde estabeleci o ambiente de desenvolvimento e compreendi a arquitetura geral do GovHub-br, esta sprint focou na implementação prática de soluções de orquestração de dados. Inicialmente planejava contribuir com melhorias nas pipelines existentes, mas ao identificar que outros membros da equipe já estavam trabalhando nessas issues, redirecionei meus esforços para uma demanda crítica: a criação de uma DAG no Apache Airflow para automatizar a ingestão de dados de emendas parlamentares. 

Esta mudança se mostrou estratégica, pois as emendas parlamentares representam uma fonte crucial de informações sobre alocação de recursos públicos no Brasil, alinhando-se perfeitamente com os objetivos de transparência do GovHub-br. O período foi dedicado ao estudo aprofundado sobre orquestração de workflows, integração com APIs governamentais e colaboração efetiva na definição das responsabilidades de cada membro da equipe.

### Atividades Realizadas

| Data  | Atividade                                        | Tipo (Código/Doc/Discussão/Outro) | Link/Referência | Status    |
| ----- | ------------------------------------------------ | --------------------------------- | --------------- | --------- |
| 12/09 | Estudo da documentação oficial do Airflow e conceitos de DAGs aplicados ao contexto governamental | Estudo | [Documentação Airflow](https://airflow.apache.org/docs/apache-airflow/stable/core-concepts/dags.html) | Concluído |
| 15/09 | Análise das APIs do Portal da Transparência para emendas parlamentares | Estudo | [API Portal Transparência](https://portaldatransparencia.gov.br/api-de-dados) | Concluído |
| 18/09 | Reunião de alinhamento da equipe para distribuição das responsabilidades e definição de padrões de desenvolvimento | Discussão | - | Concluído |
| 20/09 | Estudo dos operadores Airflow mais adequados para ingestão de dados governamentais | Estudo | Documentação técnica interna | Concluído |
| 23/09 | Desenvolvimento colaborativo da DAG para ingestão automatizada de dados de emendas parlamentares | Código | [Link do PR](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/blob/feat/dag-ingestao-emendas/airflow_lappis/dags/data_ingest/emendas_parlamentares/emendas_parlamentares_dag.py) | Em andamento |

### Principais Conquistas

* **Implementação de solução crítica**: Desenvolvimento colaborativo de uma DAG funcional para automatizar a ingestão de dados de emendas parlamentares, contribuindo diretamente para o objetivo de transparência do projeto.
* **Evolução técnica significativa**: Partindo do conhecimento geral adquirido na Sprint 0, desenvolvi compreensão sólida e aplicada dos conceitos do Airflow, incluindo estruturação de workflows complexos e gerenciamento de dependências entre tasks.
* **Integração prática com dados governamentais**: Primeira experiência hands-on integrando APIs oficiais do governo brasileiro ao ecossistema de dados do GovHub-br.
* **Fortalecimento da colaboração**: Participação ativa na definição de padrões de desenvolvimento da equipe, estabelecendo bases sólidas para sprints futuras.

### Principais Obstáculos

* **Complexidade da orquestração de dados**: Curva de aprendizado acentuada para dominar completamente o sistema de dependências entre tasks em DAGs complexas, especialmente considerando a criticidade dos dados governamentais.
* **Integração de tecnologias**: Desafios na implementação adequada dos **operators** do Airflow e sua integração eficiente com funções Python customizadas, mantendo a arquitetura Medallion estabelecida no projeto.
* **Particularidades dos dados governamentais**: Necessidade de compreender nuances específicas dos dados de emendas parlamentares, como estruturas hierárquicas e relacionamentos complexos.

### Conhecimentos Adquiridos

* **Orquestração aplicada ao setor público**: Compreensão da importância fundamental da modularização no desenvolvimento de DAGs para garantir manutenibilidade e escalabilidade, especialmente em projetos de transparência governamental.
* **Integração de dados governamentais**: Experiência prática valiosa com integração de APIs do Portal da Transparência e persistência de dados em bancos PostgreSQL através de workflows automatizados.
* **Colaboração em projetos open source**: Entendimento mais profundo da necessidade de aderência aos padrões arquiteturais estabelecidos pela comunidade para facilitar contribuições futuras e manutenção colaborativa.
* **Continuidade do aprendizado**: Conexão clara entre os conhecimentos teóricos da Sprint 0 e a aplicação prática, consolidando o entendimento sobre o ecossistema completo do GovHub-br.

### Objetivos para a Próxima Sprint

* [ ] **Finalização e otimização**: Refatorar e otimizar a DAG desenvolvida, implementando melhor modularização e integração com a arquitetura Medallion existente.
* [ ] **Documentação técnica**: Criar documentação detalhada do processo de desenvolvimento da DAG, incluindo decisões arquiteturais, padrões adotados e lições aprendidas para facilitar contribuições futuras.
* [ ] **Expansão do conhecimento**: Explorar outras fontes de dados governamentais que poderiam se beneficiar de abordagem similar, ampliando o impacto do trabalho realizado.

### Reflexões Pessoais

Esta sprint marcou uma transição importante do estudo teórico para a implementação prática, consolidando meu envolvimento com o projeto GovHub-br. A experiência de trabalhar diretamente com dados de emendas parlamentares me fez compreender ainda mais profundamente o potencial transformador deste projeto para a transparência pública brasileira. 

O desafio de criar uma DAG robusta para dados governamentais me proporcionou um aprendizado técnico significativo, mas principalmente me conectou de forma mais concreta com o propósito do projeto. Cada linha de código desenvolvida tem o potencial de facilitar o acesso de cidadãos a informações sobre como seus recursos públicos são utilizados.

A colaboração com a equipe durante esta sprint também foi enriquecedora, estabelecendo bases sólidas para contribuições futuras e fortalecendo minha compreensão sobre desenvolvimento colaborativo em projetos open source de impacto social.

---

# Diário de Bordo – \[Victor Schmidt]

**Disciplina:** \[GCES]

**Equipe:** \[GovHub]

**Comunidade/Projeto de Software Livre:** \[GovHub-br]

---

## Sprint 0 – \[01/09/2025 – 10/09/2025]

### Resumo da Sprint

Durante esta sprint inicial, focamos na compreensão geral do projeto GovHub-br, um sistema brasileiro de integração de dados governamentais. As atividades incluíram exploração da arquitetura do sistema, configuração do ambiente de desenvolvimento e criação do fork para trabalho em equipe. O projeto mostrou-se ser uma solução moderna para gestão de dados públicos, utilizando tecnologias como Apache Airflow, dbt, Jupyter e Superset.

### Atividades Realizadas

| Data | Atividade | Tipo | Link/Referência | Status |
| -- | -- | -- | -- | -- |
| 01/09 | Exploração inicial do repositório GovHub-br | Estudo | https://github.com/GovHub-br/data-application-gov-hub | Concluído |
| 02/09 | Leitura da documentação e README | Estudo     | README.md e e-book do projeto | Concluído |
| 03/09 | Análise da arquitetura Medallion | Estudo | Documentação técnica | Concluído |
| 05/09 | Configuração do ambiente Docker | Código | docker-compose.yml | Concluído |
| 09/09 | Criação do fork para trabalho em equipe e documentação do progresso da sprint | Código | Fork no GitHub | Concluído |

### Maiores Avanços

* **Entendimento da proposta do projeto**: Compreendi que o GovHub-br visa integrar sistemas estruturantes do governo federal (TransfereGov, Siape, Siafi, ComprasGov, Siorg) para gerar insights estratégicos.
* **Configuração bem-sucedida do ambiente**: Consegui rodar todo o stack de tecnologias localmente usando Docker Compose.
* **Familiarização com tecnologias modernas**: Aprendi sobre a arquitetura de dados moderna com Airflow para orquestração, dbt para transformação, e Superset para visualização.
* **Fork criado**: Estabeleci o repositório da equipe para desenvolvimento colaborativo.

### Maiores Dificuldades

* **Complexidade inicial do stack**: O projeto utiliza múltiplas tecnologias integradas, o que exigiu tempo para compreender como cada componente se conecta.
* **Volume de documentação**: Há bastante material para absorver, incluindo o e-book e slides do projeto.

### Aprendizados

* **Arquitetura Medallion**: Entendi os conceitos de camadas Bronze, Silver e Gold para organização de dados.
* **Orquestração com Airflow**: Compreendi como DAGs podem automatizar fluxos de dados complexos.
* **Transformação com dbt**: Aprendi sobre a ferramenta de transformação de dados e sua importância no pipeline.
* **Gestão de dados governamentais**: Percebi os desafios de integração de sistemas públicos fragmentados.
* **Docker Compose para desenvolvimento**: Vi como containerização facilita a configuração de ambientes complexos.


### Plano Pessoal para a Próxima Sprint

* [ x ] Contribuir com documentação ou correção de bugs identificados
* [ x ] Explorar em detalhes os modelos dbt existentes
* [ x ] Participar de discussions ou issues abertas no repositório
* [ x ] Compreender melhor o fluxo de dados dos sistemas governamentais integrados
* [ x ] Estudar mais sobre as ferramentas Jupyter e Superset para análise e visualização

---

## Sprint 1 – \[11/09/2025 – 24/09/2025]

### Resumo da Sprint

Durante essa sprint defini e implementei alguns rulesets dentro do 
repositório para impedir commits diretamente na branch `main`, também 
estudei os DAG's para implementar a DAG de Emendas Parlamentares. 
Também acompanhei as reuniões de treinamento e explicações da 
arquitetura feitas pelos mantenedores.

### Atividades Realizadas

| Data | Atividade | Tipo | Link/Referência | Status |
| -- | -- | -- | -- | -- |
| 11/09 | Análise das APIs do Portal da Transparência | Estudo | https://api.portaldatransparencia.gov.br/swagger-ui/index.html | Concluído |
| 13/09 | Estudo das APIs da Câmara dos Deputados | Estudo | https://dadosabertos.camara.leg.br/swagger/api.html?tab=api | Concluído |
| 15/09 | Implementação de rulesets para proteção da branch main | Código | Configurações do repositório | Concluído |
| 18/09 | Estudo dos DAGs existentes no projeto | Estudo | DAGs do Airflow | Concluído |
| 20/09 | Planejamento da implementação da DAG de Emendas Parlamentares | Planejamento | Documentação técnica | Concluído |
| 24/09 | Acompanhamento nas reuniões de treinamento e explicações da arquitetura | Treinamento | Reuniões com mantenedores | Concluído |

### Maiores Avanços

* **Proteção da branch main**: Implementei com sucesso rulesets no repositório para impedir commits diretos na branch principal, garantindo maior segurança e controle de qualidade do código.
* **Análise das APIs governamentais**: Estudei detalhadamente as APIs do Portal da Transparência e Câmara dos Deputados, compreendendo suas estruturas e possibilidades de integração.
* **Estudo dos DAGs Airflow**: Aprofundei o conhecimento sobre os DAGs existentes no projeto, preparando-me para implementar a DAG de Emendas Parlamentares.
* **Capacitação técnica**: Acompanhei as reuniões de treinamento com os mantenedores, absorvendo conhecimento sobre a arquitetura e melhores práticas do projeto.

### Maiores Dificuldades

* **Complexidade das APIs governamentais**: As APIs do Portal da Transparência e Câmara dos Deputados apresentaram estruturas de dados complexas que exigiram tempo adicional para compreensão.
* **Implementação de rulesets**: Configurar adequadamente os rulesets de proteção da branch main demandou estudo sobre as configurações do GitHub e boas práticas.
* **Curva de aprendizado do Airflow**: Compreender os DAGs existentes e planejar a implementação da nova DAG de Emendas Parlamentares foi desafiador.
* **Integração de conhecimentos**: Conectar os conhecimentos teóricos sobre as APIs com a implementação prática no ambiente Airflow apresentou dificuldades.

### Aprendizados

* **Configuração de rulesets**: Aprendi como implementar proteções de branch no GitHub, garantindo qualidade e segurança do código através de workflows automatizados.
* **Análise de APIs governamentais**: Compreendi a estrutura e funcionamento das APIs do Portal da Transparência e Câmara dos Deputados, identificando oportunidades de integração.
* **Desenvolvimento de DAGs**: Aprofundei meu conhecimento sobre orquestração de dados com Airflow, estudando DAGs existentes para implementar a DAG de Emendas Parlamentares.
* **Gestão de dados governamentais**: Percebi os desafios específicos de trabalhar com dados públicos e a importância de estruturas bem definidas para ingestão.


### Plano Pessoal para a Próxima Sprint

* [ ] Implementar a DAG de Emendas Parlamentares baseada nos estudos realizados
* [ ] Refinar e otimizar os rulesets implementados na branch main
* [ ] Contribuir com abertura de issues específicas para desenvolvimento das DAGs de ingestão
* [ ] Aprofundar conhecimentos sobre as APIs estudadas através de testes práticos
* [ ] Participar ativamente das discussões sobre políticas GCES para comunidade aberta
* [ ] Documentar os aprendizados sobre as APIs governamentais para facilitar contribuições futuras
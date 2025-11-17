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

* [ x ] Implementar a DAG de Emendas Parlamentares baseada nos estudos realizados
* [ x ] Refinar e otimizar os rulesets implementados na branch main
* [ x ] Contribuir com abertura de issues específicas para desenvolvimento das DAGs de ingestão
* [ x ] Aprofundar conhecimentos sobre as APIs estudadas através de testes práticos
* [ x ] Participar ativamente das discussões sobre políticas GCES para comunidade aberta
* [ x ] Documentar os aprendizados sobre as APIs governamentais para facilitar contribuições futuras

---

## Sprint 2 – \[25/09/2025 – 08/10/2025]

### Resumo da Sprint

Durante esse Sprint implementei a ingestão de dados de emendas parlamentares do Portal da Transparência. Criei uma DAG do Airflow que coleta dados via API com paginação automática e persiste no PostgreSQL usando UPSERT com IDs únicos baseados em hash SHA256.

Desenvolvi 17 testes (9 unitários + 8 de integração) alcançando 100% de cobertura no ClienteEmendas. Implementei configurações com .env.example para segurança de API keys e reorganizei a estrutura de pastas do projeto.

A DAG foi testada em ambiente real com dados inseridos corretamente no banco.

### Atividades Realizadas

| Data | Atividade | Tipo | Link/Referência | Status |
| -- | -- | -- | -- | -- |
| 25/09 | Implementação da DAG de ingestão de emendas parlamentares | Código | [PR #6](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/6) | Concluído |
| 27/09 | Desenvolvimento do ClienteEmendas com paginação automática | Código | [PR #6](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/6) | Concluído |
| 29/09 | Implementação de UPSERT com IDs únicos SHA256 | Código | [PR #6](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/6) | Concluído |
| 01/10 | Desenvolvimento de testes unitários (9 testes) | Teste | [PR #6](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/6) | Concluído |
| 03/10 | Desenvolvimento de testes de integração (8 testes) | Teste | [PR #6](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/6) | Concluído |
| 05/10 | Configuração de segurança com .env.example | Código | [PR #6](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/6) | Concluído |
| 06/10 | Reorganização da estrutura de pastas do projeto | Código | [PR #6](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/6) | Concluído |
| 08/10 | Teste da DAG em ambiente real com dados no banco | Teste | [PR #6](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/6) | Concluído |

### Maiores Avanços

* **Implementação completa da DAG de Emendas Parlamentares**: Criei uma DAG funcional do Airflow que coleta dados de emendas parlamentares do Portal da Transparência com paginação automática e persiste no PostgreSQL usando UPSERT com IDs únicos SHA256.
* **Desenvolvimento de testes abrangentes**: Implementei 17 testes (9 unitários + 8 de integração) alcançando 100% de cobertura no ClienteEmendas, garantindo qualidade e confiabilidade do código.
* **Configurações de segurança**: Implementei configurações com .env.example para proteção de API keys e remoção de dados sensíveis do histórico do repositório.
* **Reorganização da estrutura do projeto**: Melhorei a organização das pastas e estrutura do código, facilitando manutenção e contribuições futuras.
* **Validação em ambiente real**: Testei a DAG em ambiente real com dados inseridos corretamente no banco, confirmando o funcionamento end-to-end.

### Maiores Dificuldades

* **Implementação de paginação automática**: Desenvolver a lógica de paginação automática para esgotar todos os dados da API do Portal da Transparência foi complexo, exigindo tratamento de diferentes cenários de resposta.
* **Geração de IDs únicos SHA256**: Implementar o sistema de UPSERT com IDs únicos baseados em hash SHA256 demandou compreensão profunda da estrutura dos dados e garantia de consistência.
* **Desenvolvimento de testes abrangentes**: Criar 17 testes cobrindo cenários de sucesso, erro e edge cases exigiu planejamento detalhado e mocks complexos para API e banco de dados.
* **Configuração de segurança**: Implementar as configurações de segurança com .env.example e remover dados sensíveis do histórico do repositório apresentou desafios de gerenciamento de credenciais.
* **Integração com PostgreSQL**: Garantir que a persistência dos dados no PostgreSQL funcionasse corretamente com UPSERT e metadados técnicos demandou testes extensivos.

### Aprendizados

* **Desenvolvimento de DAGs Airflow**: Aprofundei significativamente meu conhecimento sobre orquestração de dados, implementando uma DAG completa com paginação automática, retry automático e logs detalhados.
* **Sistemas de UPSERT com IDs únicos**: Aprendi a implementar estratégias robustas de persistência usando hash SHA256 para garantir unicidade e evitar duplicação de dados em reprocessamentos.
* **Desenvolvimento de testes abrangentes**: Compreendi a importância de cobertura de testes completa (100%), aprendendo a estruturar testes unitários e de integração com mocks para APIs e bancos de dados.
* **Configurações de segurança**: Adquiri conhecimento sobre boas práticas de segurança, implementando .env.example e gerenciando credenciais de forma segura em projetos colaborativos.
* **Paginação automática em APIs**: Aprendi a implementar lógica robusta de paginação que esgota todos os dados disponíveis em APIs governamentais, tratando diferentes cenários de resposta.
* **Metadados técnicos**: Compreendi a importância de gerar metadados técnicos por registro para auditoria e rastreabilidade de dados governamentais.


### Plano Pessoal para a Próxima Sprint

* [ ] Contribuir com abertura de issues específicas para desenvolvimento de novas DAGs de ingestão baseadas nas APIs estudadas
* [ ] Aplicar os conhecimentos adquiridos sobre testes para melhorar a cobertura de outros componentes do projeto
* [ ] Implementar melhorias na DAG de Emendas Parlamentares baseadas em feedback e novos requisitos
* [ ] Participar ativamente das discussões sobre políticas GCES para comunidade aberta
* [ ] Documentar os aprendizados sobre desenvolvimento de DAGs para facilitar contribuições de outros membros da equipe
* [ ] Explorar implementação de novas funcionalidades como monitoramento e alertas para as DAGs
* [ ] Contribuir com refatorações e otimizações na estrutura do projeto baseadas na experiência adquirida

## Sprint 3 – [09/10/2025 - 22/10/2025]

### Resumo da Sprint

A sprint foi dedicada ao desenvolvimento do modelo Bronze de Emendas Parlamentares no DBT, estabelecendo toda a base necessária para a ingestão estruturada dos dados provenientes da API do Portal da Transparência.
Esse trabalho envolveu padronização de campos, normalização de formatos, unificação de nomenclaturas, além da preparação da documentação e das regras de validação que irão sustentar as próximas camadas do pipeline (Silver e Gold).
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


## Sprint 4 – [23/10/2025 - 05/11/2025]

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


# Diário de Bordo – Daniel Ferreira

**Disciplina:** Gestão de Configuração e Evolução de Software (GCES)  
**Equipe:** GovHub  
**Comunidade/Projeto de Software Livre:** GovHub-br  

---

## Sprint 0 – 01/09/2025 – 10/09/2025  

### Resumo da Sprint  

Nesta sprint inicial, foquei principalmente em estudar o projeto GovHub-br, entendendo sua proposta e principais tecnologias utilizadas, além de realizar a configuração completa do ambiente de desenvolvimento.  

### Atividades Realizadas  

| Data | Atividade | Tipo | Link/Referência | Status |  
|------|-----------|------|-----------------|---------|  
| 02/09 | Análise inicial do repositório GovHub-br | Estudo | https://github.com/GovHub-br/data-application-gov-hub | ✅ Concluído |  
| 03/09 | Estudo da documentação do projeto GovHub-br | Estudo | README.md e docs oficiais | ✅ Concluído |  
| 06/09 | Setup completo do ambiente Docker | Implementação | docker-compose.yml | ✅ Concluído |  

### Maiores Avanços  

* Consegui configurar e rodar o ambiente local.  
* Compreensão inicial sobre a proposta do GovHub-br e seu impacto.  

### Maiores Dificuldades  

* A quantidade de tecnologias diferentes envolvidas (Airflow, dbt, Superset) exige tempo para entender como tudo se conecta.  
* Foi necessário revisar a documentação algumas vezes até conseguir configurar o ambiente corretamente.  

### Aprendizados  

* Entendi melhor os conceitos de containerização e como o Docker simplifica a replicação de ambientes de dados.  
* Aprendi sobre a importância de organizar os dados em camadas (Bronze, Silver e Gold).
* Percebi como uma documentação clara e detalhada sobre a configuração do ambiente é crucial para agilizar o processo de onboarding de novos contribuidores.

### Plano Pessoal para a Próxima Sprint  

* [ ] Aprofundar o estudo nos modelos dbt.  
* [ ] Explorar os pipelines no Airflow para entender a orquestração.
* [ ] Estudar mais sobre as ferramentas Jupyter, Superset e Airflow para análise e visualização. 
* [ ] Contribuir com melhorias de documentação ou resolver alguma issue.  

### Reflexões Pessoais  

Foi uma sprint de introdução, mas já deu para perceber o potencial de aprendizado técnico e impacto social do projeto. Senti que dominar essas ferramentas vai ser importante não só para o projeto, mas também para minha formação como engenheiro de software.  

---

## Sprint 1 – 11/09/2025 – 24/09/2025

### Resumo da Sprint

Após a fase de imersão e configuração do ambiente na Sprint 0, esta sprint marcou meu primeiro mergulho profundo no desenvolvimento de uma pipeline de dados para o GovHub-br. Fui designado para a issue de criação de uma DAG de ingestão para os detalhes e recursos de deputados.

O desafio consistiu em desenvolver um workflow no Apache Airflow capaz de ler os IDs dos deputados já existentes na base, consultar dinamicamente múltiplos endpoints da API de Dados Abertos da Câmara para cada um deles e persistir essas informações em tabelas `raw` dedicadas. O foco foi garantir que o processo fosse idempotente — permitindo reprocessamentos sem duplicar dados — e escalável, estabelecendo uma base sólida para a construção de perfis detalhados sobre os representantes públicos

### Atividades Realizadas

| Data | Atividade | Tipo | Link/Referência | Status |
|---|---|---|---|---|
| 12/09 | Estudo de padrões de DAGs dinâmicas no Airflow para iteração sobre múltiplos IDs | Estudo | Documentação Airflow & artigos técnicos | ✅ Concluído |
| 15/09 | Análise e mapeamento dos endpoints da API de Dados Abertos da Câmara referentes a `/deputados/{id}` | Estudo | [API Dados Abertos - Deputados](https://dadosabertos.camara.leg.br/api/v2/deputados) | ✅ Concluído |
| 18/09 | Reunião de alinhamento da equipe para distribuição das responsabilidades e definição de padrões de desenvolvimento | Discussão | - | ✅ Concluído |
| 20/09 | Definição da estratégia de persistência com `UPSERT` para garantir idempotência na ingestão de dados | Código/Design | Documentação do PostgreSQL | ✅ Concluído |
| 23/09 | Desenvolvimento da DAG para orquestrar a ingestão de detalhes dos deputados por ID | Código | [Link do PR](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/5)/ | 🚧 Em andamento |

### Maiores Avanços

* **Base de uma DAG escalável:** Consegui criar uma estrutura de DAG que busca dados por ID, um padrão que poderemos reusar em outras ingestões.
* **Integridade dos dados garantida:** Implementei a lógica de `UPSERT` (INSERT/UPDATE), o que deixa a pipeline mais segura contra falhas e reprocessamentos.
* **Primeiro contato com a API da Câmara:** Tive minha primeira experiência prática com a API de Dados Abertos, entendendo melhor como ela funciona.
* **Seguindo a arquitetura:** Todo o desenvolvimento foi feito para popular a camada `raw` (bronze), conforme o padrão Medallion que usamos no projeto.

### Maiores Dificuldades

* **Iteração no Airflow:** Fazer a DAG rodar um fluxo de tarefas para cada deputado (uma iteração dinâmica) foi mais complexo do que eu imaginava.
* **Lógica de `UPSERT`:** Pensar na melhor forma de implementar o `UPSERT` de um jeito eficiente dentro do Airflow deu um certo trabalho.
* **Definição das chaves únicas:** Acertar as chaves primárias para cada tabela foi um ponto crucial e desafiador para o `UPSERT` funcionar corretamente.

### Aprendizados

* **Workflows dinâmicos no Airflow:** Aprendi na prática como criar pipelines que se adaptam aos dados de entrada, e não apenas fluxos estáticos.
* **Importância da idempotência:** Ficou muito claro para mim o quanto a idempotência é essencial para ter pipelines de dados confiáveis.
* **Consumo de APIs do governo:** Entendi melhor as boas práticas para lidar com APIs públicas, como tratar diferentes respostas e organizar os dados brutos.
* **Colaboração em ETL:** As conversas com a equipe sobre o escopo e as chaves dos dados foram muito importantes para o desenvolvimento do processo de ETL.

### Plano para a Próxima Sprint

* [ ] **Finalizar e testar a DAG:** Concluir o código, rodar os testes com a amostra de 50 IDs e confirmar que o reprocessamento não duplica nada.
* [ ] **Refatorar o código:** Depois de validar, quero otimizar o código, melhorando as consultas e a organização geral.
* [ ] **Criar a documentação:** Documentar como a DAG funciona, as decisões que tomei e os endpoints que ela usa.
* [ ] **Planejar a camada Silver:** Começar a pensar em como vamos limpar e transformar esses dados brutos para a próxima etapa da arquitetura.

### Reflexões Pessoais

Senti que meu aprendizado deu um salto nesta sprint, passando da teoria para a prática. Trabalhar diretamente com os dados dos deputados me conectou mais com o propósito do GovHub-br. Percebi que não estamos só juntando números, mas montando um perfil detalhado de quem toma as decisões no país.

Resolver o desafio técnico do `UPSERT` e da escalabilidade foi bem gratificante. Ver o código funcionando me deixa confiante de que estou construindo algo sólido. A colaboração com o time foi fundamental. Estou animado para fechar essa tarefa e ver os dados sendo usados para gerar mais transparência.

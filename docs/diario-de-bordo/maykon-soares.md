# Diário de Bordo – [Maykon Júnio dos Santos Soares]

**Disciplina:** GCES  
**Equipe:** GovHub  
**Comunidade/Projeto de Software Livre:** GovHub-br

---

## Sprint 0 – 01/09/2025 – 10/09/2025

### Resumo da Sprint

Na sprint de abertura, o objetivo principal foi conhecer melhor o projeto **GovHub-br**, levantar informações sobre sua arquitetura e preparar o ambiente para futuros desenvolvimentos. As atividades envolveram desde a leitura de materiais de apoio até a configuração prática de ferramentas e a criação do repositório da equipe.

### Atividades Realizadas

| Data  | Atividade                                             | Tipo (Código/Doc/Discussão/Outro) | Link/Referência                                       | Status    |
| ----- | ----------------------------------------------------- | --------------------------------- | ----------------------------------------------------- | --------- |
| 08/09 | Primeira exploração do repositório GovHub-br          | Estudo                            | https://github.com/GovHub-br/data-application-gov-hub | Concluído |
| 08/09 | Leitura do README e do material de apoio              | Estudo                            | README.md e e-book do projeto                         | Concluído |
| 08/09 | Estudo da arquitetura de dados em camadas (Medallion) | Estudo                            | Documentação técnica                                  | Concluído |

### Maiores Avanços

- Compreensão clara da **finalidade do GovHub-br** como integrador de informações públicas.
- Sucesso na **instalação e execução do stack tecnológico** em containers.
- Primeira aproximação prática com a **arquitetura Medallion (Bronze, Silver, Gold)**.
- Criação do **repositório derivado (fork)** para centralizar as contribuições da equipe.

### Aprendizados

- Funcionamento da arquitetura Medallion para organizar dados em estágios.
- Introdução ao **dbt** como mecanismo de transformação de dados.

### Plano Pessoal para a Próxima Sprint

- [ ] Contribuir em pelo menos uma melhoria de documentação ou correção de bug.
- [ ] Explorar em detalhe os modelos dbt existentes no repositório.
- [ ] Participar de discussions ou issues da comunidade.
- [x] Mapear o fluxo de dados dos sistemas governamentais já integrados.
- [ ] Aprofundar o uso do Superset e do Jupyter para análise.

---

## Sprint 2 – 25/09/2025 – 08/10/2025

### Resumo da Sprint

Nesta sprint, o foco foi melhorar a **documentação de contribuição do projeto**, adicionando um tutorial claro de instalação e primeiros passos no arquivo `CONTRIBUTING.md`. Isso faz parte do planejamento de **onboarding de novos contribuidores**, garantindo que novos participantes consigam facilmente instalar, configurar e executar o projeto localmente.

### Atividades Realizadas

| Data  | Atividade                                                          | Tipo (Código/Doc/Discussão/Outro) | Link/Referência                                                                       | Status    |
| ----- | ------------------------------------------------------------------ | --------------------------------- | ------------------------------------------------------------------------------------- | --------- |
| 13/09 | Criação de tutorial de instalação no CONTRIBUTING.md               | Documentação                      | [Issue #57](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/57) | Concluído |
| 14/09 | Planejamento de onboarding e revisão de padrões de contribuição    | Documentação                      | [Commit feat: adiciona tutorial de instalação em CONTRIBUTING.md](#)                  | Concluído |
| 15/09 | Teste de instalação e execução local do projeto para novos membros | Teste                             | docs/onboarding.md                                                                    | Concluído |

### Maiores Avanços

- Tutorial de instalação adicionado ao arquivo `CONTRIBUTING.md`.
- Documentação de onboarding mais clara e estruturada.
- Processo de entrada para novos contribuidores simplificado e testado.

### Maiores Dificuldades

- Ajustar a documentação para diferentes sistemas operacionais.
- Garantir que todas as dependências fossem bem descritas no guia.
- Testar a clareza da documentação com novos contribuidores.

### Aprendizados

- A importância de um bom guia de contribuição para a escalabilidade da comunidade.
- Como estruturar documentação técnica para diferentes perfis de usuários.
- Estratégias para validar documentação na prática.

### Plano Pessoal para a Próxima Sprint

- [ ] Iniciar melhorias no pipeline de dados, começando pelo modelo bronze.
- [ ] Refatorar pequenas partes da ingestão para maior clareza.
- [ ] Explorar automação de testes de instalação no CI.

---

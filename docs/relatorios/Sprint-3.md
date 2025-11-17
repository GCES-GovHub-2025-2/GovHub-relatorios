# 📝 Relatório de Contribuição – Sprint 3

**Disciplina:** Gestão de Configuração e Evolução de Software  
**Equipe:** GovHub  
**Comunidade/Projeto de Software Livre:** GovHub-br  
**Período da Sprint:** 09/10 – 22/10

---

## 1. Objetivos da Sprint

- [x] Integração dos dados abertos da Câmara dos Deputados ([PR #11](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/11))
- [x] Adição de testes abrangentes para a DAG e cliente ([PR #11](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/11))
- [x] Início da modelagem DBT bronze para as inserções realizadas
- [x] Criação e padronização do guia de contribuição (`CONTRIBUTING.md`)

---

## 2. Entregas Coletivas

| Entrega                                              | Status    | Link/Referência                                                                                             | Observações                                  |
| ---------------------------------------------------- | --------- | ----------------------------------------------------------------------------------------------------------- | -------------------------------------------- |
| Integração dos dados abertos da Câmara dos Deputados | Concluído | [PR #11](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/11)                            | Ingestão de deputados implementada           |
| Testes abrangentes para DAG e cliente                | Concluído | [PR #11](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/11)                            | Testes unitários e de integração adicionados |
| Início da modelagem DBT bronze                       | Parcial   | –                                                                                                           | Estrutura inicial de tabelas bronze definida |
| Criação do guia de contribuição (`CONTRIBUTING.md`)  | Concluído | [CONTRIBUTING.md](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/blob/main/CONTRIBUTING.md) | Guia revisado e validado com checklist de PR |

---

## 3. Contribuições Individuais

| Integrante                     | Contribuições                                                                                                              | Links (PRs, Issues, Docs)                                                                          | Observações                       |
| ------------------------------ | -------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | --------------------------------- |
| Maykon Júnio dos Santos Soares | Criação e padronização do guia de contribuição, testes automatizados com pytest e validação do ambiente de desenvolvimento | [PR #11](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/11) / CONTRIBUTING.md | Foco em documentação e testes     |
| Davi de Aguiar Vieira          | Revisão da ingestão de deputados, apoio na validação dos testes e início da modelagem DBT bronze                           | [PR #11](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/11)                   | Foco em ingestão e testes         |
| Mateus de Castro Santos        | Participação na revisão da ingestão, validação dos testes e colaboração na estruturação da modelagem bronze                | [PR #11](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/11)                   | Foco em testes e modelagem bronze |
| Leonardo Fachinello Bonetti        | Correção dos testes, otimização do código da DAG mantendo somente o necessário, correção do código para o padrão definido no projeto, envio do pull request da dag de deputados e inicio da modelagem bronze de deputados          | [PR #11](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/11)  [Issue #4](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/4)                 | Foco na finalização do PR e inicio da modelagem bronze |
| Mateus Henrique Queiroz Magalhães Sousa     |   O desenvolvimento completo do modelo Bronze de Emendas Parlamentares no DBT.      | [PR #11](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/12)  [Issue #8](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/8)                 | Foco na modelagem bronze para emendas parlamentares |
| Victor Hugo Lima Schmidt    |    O desenvolvimento completo do modelo Bronze de Emendas Parlamentares no DBT, estruturando toda a base necessária para que o pipeline possa avançar para as camadas Silver e Gold.     | [PR #11](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/12)  [Issue #8](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/8)                 | Foco na modelagem bronze para emendas parlamentares |


---

## 4. Maiores Avanços

- Integração dos dados abertos da Câmara dos Deputados concluída
- Implementação de testes unitários e de integração para DAG e cliente
- Estruturação inicial da camada bronze no DBT
- Guia de contribuição (`CONTRIBUTING.md`) finalizado, validado e testado para onboarding

---

## 5. Maiores Dificuldades

- Ajustes na estrutura dos dados para garantir compatibilidade com o modelo bronze
- Definição dos critérios de granularidade para as tabelas bronze
- Cobertura de testes para cenários de erro e dados inconsistentes
- Garantir compatibilidade do guia de contribuição em diferentes sistemas operacionais

---

## 6. Lições Aprendidas

- A integração de dados abertos exige validação constante dos formatos e contratos
- Testes abrangentes são essenciais para garantir a confiabilidade das DAGs e clientes
- Iniciar a modelagem bronze desde cedo facilita o alinhamento do time e reduz retrabalho
- Um guia de contribuição bem estruturado melhora a entrada de novos membros e reduz erros

---

## 7. Planejamento para a Próxima Sprint

- [ ] Evoluir a modelagem DBT bronze com base nos dados integrados
- [ ] Expandir cobertura de testes para novos cenários
- [ ] Refatorar trechos do código de ingestão para maior clareza e modularidade
- [ ] Documentar decisões de modelagem e contratos de dados
- [ ] Apoiar o onboarding de novos membros com materiais de apoio

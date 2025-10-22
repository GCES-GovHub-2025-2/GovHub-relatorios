# 📝 Relatório de Contribuição – Sprint 3

**Disciplina:** Gestão de Configuração e Evolução de Software
**Equipe:** [GovHub]
**Comunidade/Projeto de Software Livre:** [GovHub]
**Período da Sprint:** [09/10 – 22/10]

---

## 1. Objetivos da Sprint

- [x] Integração dos dados abertos da Câmara dos Deputados ([PR #11](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/11))
- [x] Adição de testes abrangentes para a DAG e cliente ([PR #11](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/11))
- [x] Início da modelagem DBT bronze para as inserções realizadas

---

## 2. Entregas Coletivas

| Entrega                                                        | Status    | Link/Referência                                                                                                   | Observações                                      |
| -------------------------------------------------------------- | --------- | ----------------------------------------------------------------------------------------------------------------- | ------------------------------------------------ |
| Integração dos dados abertos da Câmara dos Deputados           | Concluído | [PR #11](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/11)                                 | Ingestão de deputados implementada               |
| Testes abrangentes para DAG e cliente                          | Concluído | [PR #11](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/11)                                 | Testes unitários e de integração adicionados      |
| Início da modelagem DBT bronze                                 | Parcial   | –                                                                                                                | Estrutura inicial de tabelas bronze definida      |

---

## 3. Contribuições Individuais

| Integrante                | Contribuições                                                                                                   | Links (PRs, Issues, Docs)                                                                                 | Observações                       |
|--------------------------|----------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------|-----------------------------------|
| Davi de Aguiar Vieira    | Revisão da ingestão de deputados, apoio na validação dos testes e início da modelagem DBT bronze                | [PR #11](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/11)                          | Foco em ingestão e testes         |
| Mateus de Castro Santos  | Participação na revisão da ingestão, validação dos testes e colaboração na estruturação da modelagem bronze     | [PR #11](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/11)                          | Foco em testes e modelagem bronze |

---

## 4. Maiores Avanços

- Integração dos dados abertos da Câmara dos Deputados
- Implementação de testes unitários e de integração para DAG e cliente
- Estruturação inicial da camada bronze no DBT

---

## 5. Maiores Dificuldades

- Ajustes na estrutura dos dados para garantir compatibilidade com o modelo bronze
- Definição dos critérios de granularidade para as tabelas bronze
- Cobertura de testes para cenários de erro e dados inconsistentes

---

## 6. Lições Aprendidas

- A integração de dados abertos exige validação constante dos formatos e contratos
- Testes abrangentes são essenciais para garantir a confiabilidade das DAGs e clientes
- Iniciar a modelagem bronze desde cedo facilita o alinhamento do time e reduz retrabalho

---

## 7. Planejamento para a Próxima Sprint

- [ ] Evoluir a modelagem DBT bronze com base nos dados integrados
- [ ] Expandir cobertura de testes para novos cenários
- [ ] Documentar decisões de modelagem e contratos de dados
- [ ] Apoiar o onboarding de novos membros com materiais de apoio

---

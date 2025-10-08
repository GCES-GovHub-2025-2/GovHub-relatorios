# 📝 Relatório de Contribuição – Sprint 2

**Disciplina:** Gestão de Configuração e Evolução de Software

**Equipe:** [GovHub]

**Comunidade/Projeto de Software Livre:** [GovHub]

**Período da Sprint:** [25/09 – 08/10]

---

## 1. Objetivos da Sprint

-   [x] Integração do Portal da Transparência (emendas parlamentares)
-   [x] Revisão e aprovação da migração do CI/CD
-   [x] Adição de ChangeLog ao projeto
-   [x] Template de commit para padronização
-   [x] Atualização do template de Pull Request
-   [x] Definição de atividades futuras de modelagem DBT (camada bronze) para Portal da Transparência
-   [ ] Persistência de DAGs de deputados

---

## 2. Entregas Coletivas

| Entrega                                                       | Status    | Link/Referência                                                                                                                                                                                                                                       | Observações                                                    |
| ------------------------------------------------------------- | --------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| Integração do Portal da Transparência (emendas parlamentares) | Concluído | [PR #6](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/6)                                                                                                                                                                        | DAG de emendas implementada e validada                         |
| Revisão e aprovação da migração do CI/CD                      | Concluído | [PR #11](https://github.com/GovHub-br/data-application-gov-hub/pull/11)                                                                                                                                                                               | Pipeline consolidada em GitHub Actions                         |
| Adição de ChangeLog                                           | Concluído | [PR #51](https://github.com/GovHub-br/gov-hub/pull/51/files)                                                                                                                                                                                          | Registro de mudanças padronizado                               |
| Template de commit no repositório de relatórios               | Concluído | [PR #16](https://github.com/GCES-GovHub-2025-2/GovHub-relatorios/pull/16)                                                                                                                                                                             | Padronização de mensagens de commit (incentivo a Conventional) |
| Definição de atividades futuras de modelagem DBT (bronze)     | Concluído | Issues: [#8](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/8), [#9](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/9), [#10](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/10) | Backlog da modelagem bronze definido                           |
| Persistência de DAGs de deputados                             | Parcial   | –                                                                                                                                                                                                                                                     | Configuração e estratégia inicial de persistência em andamento |
| Template de commit no `gov-hub`                               | Concluído | [PR #54](https://github.com/GovHub-br/gov-hub/pull/54)                                                                                                                                                                                                | Padronização de mensagens de commit (incentivo a Conventional) |
| Atualização do template de Pull Request                       | Concluído | [PR #56](https://github.com/GovHub-br/gov-hub/pull/56)                                                                                                                                                                                                | Template atualizado para incluir informações relevantes        |

---

## 3. Contribuições Individuais

| Integrante              | Contribuições                                                                                                                           | Links (PRs, Issues, Docs)                                                                                                                                                                                                                                                                                                                                                                                      | Observações      |
| ----------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- |
| Davi de Aguiar Vieira   | Revisão na integração de emendas (Portal da Transparência), revisão da migração de CI/CD e definição do escopo da modelagem DBT bronze. | [PR #6](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/6), [PR #11](https://github.com/GovHub-br/data-application-gov-hub/pull/11), Issues: [#8](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/8), [#9](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/9), [#10](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/10) | Foco em 1, 2 e 5 |
| Mateus de Castro Santos | Atuação na análise e revisão da integração de emendas, apoio na revisão da migração de CI/CD e no planejamento da modelagem bronze.     | [PR #6](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/6), [PR #11](https://github.com/GovHub-br/data-application-gov-hub/pull/11), Issues: [#8](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/8), [#9](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/9), [#10](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/10) | Foco em 1, 2 e 5 |

---

## 4. Maiores Avanços

-   Integração inicial de dados de emendas parlamentares via Portal da Transparência
-   Pipeline CI/CD consolidada na organização, reduzindo fricção entre repositórios
-   Padronização documental (ChangeLog) e de processo (template de commit)
-   Backlog de modelagem DBT bronze estruturado para próximas iterações

---

## 5. Maiores Dificuldades

-   Ajustes de credenciais e segredos na transição de CI/CD entre organizações
-   Definição de granularidade e esquema-alvo para a camada bronze do DBT
-   Ausência de documentação uniforme nas fontes públicas (APIs) exigindo validações adicionais

---

## 6. Lições Aprendidas

-   Ter um ChangeLog e um template de commit facilita rastreabilidade e revisões
-   Consolidar CI/CD cedo reduz riscos e acelera ciclos de entrega
-   Começar pela camada bronze do DBT ajuda a alinhar expectativas de schema e qualidade de dados
-   Definição simples de templates de contribuição (commits, PRs, issues) melhora a experiência de novos colaboradores

---

## 7. Planejamento para a Próxima Sprint

-   [ ] Implementar primeiros modelos DBT (bronze) a partir do backlog definido
-   [ ] Evoluir a integração do Portal da Transparência (incluindo paginação, rate limits e enriquecimentos)
-   [ ] Finalizar a persistência e agendamento das DAGs de deputados
-   [ ] Adicionar testes e monitoramento básico (alertas) nas DAGs
-   [ ] Ampliar documentação de dados e do processo de contribuição

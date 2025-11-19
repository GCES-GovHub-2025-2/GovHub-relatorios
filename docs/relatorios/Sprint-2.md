# 📝 Relatório de Contribuição – Sprint 2 e 3

**Disciplina:** Gestão de Configuração e Evolução de Software  
**Equipe:** [GovHub]  
**Comunidade/Projeto de Software Livre:** [GovHub]

---

## 🧭 Período das Sprints

-   **Sprint 2:** 25/09 – 08/10
-   **Sprint 3:** 09/10 – 25/10

---

## 1. Objetivos das Sprints

### 🎯 Sprint 2

-   [x] Integração do Portal da Transparência (emendas parlamentares)
-   [x] Revisão e aprovação da migração do CI/CD
-   [x] Adição de ChangeLog ao projeto
-   [x] Template de commit para padronização
-   [x] Atualização do template de Pull Request
-   [x] Definição de atividades futuras de modelagem DBT (camada bronze) para Portal da Transparência
-   [ ] Persistência de DAGs de deputados

### 🚀 Sprint 3

-   [x] Implementação completa da Gerência de Configuração (GCES)
-   [x] Implementação de Git Flow e versionamento semântico
-   [x] Configuração de automações com Dependabot e CodeQL
-   [x] Criação de templates YAML (issues e PRs)
-   [x] Documentação dos padrões de código, arquitetura e estrutura do projeto
-   [x] Limpeza e reestruturação de arquivos temporários
-   [x] Revisão final e preparação para PR principal
-   [ ] Aplicação dos padrões em outros repositórios do GovHub

---

## 2. Entregas Coletivas

| Entrega                                                       | Status    | Link/Referência                                                                                                                                                                                                                                       | Observações                                                                                     |
| ------------------------------------------------------------- | --------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| Integração do Portal da Transparência (emendas parlamentares) | Concluído | [PR #6](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/6)                                                                                                                                                                        | DAG de emendas implementada e validada                                                          |
| Implementação de testes abrangentes                           | Concluído | [PR #6](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/6)                                                                                                                                                                        | 17 testes implementados (9 unitários + 8 de integração) com 100% de cobertura no ClienteEmendas |
| Revisão e aprovação da migração do CI/CD                      | Concluído | [PR #11](https://github.com/GovHub-br/data-application-gov-hub/pull/11)                                                                                                                                                                               | Pipeline consolidada em GitHub Actions                                                          |
| Adição de ChangeLog                                           | Concluído | [PR #51](https://github.com/GovHub-br/gov-hub/pull/51/files)                                                                                                                                                                                          | Registro de mudanças padronizado                                                                |
| Template de commit no repositório de relatórios               | Concluído | [PR #16](https://github.com/GCES-GovHub-2025-2/GovHub-relatorios/pull/16)                                                                                                                                                                             | Padronização de mensagens de commit (incentivo a Conventional)                                  |
| Definição de atividades futuras de modelagem DBT (bronze)     | Concluído | Issues: [#8](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/8), [#9](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/9), [#10](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/10) | Backlog da modelagem bronze definido                                                            |
| Persistência de DAGs de deputados                             | Parcial   | –                                                                                                                                                                                                                                                     | Configuração e estratégia inicial de persistência em andamento                                  |
| Template de commit no `gov-hub`                               | Concluído | [PR #54](https://github.com/GovHub-br/gov-hub/pull/54)                                                                                                                                                                                                | Padronização de mensagens de commit (incentivo a Conventional)                                  |
| Atualização do template de Pull Request                       | Concluído | [PR #56](https://github.com/GovHub-br/gov-hub/pull/56)                                                                                                                                                                                                | Template atualizado para incluir informações relevantes                                         |
| Implementação da Gerência de Configuração (GCES)              | Concluído | [PR #57](https://github.com/GCES-GovHub-2025-2/GovHub-relatorios/pull/57)                                                                                                                                                                             | Git Flow, versionamento semântico, Dependabot e CodeQL aplicados                                |
| Criação dos templates YAML de Issues e PRs                    | Concluído | [.github/ISSUE_TEMPLATE/\*.yml](https://github.com/GCES-GovHub-2025-2/GovHub-relatorios/tree/main/.github/ISSUE_TEMPLATE)                                                                                                                             | Templates profissionais e documentados                                                          |
| Documentação completa de padrões e arquitetura                | Concluído | [docs/](https://github.com/GCES-GovHub-2025-2/GovHub-relatorios/tree/main/docs)                                                                                                                                                                       | Documentação modular, guias e convenções padronizadas                                           |

---

## 3. Contribuições Individuais

| Integrante                  | Contribuições                                                                                                                                                         | Links (PRs, Issues, Docs)                                                                                                                                                                                                                                                                                                                                                                                      | Observações                       |
| --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------- |
| **Davi de Aguiar Vieira**   | Revisão na integração de emendas (Portal da Transparência), revisão da migração de CI/CD e definição do escopo da modelagem DBT bronze.                               | [PR #6](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/6), [PR #11](https://github.com/GovHub-br/data-application-gov-hub/pull/11), Issues: [#8](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/8), [#9](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/9), [#10](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/10) | Foco em integração e modelagem    |
| **Mateus de Castro Santos** | Atuação na análise e revisão da integração de emendas, apoio na revisão da migração de CI/CD e no planejamento da modelagem bronze.                                   | [PR #6](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/pull/6), [PR #11](https://github.com/GovHub-br/data-application-gov-hub/pull/11), Issues: [#8](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/8), [#9](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/9), [#10](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/10) | Foco em testes e CI/CD            |
| **Maykon Júnio dos Santos** | Adição de tutorial de instalação no `CONTRIBUTING.md` (onboarding de novos contribuidores), documentação de padrões e guia de contribuição.                           | [Issue #57](https://github.com/GCES-GovHub-2025-2/data-application-gov-hub/issues/57), commits no `CONTRIBUTING.md`                                                                                                                                                                                                                                                                                            | Foco em onboarding e documentação |
| **Lude Ribeiro**            | Implementação completa da Gerência de Configuração, criação de templates YAML, padronização de commits e PRs, documentação de padrões, dependabot, CodeQL e Git Flow. | [PR #52](https://github.com/GCES-GovHub-2025-2/gov-hub/pull/2), [ISSUE](https://github.com/GCES-GovHub-2025-2/GovHub-relatorios/issues/6)                                                                                                                                                                                                                                                                      | Foco em GCES e automação          |

---

## 4. Maiores Avanços

-   Integração inicial de dados de emendas parlamentares via Portal da Transparência.
-   **Implementação de testes abrangentes:** 17 testes (9 unitários + 8 de integração) com 100% de cobertura no ClienteEmendas.
-   CI/CD consolidado e automatizado via GitHub Actions.
-   Padronização documental com ChangeLog e template de commit.
-   Implementação completa da **Gerência de Configuração (GCES)** no repositório:
    -   Git Flow
    -   Versionamento semântico
    -   Releases automatizadas
    -   Dependabot + CodeQL
    -   SonarQube configurado
-   Criação e documentação de **templates YAML** e guias de contribuição.
-   Estrutura de documentação modular em `docs/`, com arquitetura, padrões e troubleshooting.
-   Repositório limpo e protegido contra commits acidentais.

---

## 5. Maiores Dificuldades

-   Ajustes de credenciais e segredos durante a migração de pipelines CI/CD.
-   Integração de múltiplos repositórios com diferentes estruturas de automação.
-   Garantir consistência entre documentação, automação e versionamento.
-   Necessidade de balancear detalhamento técnico e clareza para novos contribuidores.

---

## 6. Lições Aprendidas

-   Ter um **ChangeLog** e um **template de commit** facilita rastreabilidade e revisão de código.
-   Consolidar o **CI/CD cedo** reduz riscos e acelera o ciclo de entrega.
-   **Começar pela camada bronze do DBT** alinha expectativas de schema e qualidade de dados.
-   **Templates de contribuição** (commits, PRs, issues) melhoram a colaboração e reduzem erros.
-   **Testes abrangentes** são fundamentais para confiabilidade, especialmente em pipelines de dados.
-   Uso de **mocks para APIs e bancos de dados** permite validação robusta sem dependências externas.
-   Documentação modular e bem distribuída previne retrabalho e facilita manutenção.

---

## 7. Planejamento para a Próxima Sprint

-   [ ] Implementar primeiros modelos DBT (bronze) a partir do backlog definido.
-   [ ] Evoluir a integração do Portal da Transparência (paginações, limites e enriquecimentos).
-   [ ] Finalizar a persistência e agendamento das DAGs de deputados.
-   [ ] Expandir cobertura de testes para novos módulos.
-   [ ] Configurar proteção de branches após merge do PR principal.
-   [ ] Replicar padrões e automações GCES nos demais repositórios da organização.

---

## 8. Considerações Finais

As Sprints 2 e 3 marcaram uma transição decisiva do projeto GovHub-br para um patamar de maturidade em **Gestão de Configuração e Evolução de Software**.  
Todo o ecossistema foi padronizado e automatizado, com forte ênfase em qualidade, rastreabilidade e sustentabilidade.

O repositório agora apresenta:

-   **Automação robusta** (build, testes, lint, segurança e releases);
-   **Documentação abrangente e modular**;
-   **Padrões de contribuição profissionais**;
-   **Ambiente limpo e seguro** para colaboração contínua.

Essas entregas consolidam o valor técnico do projeto e preparam o GovHub-br para um ciclo sustentável de evolução e colaboração aberta.

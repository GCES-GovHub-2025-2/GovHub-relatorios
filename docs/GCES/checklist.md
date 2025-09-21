# ✅ Checklist do projeto de Gerência de Configuração Evolução de Software

## 📦 Gerência e Controle de Versão

-   [x] Repositório público no GitHub/GitLab (com histórico limpo e organizado)
-   [ ] Uso de `git-flow` ou similar para estratégia de branches
-   [ ] Versionamento semântico (SemVer) aplicado
-   [ ] Tags e releases publicados com **Release Notes** claras
-   [x] GitHub Actions / GitLab CI configurado com:
    -   [ ] Build automatizado
    -   [ ] Testes automatizados (unitários/integrados)
    -   [ ] Linter (ex: ESLint, Flake8, etc.)
    -   [ ] Validação de segurança e dependências (ex: Dependabot, Snyk)
    -   [x] SonarQube ou similar para análise de qualidade.
-   [x] Arquivos de configuração de ambiente: `Dockerfile`, `docker-compose.yml`, `.env.example`

---

## 📚 Documentação

-   [x] `README.md` completo com:
    -   [x] Visão geral do projeto (com prints de como funciona o projeto)
    -   [x] Tecnologias utilizadas
    -   [x] Como rodar localmente (instalação + execução)
    -   [ ] Como contribuir (passo a passo) - getting started - https://blog.discourse.org/tag/getting-started/
    -   [ ] Como usar a aplicação (guia de usuário) - https://blog.discourse.org/tag/getting-started/
    -   [ ] Licença
-   [ ] `CONTRIBUTING.md` com diretrizes de contribuição
-   [ ] `CODE_OF_CONDUCT.md` com boas práticas de convivência
-   [ ] `CHANGELOG.md` com histórico de alterações
-   [x] gitpage com:
    -   [x] Landing page - visão de produto - ex: https://www.discourse.org/
    -   [ ] Arquitetura da solução
    -   [ ] Roadmap e backlog público
    -   [ ] Dicionário de dados (se aplicável)
    -   [ ] Documentação técnica de como contribuir (community)

---

## 📢 Comunicação e Comunidade

-   [ ] Sistema de governança (ex: mantenedores, comitês, votação)
-   [ ] Templates para issues e pull requests
-   [ ] Etiquetas (labels) para organizar issues (ex: good first issue, bug, enhancement) - Obs: não está sendo utilizado
-   [ ] Agendas públicas de reuniões (caso ocorram)

---

## ⚖️ Licenciamento e Aspectos Legais

-   [ ] `LICENSE` com licença de software livre (ex: MIT, GPL, Apache 2.0)
-   [ ] Verificação de licenças das dependências utilizadas
-   [ ] Termos de uso e política de privacidade (para projetos web/app)

---

## 🧪 Qualidade e Testabilidade

-   [ ] Cobertura de testes mínima estabelecida e monitorada
-   [ ] Testes end-to-end automatizados (se aplicável)
-   [x] Ferramentas de análise estática de código
-   [x] Monitoramento de qualidade com badges (ex: Codecov, SonarCloud) - Obs: SonarQube ainda não configurado corretamente.

---

## 📈 Sustentabilidade e Crescimento

-   [ ] Roadmap público com funcionalidades desejadas
-   [ ] Planejamento de onboarding de novos contribuidores (documentacao de onboarding)

---

## 🛠️ Infraestrutura e Deploy (Opcional)

-   [ ] Deploy automatizado (CI/CD) para ambiente de homologação/produção
-   [ ] Infraestrutura como código (IaC) para ambientes cloud (ex: Terraform, Ansible)
-   [ ] Observabilidade básica: logs, métricas e alertas (ex: Prometheus, Grafana, Sentry)

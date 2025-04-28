# ✅ Checklist do projeto de Gerência de Configuração Evolução de Software - Release I 28/04/2025 

### 📦 Gerência e Controle de Versão
- [x] Repositório público no GitHub/GitLab (com histórico limpo e organizado)
- [x] Uso de `git-flow` ou similar para estratégia de branches
- [x] Versionamento semântico (SemVer) aplicado
- [x] Tags e releases publicados com **Release Notes** claras
- [x] GitHub Actions / GitLab CI configurado com:
    - [x] Build automatizado
    - [x] Testes automatizados (unitários/integrados)
    - [x] Linter (ex: ESLint, Flake8, etc.)
    - [ ] Validação de segurança e dependências (ex: Dependabot, Snyk)
- [x] Arquivos de configuração de ambiente: `Dockerfile`, `docker-compose.yml`, `.env.example`

---

### 📚 Documentação
- [X] `README.md` completo com:
    - [X] Visão geral do projeto (com prints de como funciona o projeto)
    - [X] Tecnologias utilizadas
    - [X] Como rodar localmente (instalação + execução)
    - [x] Como contribuir (passo a passo) - getting started - https://blog.discourse.org/tag/getting-started/
    - [ ] Como usar a aplicação  (guia de usuário) - https://blog.discourse.org/tag/getting-started/
    - [X] Licença
- [x] `CONTRIBUTING.md` com diretrizes de contribuição
- [x] `CODE_OF_CONDUCT.md` com boas práticas de convivência
- [ ] `CHANGELOG.md` com histórico de alterações
- [ ] gitpage com:
    - [x] Landing page - visão de produto - ex: https://www.discourse.org/
    - [x] Arquitetura da solução
    - [x] Roadmap e backlog público
    - [ ] Dicionário de dados (se aplicável)
    - [x] Documentação técnica de como contribuir (community)

---

### 📢 Comunicação e Comunidade
- [ ] Sistema de governança (ex: mantenedores, comitês, votação)
- [x] Templates para issues e pull requests
- [x] Etiquetas (labels) para organizar issues (ex: good first issue, bug, enhancement)
- [ ] Agendas públicas de reuniões (caso ocorram)

---

### ⚖️ Licenciamento e Aspectos Legais
- [x] `LICENSE` com licença de software livre (ex: MIT, GPL, Apache 2.0)
- [ ] Verificação de licenças das dependências utilizadas
- [ ] Termos de uso e política de privacidade (para projetos web/app)

---

### 🧪 Qualidade e Testabilidade
- [ ] Cobertura de testes mínima estabelecida e monitorada
- [ ] Testes end-to-end automatizados (se aplicável)
- [ ] Ferramentas de análise estática de código
- [ ] Monitoramento de qualidade com badges (ex: Codecov, SonarCloud)

---

### 📈 Sustentabilidade e Crescimento
- [x] Roadmap público com funcionalidades desejadas
- [ ] Planejamento de onboarding de novos contribuidores (documentacao de onboarding)

---

### 🛠️ Infraestrutura e Deploy (Opcional)
- [ ] Deploy automatizado (CI/CD) para ambiente de homologação/produção
- [ ] Infraestrutura como código (IaC) para ambientes cloud (ex: Terraform, Ansible)
- [ ] Observabilidade básica: logs, métricas e alertas (ex: Prometheus, Grafana, Sentry)
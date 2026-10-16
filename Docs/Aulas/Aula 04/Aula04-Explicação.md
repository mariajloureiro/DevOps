#  Aula 04 - Ferramentas de Integração e Entrega Contínua (CI/CD)

##  Visão Geral da Aula

O objetivo desta aula é apresentar as principais **ferramentas de Integração Contínua (CI)** e **Entrega/Implantação Contínua (CD)**, compreendendo o ecossistema de automação, a criação de pipelines com **GitHub Actions** e as estratégias para garantir a qualidade contínua e previsibilidade na entrega de software.

---

##  Tópicos Abordados

### 1. 🔄 DevOps e o Ciclo Infinito do Software
A cultura DevOps elimina barreiras (*silos*) entre as equipes de **Desenvolvimento (DEV)** e **Operações (OPS)**, organizando o ciclo de vida da aplicação nos seguintes estágios encadeados:

* **PLAN (Planejamento):** Definição de requisitos e backlog (Jira, Trello, Azure Boards).
* **CODE (Codificação):** Escrita de código limpo, testes locais e controle de versão via Git.
* **BUILD (Compilação):** Resolução automática de dependências e empacotamento do artefato executável (JAR, Docker image, pacote NPM).
* **TEST (Testes Automatizados):** Execução de suítes de teste (Unitários, Integração, Performance) para validação imediata do código.
* **RELEASE (Liberação):** Versionamento semântico (`MAJOR.MINOR.PATCH`) e validações de qualidade (*Quality Gates*).
* **DEPLOY (Implantação):** Publicação automatizada em ambientes de homologação ou produção sem *downtime*.
* **OPERATE (Operação):** Gestão de infraestrutura como código (IaC) e orquestração de containers (Kubernetes, Ansible).
* **MONITOR (Monitoramento/Observabilidade):** Coleta de *Métricas* (CPU/memória), *Logs* (erros/ações) e *Traces* (rastreabilidade de requisições).

---

### 2.  Ecossistema de Ferramentas de CI/CD

As plataformas de CI/CD automatizam tarefas repetitivas e reduzem a intervenção manual no processo de publicação. Entre as principais ferramentas do mercado destacam-se:

| Ferramenta | Descrição & Destaques |
| :--- | :--- |
| **GitHub Actions** | Plataforma nativa do GitHub acionada por eventos do repositório (*push*, *pull request*, *tags*). |
| **Azure DevOps** | Solução completa da Microsoft abrangendo gestão ágil, repositórios, pipelines e artefatos. |
| **Jenkins** | Ferramenta *open source* altamente customizável via ecossistema de plugins. |
| **GitLab CI/CD** | Módulo de CI/CD integrado ao ecossistema do GitLab. |
| **Outras Ferramentas** | CircleCI, ArgoCD, Bamboo, Buddy, TeamCity, Spinnaker, Concourse. |

---

### 3.  GitHub Actions e Pipelines

* **O que é um Pipeline?** É a sequência automatizada de estágios responsável por conduzir o software desde o *commit* até o *deploy*.
* **Gatilhos (Events):** Pipelines são disparados automaticamente em resposta a eventos do Git (ex: `push` na branch `main`, abertura de `pull request` ou criação de uma `tag`).
* **Vantagens:** Feedback rápido para os desenvolvedores, detecção precoce de falhas e garantia de qualidade em cada alteração de código.

---

### 4.  Estrutura do Projeto e Organização de Testes

Para garantir que a automação em CI/CD execute com sucesso, a aplicação deve conter uma estrutura organizada de testes na pasta `src/`:

```text
src/
├── components/          # Componentes visuais de interface (ex: DiscountDashboard.jsx)
├── services/            # Regras de negócio da aplicação (ex: discountService.js)
├── tests/               # Suíte de testes automatizados
│   ├── unit/            # Testes unitários de funções/módulos isolados
│   ├── integration/     # Testes de integração entre módulos/APIs
│   └── performance/     # Testes de carga e desempenho
├── App.jsx              # Componente principal do React
└── main.jsx             # Ponto de entrada da aplicação
# Aula 10 - Projeto Final de DevOps

## 📌 Visão Geral do Projeto

O **Projeto Final de DevOps** consiste no desenvolvimento colaborativo em grupo de uma aplicação web completa. O objetivo principal é consolidar e aplicar na prática todos os conceitos, técnicas e ferramentas de DevOps abordados ao longo da disciplina, abrangendo desde o versionamento do código até o monitoramento e deploy automatizado.

---

## 🎯 Objetivos Principais

* **Aplicação Prática:** Vivenciar o ciclo de vida de desenvolvimento de software sob a cultura DevOps.
* **Automação:** Configurar esteiras automatizadas de testes, Integração Contínua ($CI$) e Entrega/Implantação Contínua ($CD$).
* **Padronização:** Garantir a reprodutibilidade de ambientes de desenvolvimento e produção através de contêineres.
* **Qualidade e Monitoramento:** Manter a estabilidade do código com testes automatizados e observabilidade pós-deploy.

---

## 🏗️ Arquitetura e Tema da Aplicação

### **Tema**
* Livre escolha do grupo.
* Deve solucionar um problema ou atender a uma necessidade clara e mensurável.
* Deve ser compatível com os requisitos técnicos da disciplina.

### **Camadas da Arquitetura**
1. **Front-end:** Interface do usuário (UI).
2. **Back-end:** Regras de negócio e rotas/endpoints da API.
3. **Banco de Dados:** Camada de persistência das informações.
4. **Middleware:** Integração, validação ou autenticação (quando aplicável).

---

## 🛠️ Requisitos Técnicos e Práticas Obrigatórias

### 1. Versionamento e Colaboração (Git e GitHub)
* Repositório estruturado contendo código-fonte e documentação.
* Uso de **branches** para organização de *features* e *bugfixes*.
* Histórico de **commits descritivos e organizados**.
* Fluxo de trabalho baseado em **Pull Requests (PRs)** com obrigatoriedade de **code review** por outros integrantes.

### 2. Testes Automatizados
* **Testes Unitários:** Validação isolada de funções, componentes e regras de negócio.
* **Testes de Integração:** Verificação da comunicação entre módulos/serviços.
* **Testes End-to-End (E2E):** Validação dos fluxos críticos do usuário na interface.
* **Testes de Performance:** Avaliação de latência, volume de requisições e taxa de erros.

### 3. Integração Contínua (CI)
* Utilização do **GitHub Actions** (ou ferramenta equivalente autorizada).
* Etapas obrigatórias na pipeline:
  * Instalação de dependências.
  * Validação de sintaxe e estrutura do projeto.
  * Execução automatizada de todas as suítes de teste.
  * Build da aplicação e verificações estáticas de qualidade.

### 4. Containerização e Padronização (Docker)
* Criação de `Dockerfile` para o back-end (e para o front-end, se aplicável).
* Configuração correta de portas, rede e variáveis de ambiente.
* Organização de serviços e dependências (ex.: via `docker-compose`).
* Garantia de execução e demonstração da aplicação containerizada.

### 5. Entrega e Implantação Contínua (CD)
* Construção e publicação automatizada das imagens Docker.
* Processo de **deploy automatizado**.
* Verificação automática de integridade (*healthcheck*) pós-implantação.
* Identificação clara da versão publicada e documentação do processo.

### 6. Observabilidade e Monitoramento
* **Logs:** Registro estruturado de eventos e erros relevantes.
* **Métricas Operacionais:** Acompanhamento de disponibilidade e desempenho.
* Demonstrativo de monitoramento do ambiente em produção ou homologação.

### 7. Configuração e Segurança
* **Separação de responsabilidades:** Separação estrita entre código e configurações do ambiente.
* **Variáveis de Ambiente:** Utilização de arquivos `.env` e disponibilização de um `.env.example` (sem credenciais reais).
* **Gestão de Segredos:** Proteção rigorosa de tokens, senhas e chaves privadas nas pipelines e repositórios.
* Gerenciamento adequado de permissões e checagem de vulnerabilidades.

---

## 📦 Entregáveis do Projeto

1. **Repositório GitHub:** Código-fonte, histórico de commits, branches e PRs revisados.
2. **Suíte de Testes:** Scripts de teste automatizados com evidências de execução.
3. **Pipeline CI/CD:** Arquivos de configuração funcionais do GitHub Actions.
4. **Artefatos Docker:** `Dockerfile` e configurações dos serviços.
5. **Documentação:** Arquivo `README.md` detalhado com instruções de instalação e execução.
6. **Aplicação Implantada:** Endereço público acessível ou script para implantação totalmente reproduzível.
7. **Apresentação Técnica:** Demonstração prática para a turma cobrindo arquitetura, código, testes e esteira de CI/CD.

---

## 🔗 Links e Materiais de Apoio

* **Instruções da Atividade:** [GitHub - Atividade Aula DevOps](https://github.com/deivisontakatu/aula-devops/tree/main/Atividade)
* **Repositório Base DevOps:** [projeto-devops](https://github.com/deivisontakatu/projeto-devops)
* **Exemplo de Docker:** [projeto-docker](https://github.com/deivisontakatu/projeto-docker)
* **Exemplo de Kubernetes:** [projeto-kubernetes](https://github.com/deivisontakatu/projeto-kubernetes)
* **CI/CD com GitHub Actions e Testes:** [projeto-devops-testes](https://github.com/deivisontakatu/projeto-devops-testes)
* **Gerenciamento de Variáveis de Ambiente:** [projeto-variavel-ambiente](https://github.com/deivisontakatu/projeto-variavel-ambiente)

 ## Projeto Final
 (Em produção)
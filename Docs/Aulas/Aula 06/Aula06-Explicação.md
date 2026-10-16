# 🚀 Aula 06 - Revisão de Ferramentas e Pipelines

## Tópicos Abordados

### 1.  DevOps: O Ciclo Infinito do Desenvolvimento Moderno
O DevOps integra as equipes de **Desenvolvimento (DEV)** e **Operações (OPS)** por meio de uma cultura de colaboração e automação[cite: 144]. O ciclo compreende os seguintes estágios:
* **Plan:** Planejamento ágil e gestão de tarefas (Jira, Trello, Azure Boards)[cite: 145].
* **Code:** Codificação colaborativa e controle de versão[cite: 146].
* **Build:** Compilação automatizada e geração de artefatos (JAR, Docker, pacotes NPM)[cite: 147].
* **Test:** Validação contínua com testes automatizados para detectar falhas precocemente[cite: 148].
* **Release:** Controle de versões semânticas (*SemVer*) e *Quality Gates*[cite: 149].
* **Deploy:** Implantação rápida e automatizada nos ambientes de execução[cite: 150].
* **Operate:** Gestão e escalabilidade de infraestrutura (Kubernetes, Ansible)[cite: 151].
* **Monitor:** Observabilidade contínua coletando *métricas*, *logs* e *traces*[cite: 152].

---

### 2.  Estrutura e Regras de um Pipeline
* **Definição:** Sequência de validações automatizadas executadas durante o ciclo de entrega de software[cite: 153].
* **Build uma única vez:** O mesmo artefato gerado é promovido entre os ambientes (Desenvolvimento $\rightarrow$ Homologação $\rightarrow$ Produção)[cite: 153].
* **Fail-Fast (Falhou? Para tudo):** Caso ocorra um erro em qualquer etapa, o fluxo é interrompido imediatamente para evitar a propagação de falhas[cite: 153].

---

### 3.  Estágios do Pipeline
* **Build:** Preparação e compilação do código para execução ou distribuição[cite: 154].
* **Testes:** Execução automática de suítes de testes para preservar funcionalidades existentes[cite: 155].
* **Qualidade:** Verificação de padrões e inconsistências no código[cite: 156].
* **Segurança:** Identificação de vulnerabilidades, dependências inseguras e dados sensíveis expostos[cite: 157].
* **Artefatos (Package):** Empacotamento, versionamento e armazenamento de arquivos de distribuição[cite: 158].
* **Deploy:** Publicação automatizada do software validado no ambiente de destino[cite: 159].
* **Release e Monitoramento:** Disponibilização de versões específicas e monitoramento em tempo real[cite: 160].

---

### 4.  GitHub Actions e Workflows
* **GitHub Actions:** Ferramenta de automação nativa do GitHub para criar fluxos de trabalho associados a eventos do repositório[cite: 163, 166].
* **Gatilhos Comuns (Triggers):** Ações como `push` na branch principal, abertura de `pull requests`, criação de tags ou publicação de releases[cite: 166].
* **Marketplace:** Catálogo de extensões e ferramentas prontas para integrar build, testes, segurança e deploy[cite: 164].

---

##  Atividade Prática da Aula

1. **Implementação de Pipeline:** Configurar uma pipeline utilizando o GitHub Actions para ser executada automaticamente a cada novo `push` na branch principal (`main`)[cite: 167].
2. **Análise de Repositórios:** Pesquisar no GitHub pelo menos três projetos que utilizem integração de Pipeline, documentando suas características, funcionalidades, gatilhos configurados e histórico de execução[cite: 167].

---

##  Referências Bibliográficas

* **HUMBLE, J.; PRIKLANDNICKI, R.** *Entrega Contínua: Como Entregar Software de Forma Rápida e Confiável*. São Paulo: Bookman, 2013[cite: 168].
* **KIM, G. et al.** *Manual de DEVOPS: Como obter agilidade, confiabilidade e segurança em organizações tecnológicas*. São Paulo: Alta Books, 2018[cite: 169].
* **SATO, D.** *DevOps na prática: entrega de software confiável e automatizada*. São Paulo: Casa do Código, 2014[cite: 168].
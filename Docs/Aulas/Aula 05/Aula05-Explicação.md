# 🚀 Aula 05 - Pipeline de Integração Contínua

##  Tópicos Abordados

### 1.  O que é um Pipeline?
Um pipeline consiste em uma sequência de validações e tarefas automatizadas executadas durante o ciclo de entrega de software[cite: 125]. 
* **Regra de Ouro (Build uma única vez):** O mesmo artefato gerado é promovido e implantado em todos os ambientes (Desenvolvimento $\rightarrow$ Homologação $\rightarrow$ Produção)[cite: 125].
* **Fail-Fast (Falhou, para tudo):** Caso ocorra um erro em qualquer etapa, o fluxo é interrompido imediatamente para evitar a propagação de falhas[cite: 125].

---

### 2.  Estágios do Pipeline de CI/CD

Cada alteração de código enviada para o repositório despoleta o fluxo automático passando pelas seguintes etapas:

* **Pipeline de Build:** Prepara o software para execução ou distribuição, realizando a compilação automatizada e gerando artefatos como arquivos `.jar`, `.war`, `.apk` ou imagens Docker[cite: 126].
* **Pipeline de Testes:** Executa automaticamente testes automatizados para assegurar que novas alterações não quebrem funcionalidades já existentes[cite: 127].
* **Pipeline de Qualidade:** Verifica se o código atende rigorosamente aos padrões de qualidade estabelecidos antes de prosseguir[cite: 128].
* **Pipeline de Segurança:** Analisa vulnerabilidades no código, verifica dependências desatualizadas, identifica configurações inseguras e evita a exposição de dados sensíveis[cite: 129].
* **Pipeline de Artefatos (Package):** Empacota, versiona e armazena os artefatos de distribuição gerados no build[cite: 130].
* **Pipeline de Deploy:** Realiza a publicação automática do software validado em um ambiente de execução de destino[cite: 131].
* **Pipeline de Release e Monitoramento:** Cria versões específicas do software para os usuários finais e monitora a aplicação em tempo real no ambiente de produção[cite: 132].

---

### 3.  GitHub Actions e o Marketplace

* **GitHub Actions:** Ferramenta nativa de automação integrada ao GitHub que permite criar workflows acionados por eventos do repositório (como `push`, `pull_request`, criação de tags ou releases)[cite: 135, 138].
* **GitHub Marketplace:** Catálogo oficial de extensões e *Actions* prontas desenvolvidas pela comunidade e parceiros, facilitando a integração de etapas de build, testes, segurança e deploy[cite: 136].

---

## Atividade Prática da Aula

1. **Seleção de Actions:** Escolher **3 Actions** diferentes disponíveis no GitHub Marketplace[cite: 139].
2. **Desenvolvimento do Workflow:** Construir um projeto integrando essas três ferramentas em etapas adequadas de uma pipeline automatizada no GitHub Actions[cite: 139].
3. **Documentação:** Descrever no projeto quais foram as Actions utilizadas, suas respectivas funções e como contribuíram para a automação do fluxo[cite: 139].

---

##  Referências Bibliográficas

* **HUMBLE, J.; PRIKLANDNICKI, R.** *Entrega Contínua: Como Entregar Software de Forma Rápida e Confiável*. São Paulo: Bookman, 2013[cite: 140].
* **KIM, G. et al.** *Manual de DEVOPS: Como obter agilidade, confiabilidade e segurança em organizações tecnológicas*. São Paulo: Alta Books, 2018[cite: 141].
* **SATO, D.** *DevOps na prática: entrega de software confiável e automatizada*. São Paulo: Casa do Código, 2014[cite: 140].
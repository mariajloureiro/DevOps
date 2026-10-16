# 🚀 Aula 03 - Gerência de Configuração e Projetos React
## 📌 Visão Geral da Aula
## Tópicos Abordados

### 1.  O Problema da Gerência de Configuração
* **O Desafio:** Garantir que todos os desenvolvedores da equipe trabalhem exatamente com a mesma configuração (versões idênticas de código, bibliotecas, variáveis de ambiente e bancos de dados)[cite: 218].
* **O Dilema:** Códigos rodando perfeitamente em versões recentes de desenvolvimento (ex: Node 20) podem falhar em ambientes de produção com versões diferentes (ex: Node 18)[cite: 219].

---

### 2.  Itens de Configuração
A configuração engloba todo o conjunto de informações que determina o funcionamento do sistema[cite: 220]:
* **Código:** Arquivos fonte (`.js`, `.java`, `.py`) e scripts da aplicação[cite: 221].
* **Dependências:** Arquivos de gerenciamento de pacotes (`package.json`, `pom.xml`)[cite: 221].
* **Configurações de Ambiente:** Variáveis e parâmetros sensíveis (`.env`, arquivos YAML ou JSON)[cite: 220, 221].
* **Banco de Dados & Infraestrutura:** Scripts SQL, definições de Docker e Terraform[cite: 221].
* **Documentação & Scripts:** Arquivos `README`, scripts de build, teste e deploy[cite: 221].

---

### 3.  Node.js e NPM (Node Package Manager)
* **Node.js:** Ambiente de execução JavaScript no servidor (backend), permitindo unificar a linguagem utilizada no frontend e no backend[cite: 222].
* **NPM:** Gerenciador de pacotes do Node.js responsável por automatizar a instalação, atualização e remoção de bibliotecas[cite: 226].
* **package.json:** Arquivo central que registra as dependências do projeto. Através dele, o comando `npm install` baixa automaticamente todos os pacotes necessários na pasta `node_modules`[cite: 226, 229].

---

### 4.  Criação e Estrutura de Projetos React
Utilização do comando `npx create-react-app` para estruturar uma aplicação React com build via Webpack e Babel[cite: 227]:
* **Passos para execução:**
  1. `npx create-react-app meu-projeto-react`[cite: 228]
  2. `cd meu-projeto-react`[cite: 228]
  3. `code .` (para abrir no VS Code)[cite: 228]
  4. `npm start` (para iniciar o servidor de desenvolvimento local na porta `3000`)[cite: 228, 230]
* **Estrutura de Pastas Principal:**
  * `src/`: Contém os componentes e arquivos JavaScript do projeto (`App.js`, `index.js`, estilos)[cite: 229, 231].
  * `public/`: Contém arquivos públicos, HTML e imagens[cite: 229].
  * `.gitignore`: Define os arquivos e pastas ignorados pelo Git (como senhas e o diretório `node_modules`)[cite: 229].

---

### 5.  Busca por Templates Open Source
Para acelerar o desenvolvimento, pode-se reutilizar modelos validados da comunidade[cite: 232]:
* **GitHub:** Pesquisa de repositórios para clonagem via `git clone <url>`[cite: 232].
* **Vercel:** Busca de templates para download e deploy rápido[cite: 232].
* **CodeSandbox:** Plataforma de templates online interativos[cite: 232].

---

##  Atividade Prática da Aula

1. **Pesquisa e Importação:** Pesquisar e importar um template de projeto desenvolvido em React, realizando as personalizações necessárias e salvando-o em um repositório no GitHub[cite: 233].
2. **Documentação:** Registrar todas as etapas da atividade em um único arquivo, incluindo descrições, capturas de tela (*prints*) e os links de acesso ao repositório no GitHub e ao projeto hospedado na Vercel[cite: 233].

---

##  Referências Bibliográficas

* **BANKS, A.; PORCELLO, E.** *Learning React*. O'Reilly Media, 2017[cite: 227].
* **HUMBLE, J.; PRIKLANDNICKI, R.** *Entrega Contínua: Como Entregar Software de Forma Rápida e Confiável*. São Paulo: Bookman, 2013[cite: 235].
* **KIM, G. et al.** *Manual de DEVOPS: Como obter agilidade, confiabilidade e segurança em organizações tecnológicas*. São Paulo: Alta Books, 2018[cite: 236].
* **MORAES, G.** *Caixa de Ferramentas DevOps*. São Paulo: Casa do Código, 2015[cite: 236].
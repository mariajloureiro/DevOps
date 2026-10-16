# Aula 2: Controle de Versão e Git

## 1. Controle de Versão Distribuído (DVCS)
O Git é um sistema distribuído onde cada desenvolvedor possui um repositório completo em sua máquina local, garantindo autonomia e histórico completo offline.

---

## 2. Fluxos de Trabalho (Git Workflows)

### A. Git Flow
Ideal para projetos com lançamentos agendados e múltiplos ambientes.
* **`main` / `master`:** Código em produção.
* **`develop`:** Código de integração para o próximo lançamento.
* **`feature/*`:** Desenvolvimento de novas funcionalidades.
* **`release/*`:** Preparação e homologação da versão.
* **`hotfix/*`:** Correções urgentes em produção.

### B. Trunk-Based Development
Focado em alta frequência de integração e integração contínua rigorosa.
* Os desenvolvedores integram alterações curtas diretamente no branch principal (`main` ou `trunk`) diariamente.
* Utiliza **Feature Flags / Feature Toggles** para esconder código incompleto em produção.

---

## 3. Boas Práticas no Uso do Git
* **Commits Atômicos:** Cada commit deve realizar apenas uma alteração lógica.
* **Mensagens Claras:** Padrões como *Conventional Commits* (`feat:`, `fix:`, `docs:`).
* **Code Reviews via Pull Requests (PRs):** Garantia de qualidade e transferência de conhecimento antes do merge.
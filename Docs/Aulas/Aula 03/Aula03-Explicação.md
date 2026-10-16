# Aula 3: Integração Contínua (CI) e Entrega Contínua (CD)

## 1. Integração Contínua (CI)
Prática de automatizar a integração de alterações de código de múltiplos colaboradores em um repositório compartilhado.

### Etapas da Pipeline de CI:
1. **Code Checkout:** Baixa o código mais recente.
2. **Linting & Análise Estática:** Verificação de formatação e boas práticas (ex: SonarQube).
3. **Build:** Compilação da aplicação e resolução de dependências.
4. **Automated Tests:** Execução de testes unitários e de integração.

---

## 2. Entrega Contínua (CD) vs. Implantação Contínua (CD)

| Conceito | Descrição | Aprovação em Produção |
| :--- | :--- | :--- |
| **Continuous Delivery** | O código passa por todas as etapas e fica pronto para ir a produção a qualquer momento. | **Manual** (depende de um clique/aprocão) |
| **Continuous Deployment** | O código aprovado em todos os testes vai automaticamente para produção. | **100% Automatizada** |

---

## 3. Estratégias de Deploy
* **Blue-Green Deployment:** Dois ambientes idênticos. O tráfego muda do Blue (atual) para o Green (novo) instantaneamente.
* **Canary Deployment:** O novo código é liberado gradualmente para uma pequena porcentagem dos usuários.
* **Rolling Updates:** Substituição gradual das instâncias velhas pelas novas.
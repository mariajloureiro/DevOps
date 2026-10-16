# 🚀 Aula 07 - Testes Automatizados e Qualidade de Software

##  Tópicos Abordados

### 1.  O que são Testes Automatizados?
São verificações executadas automaticamente por ferramentas para validar o comportamento esperado de uma aplicação[cite: 173]. 
* **Vantagens da Automação:** Redução de erros humanos, aumento da velocidade nas entregas, identificação rápida de falhas logo após alterações no código e garantia de consistência nos cenários de teste[cite: 174].
* **Fail-Fast:** Se uma etapa de teste falhar na pipeline, o fluxo é interrompido imediatamente para evitar que versões com erros avancem para produção[cite: 188].

---

### 2.  Tipos de Testes Aplicados
Os testes técnicos atuam em conjunto para assegurar o funcionamento correto do sistema[cite: 182]:
* **Testes Unitários:** Validam pequenas partes isoladas do código (funções, métodos e componentes), sendo executados rapidamente[cite: 182, 183].
* **Testes de Integração:** Verificam a comunicação eficiente e a troca de informações entre módulos, APIs, serviços e bancos de dados[cite: 182, 184].
* **Testes de Performance:** Avaliam a velocidade, o tempo de resposta e o comportamento da aplicação sob condições de carga e estresse[cite: 182, 185].

---

### 3.  Qualidade de Software e Análise Estática
* **Conceito de Qualidade:** A qualidade deixa de ser exclusividade da fase de testes e passa a integrar todo o ciclo de desenvolvimento, entrega e operação (DevOps)[cite: 186].
* **ESLint:** Ferramenta de análise estática utilizada para identificar problemas de padronização, qualidade e inconsistências em códigos JavaScript diretamente na pipeline de CI[cite: 187].

---

##  Atividade Prática da Aula

1. **Desenvolvimento do Projeto:** Criar um novo projeto estruturado que integre três tipos de testes automatizados: **unitário**, **integração** e **performance**, permitindo que sejam executados e analisados de forma independente[cite: 190].
2. **Configuração da Pipeline:** Criar um arquivo `.yml` utilizando o **GitHub Actions** configurado para ser disparado automaticamente a cada `push` na branch principal (`main`), instalando as dependências e executando os testes[cite: 190].

---

##  Referências Bibliográficas

* **HUMBLE, J.; PRIKLANDNICKI, R.** *Entrega Contínua: Como Entregar Software de Forma Rápida e Confiável*. São Paulo: Bookman, 2013[cite: 191].
* **KIM, G. et al.** *Manual de DEVOPS: Como obter agilidade, confiabilidade e segurança em organizações tecnológicas*. São Paulo: Alta Books, 2018[cite: 192].
* **PIRES, A.; MILITÃO, J.** *Integração Contínua com Jenkins*. São Paulo: Casa do Código, 2019[cite: 192].
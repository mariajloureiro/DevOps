# Aula 6: Infraestrutura como Código (IaC)

## 1. Conceito de IaC
Prática de gerenciar e provisionar a infraestrutura de TI (servidores, redes, bancos de dados) por meio de arquivos de código legíveis por máquina, ao invés de configurações manuais.

---

## 2. Vantagens Principais
* **Reprodutibilidade:** Ambientes de Dev, Staging e Prod idênticos.
* **Rastreabilidade e Versionamento:** Alterações na infraestrutura salvas no Git.
* **Idempotência:** Executar o mesmo código múltiplas vezes garante sempre o mesmo resultado final sem duplicar recursos.

---

## 3. Categorias e Ferramentas

### A. Provisionamento de Infraestrutura (Declarativo)
Descreve **o que** deve ser criado. O estado atual é comparado com o desejado.
* **Exemplos:** Terraform, OpenTofu, AWS CloudFormation.

### B. Gerenciamento de Configuração (Imperativo/Declarativo)
Automação da instalação de softwares e pacotes nos servidores já criados.
* **Exemplos:** Ansible, Puppet, Chef.
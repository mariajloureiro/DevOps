# Aula 9: Documentação de Software em Projetos DevOps

## 1. Importância da Documentação no DevOps
A documentação no ciclo DevOps reduz a dependência de explicações informais e permite que qualquer membro da equipe (ou novos integrantes) execute e entenda o projeto de forma autônoma.

> *"Se eu entrar hoje no GitHub do seu projeto, consigo entender e executá-lo sem perguntar nada para você?"*

### Problemas decorrentes da AUSÊNCIA de documentação:
* Dependência de pessoas específicas ("gargalos de conhecimento").
* Dificuldade no onboarding de novos desenvolvedores.
* Configurações de ambiente executadas de forma inconsistente.
* Maior tempo médio para resolução de problemas (MTTR elevado).
* Perda de conhecimento com a rotatividade da equipe.

---

## 2. As Quatro Necessidades Atendidas pela Documentação
1. **Comunicação:** Compartilhamento claro do conhecimento.
2. **Manutenção:** Facilidade de correção e evolução de código/infra.
3. **Colaboração:** Trabalho em equipe padronizado.
4. **Continuidade:** Redução da dependência de indivíduos isolados.

---

## 3. Tipos de Documentação de Software
* **Documentação Técnica:** Arquitetura, diagramas, APIs, esquemas de banco de dados, variáveis e configurações.
* **Documentação de Projeto:** Requisitos, escopo, objetivos, decisões de design (*ADRs*).
* **Documentação de Processo:** Estratégias de branch, regras de Pull Request, pipelines de CI/CD, deploys e políticas de testes.

---

## 4. Estrutura Essencial de um README.md Profissional

O arquivo `README.md` é a porta de entrada de qualquer repositório. Ele deve conter obrigatoriamente:

1. **Descrição & Propósito:** O que o projeto faz e qual problema resolve.
2. **Tecnologias & Pré-requisitos:** Stack completa, versões mínimas recomendadas (Node, Python, Docker, etc.).
3. **Instalação & Configuração:** Passo a passo sequencial para clonar, instalar dependências e rodar.
4. **Variáveis de Ambiente:** Exemplo de `.env.example` explicitando chaves sem expor dados sensíveis.
5. **Execução & Testes:** Comandos para subir a aplicação e rodar suítes de testes unitários e de integração.
6. **Estrutura de Pastas:** Apresentação da organização de diretórios (`src/`, `tests/`, `.github/workflows/`).

---

## 5. Boas Práticas de Segurança: O que NÃO Documentar
* ❌ Senhas, tokens de acesso ou credenciais de banco de dados.
* ❌ Chaves de API privadas ou segredos de produção.
* ❌ Arquivos `.env` reais ou arquivos de chave privada (`.pem`, `.key`).
* ❌ Dados sensíveis de clientes ou informações pessoais (LGPD/GDPR).
* ❌ Detalhes de infraestrutura interna restrita que representem brechas de segurança.
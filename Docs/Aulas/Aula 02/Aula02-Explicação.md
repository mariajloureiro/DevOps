## Aula 02: Conceitos de Integração e Entrega Contínua de Software

## Conceitos e Tópicos Abordados

1. O Problema da Entrega Tradicional de Software

Antes do DevOps, as equipes de Desenvolvimento (DEV) e Operações/Infraestrutura (OPS) trabalhavam de forma isolada (silos organizacionais).

Cenário Antigo: Testes e deploys manuais, entregas demoradas, muitos erros em produção, instabilidade e a clássica frase: "Funciona na minha máquina, mas dá erro no servidor".

Cenário Atual (DevOps): Testes automatizados, pipelines $CI/CD$ e deploys confiáveis, rápidos, seguros e previsíveis.

2. DevOps: O Ciclo Infinito do Desenvolvimento Moderno

DevOps é uma cultura e filosofia que conecta as fases de desenvolvimento e operação em um fluxo contínuo dividido em 8 etapas:

PLAN (Planejamento): Definição de tarefas e prioridades em metodologias ágeis (ex: Jira, Trello, Azure Boards).

CODE (Codificação): Escrita, revisão e controle de versão do código com boas práticas e testes.

BUILD (Compilação): Transformação do código-fonte em artefatos executáveis (JAR, imagens Docker, pacotes NPM) via compilação e análise estática (SonarQube).

TEST (Testes Automatizados): Execução contínua de testes para garantir qualidade e segurança antes de chegar ao cliente.

RELEASE (Liberação): Versionamento do artefato e aprovação através de Quality Gates.

DEPLOY (Implantação): Publicação automatizada nos ambientes de produção (ex: Kubernetes, AWS EKS, Vercel).

OPERATE (Operação): Gestão da infraestrutura como código ($IaC$), escalabilidade e estabilidade (ex: Ansible, Kubernetes).

MONITOR (Monitoramento & Observabilidade): Coleta contínua de métricas (uso de memória/CPU), logs e traces para alimentar o próximo ciclo de planejamento (ex: Grafana, Graylog).

3. Integração Contínua, Entrega Contínua e Deploy Contínuo

Integração Contínua ($CI$): Prática de integrar o código ao repositório central com frequência. Cada commit dispara automaticamente o build, testes automatizados e análises de qualidade para detectar falhas precocemente.

Entrega Contínua ($CD$ / Continuous Delivery ): Automatiza a preparação do software até a fase de release. O código aprovado está sempre pronto para ir para produção, dependendo apenas da aprovação manual para o deploy final.

Deploy Contínuo ($CD$ / Continuous Deployment ): Publicação totalmente automática das alterações em produção assim que elas passam por todas as validações do pipeline, sem necessidade de intervenção humana.

4. Versionamento Semântico (SemVer)

O Semantic Versioning estabelece uma convenção para indicar claramente a natureza das mudanças no software através do padrão:

$$\text{MAJOR}.\text{MINOR}.\text{PATCH} \quad (\text{Exemplo: } v2.1.3)$$

MAJOR (Ápice): Alterações grandes que causam incompatibilidade com versões anteriores (quebra de API).

MINOR (Incremento): Adição de novas funcionalidades mantendo a compatibilidade (backwards-compatible).

PATCH (Correção): Correções de bugs sem impactar a interface ou funcionalidades existentes.

Tipos de Alteração comuns nos Commits:

Bug Fix: Correção de falhas.

New Feature: Nova funcionalidade.

Feature Enhancement: Melhorias em funções existentes.

Refactoring: Limpeza ou reestruturação do código sem alterar comportamento.

Performance: Otimização de tempo/processamento.

Security Patch: Correções de segurança.

5. Git, VS Code, GitHub e Tags

O Git é um sistema distribuído de controle de versão criado por Linus Torvalds.

Configuração Inicial no Terminal:

git config --global user.name "Seu Nome"
git config --global user.email "seu.email@exemplo.com"


Tags no Git: Marcadores utilizados para identificar pontos chave na história do projeto, como lançamentos de versões (releases).

Tag Leve (Lightweight): Aponta para um commit específico.

Tag Anotada (Annotated): Inclui mensagem, autor e data.

Comandos úteis:

git tag                 # Lista todas as tags
git tag 1.0.0           # Cria uma tag na versão 1.0.0
git push origin 1.0.0   # Envia a tag para o GitHub


6. O que é Deploy e Hospedagem na Vercel

Deploy: Etapa de publicar e disponibilizar a aplicação em um ambiente acessível aos usuários finais.

Vercel: Plataforma moderna otimizada para hospedagem estática e frontend que se conecta diretamente ao GitHub, realizando deploys automáticos e instantâneos a cada git push.

## Atividade Prática da Aula

Configuração e Criação: Configurar o VS Code com Git e criar os arquivos básicos de um projeto web (index.html, style.css e script.js).

Versionamento Inicial: Inicializar o repositório local, realizar o primeiro commit e publicar o projeto em um repositório no GitHub.

Atualização & Tags: Realizar alterações no código, registrar novos commits e atribuir uma Tag indicando a versão (ex: 1.0.0).

Envio: Documentar o fluxo/passo a passo realizado e fazer o envio da atividade na plataforma CANVAS.

## Referências Principais

HUMBLE, J.; PRIKLANDNICKI, R. Entrega Contínua: Como Entregar Software de Forma Rápida e Confiável. São Paulo: Bookman, 2013.

KIM, G. et al. Manual de DEVOPS: Como obter agilidade, confiabilidade e segurança em organizações tecnológicas. São Paulo: Alta Books, 2018.

SATO, D. DevOps na prática: entrega de software confiável e automatizada. São Paulo: Casa do Código, 2014.
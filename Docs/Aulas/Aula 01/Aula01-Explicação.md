## Aula 01: Apresentação da Disciplina e Introdução ao DevOps
 ## Conceitos e Tópicos Abordados

1. Versionamento de Código e Deploy

O Controle de Versões é a prática de registrar alterações em arquivos ao longo do tempo.

Benefícios: Permite recuperar versões anteriores, rastrear modificações e viabilizar a colaboração em equipe por meio de branches (ramificações).

Plataformas Utilizadas: GitHub, GitLab e Bitbucket.

Deploy: Métodos de implantação de código em ambientes de desenvolvimento, homologação e produção.

2. Automação de Pipelines & CI/CD

Um Pipeline representa a sequência automatizada de etapas desde a escrita do código até a sua disponibilização em produção.

Automação: Reduz erros humanos, automatiza tarefas repetitivas (compilação, testes, análises) e fornece feedback rápido para o time.

Integração Contínua ($CI$): Prática de integrar o código ao repositório principal com frequência. Cada alteração dispara compilações e testes automatizados para identificar falhas precocemente.

Entrega Contínua ($CD$): Garante que, após aprovado nos testes, o software esteja sempre em estado de publicação de forma rápida, estável e segura.

3. Qualidade de Software e Testes Automatizados

A qualidade do código é validada durante todo o ciclo de desenvolvimento:

Análise Automatizada: Valida padronização, complexidade, segurança, cobertura de testes e vulnerabilidades.

Categorias de Testes Automatizados:

Testes Unitários: Validação de pequenas unidades isoladas de código.

Testes de Integração: Validação da comunicação entre diferentes módulos.

Testes Funcionais & End-to-End ($E2E$): Validação do fluxo completo do ponto de vista do usuário final.

4. Containers e Estratégias de Implantação

Containers (Docker): Empacotam a aplicação juntamente com todas as suas dependências em um ambiente padronizado, garantindo paridade entre desenvolvimento, testes e produção.

Estratégias de Deploy:

Rolling Update: Atualização gradual das instâncias da aplicação.

Blue-Green Deployment: Uso de dois ambientes idênticos para trocar o tráfego instantaneamente.

Canary Release: Liberação de novas versões para um pequeno grupo de usuários antes do rollout total.

## Critérios de Avaliação da Disciplina

A nota final da disciplina será calculada utilizando a seguinte fórmula:

$$\text{Média Final} = (P1 \times 0,25) + (P2 \times 0,25) + ((PJ + AT) \times 0,25)$$

$P1$: Prova 1

$P2$: Prova 2

$PJ$: Projeto

$AT$: Atividades Semanais

## Atividade Prática em Grupo

Formação de Grupos: Grupos de 3 a 5 integrantes fixos para as entregas do semestre.

Repositório no GitHub: Criação do repositório principal do grupo para armazenar os exercícios da disciplina.

Arquivo README: Elaboração do resumo da Aula 01 em padrão Markdown.

Avaliação Diagnóstica: Preenchimento do formulário inicial disponibilizado pelo professor.

## Referências Principais

HUMBLE, J.; PRIKLANDNICKI, R. Entrega Contínua: Como Entregar Software de Forma Rápida e Confiável. São Paulo: Bookman, 2013.

KIM, G. et al. Manual de DEVOPS: Como obter agilidade, confiabilidade e segurança em organizações tecnológicas. São Paulo: Alta Books, 2018.

SATO, D. DevOps na prática: entrega de software confiável e automatizada. São Paulo: Casa do Código, 2014.
# Aula 5: Orquestração com Kubernetes (K8s)

## 1. Por que usar Orquestração?
Quando a quantidade de containers cresce em produção, é necessário automação para:
* Escalonamento automático (*Auto-scaling*).
* Alta disponibilidade e recuperação de falhas (*Self-healing*).
* Balanceamento de carga (*Load Balancing*).
* Atualizações sem interrupção de serviço (*Zero-downtime deploys*).

---

## 2. Arquitetura do Kubernetes

### Control Plane (Master Node)
* **kube-apiserver:** Ponto central de comunicação da API.
* **etcd:** Banco de dados chave-valor para estado do cluster.
* **kube-scheduler:** Aloca Pods nos Worker Nodes disponíveis.
* **kube-controller-manager:** Garante que o estado atual seja igual ao desejado.

### Worker Nodes
* **kubelet:** Agente local que garante a execução dos containers.
* **kube-proxy:** Gerencia regras de rede e roteamento.
* **Container Runtime:** Motor de containerização (ex: `containerd`).

---

## 3. Principais Objetos K8s
* **Pod:** Menor unidade do K8s; encapsula um ou mais containers compartilhando rede e armazenamento.
* **Deployment:** Define o estado desejado dos Pods (número de réplicas, versão da imagem).
* **Service:** Endereço de rede estável (ClusterIP, NodePort, LoadBalancer) para expor e balancear os Pods.
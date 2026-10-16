# Aula 4: Containerização com Docker

## 1. Containers vs. Máquinas Virtuais (VMs)

* **Máquinas Virtuais:** Incluem o SO convidado (*Guest OS*) completo sobre um hypervisor. Consomem mais memória, disco e tempo de boot.
* **Containers:** Compartilham o Kernel do sistema operacional hospedeiro. São extremamente leves, inicializam em segundos e garantem o famoso princípio *"funciona na minha máquina, funciona em produção"*.

---

## 2. Conceitos Fundamentais do Docker

* **Dockerfile:** Arquivo declarativo com as instruções passo a passo para criar a imagem.
* **Imagem:** Pacote estático, somente leitura, contendo código, runtime, bibliotecas e variáveis de ambiente.
* **Container:** A instância em execução de uma imagem.
* **Volume:** Mecanismo para persistência de dados fora do ciclo de vida do container.
* **Network:** Isolamento e comunicação entre containers.

---

## 3. Exemplo Prático de Dockerfile
```dockerfile
FROM node:18-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 3000
CMD ["npm", "start"]
```

---

## 4. Docker Compose
Ferramenta para definir e rodar aplicações multi-container usando um arquivo `docker-compose.yml` unificado.
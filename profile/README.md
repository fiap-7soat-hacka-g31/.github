# FIAP X

## FIAP - Software Architecture Hackaton - Fase 5

Este projeto foi desenvolvido durante a `Fase V` do curso de `Arquitetura de Software` da FIAP como requisito para avaliação.

## Integrantes do Grupo
- Julio Augusto Silva (RM355432)
- Lucas Henrique de Oliveira Silva (RM354904)
- Getúlio Magela Silva (RM355427)
- Lucas Rego Lima (RM356101)
- Lilian Rosario de Jesus (RM355928)

## Apresentação em Vídeo

- [Assistir no YouTube](link:TODO)

## Diagramas

### Event Storming :[Ver no Miro 👁️](https://miro.com/app/board/o9J_lHsdpmE=/?moveToWidget=3458764614656328237&cot=10):

![Event Storming](../resources/event-storming.png)

### Arquitetura Cloud :[Ver no Miro 👁️](https://miro.com/app/board/o9J_lHsdpmE=/?moveToWidget=3458764614649572419&cot=10):

![Cloud Architecture](../resources/cloud-architecture.png)

## Serviços:

### Fiap X API

Serviço responsável por gerenciar as postagens de vídeos criando URLs assinadas para upload e a gestão do conteúdo como listagem e download.

### Fiap X Worker

Serviço responsável por realizar o processamento de imagens a partir de arquivos de vídeo.

### Fiap X Identity

Serviço de autenticação permitindo o cadastro, solicitações de acesso e verificação de tokens de acesso.

### Fiap X Notifications

Serviço responsável pelo envio de notificações de sucesso ou falha no processamento dos vídeos enviados.

## Repositórios da solução:

- Provisionamento de infraestrutura de banco de dados MongoDB com terraform: [Ver repositório](https://github.com/fiap-7soat-hacka-g31/soat7-hacka-fiap-x-mongodb)
- Provisionamento de infraestrutura de Kubernetes com terraform: [Ver repositório](https://github.com/fiap-7soat-hacka-g31/soat7-hacka-fiap-x-k8s)
- Provisionamento de infraestrutura de APIGateway com terraform: [Ver repositório](https://github.com/fiap-7soat-hacka-g31/soat7-hacka-fiap-x-gateway)
- Serviço de mensageria RabbitMQ dentro do cluster Kubernetes: [Ver repositório](https://github.com/fiap-7soat-hacka-g31/soat7-hacka-fiap-x-rabbitmq)
- Serviço FIAP X Identity: [Ver repositório](https://github.com/fiap-7soat-hacka-g31/soat7-hacka-fiap-x-identity)
- Serviço FIAP X API: [Ver repositório](https://github.com/fiap-7soat-hacka-g31/soat7-hacka-fiap-x-api)
- Serviço FIAP X Worker: [Ver repositório](https://github.com/fiap-7soat-hacka-g31/soat7-hacka-fiap-x-worker)
- Serviço FIAP X Notification: [Ver repositório](https://github.com/fiap-7soat-hacka-g31/soat7-hacka-fiap-x-notifications)

## CICD e DevOps

- Todos os repositórios estão com esteiras automatizadas para implantação.
- Todos os repositórios possuem proteções na branch principal (main), requisitando Pull Request com duas aprovações e que todos os checks de pipe tenham passado antes de realizar o merge.

## OpenAPI - Swagger

- Todos os serviços possuem Swagger disponibilizados na rota `/docs` que pode ser acessada com o serviço em execução. Contudo apenas os serviços FiapXAPI e FiapXIdentity possuem integração por HTTP, tornando-os mais enriquecidos.

## Requisitos:

### Requisitos Funcionais:

- Autenticação
- Upload de arquivos de vídeo
- Download de arquivos
- Notificações de processamento

### Não Funcionais:

- Infraestrutura provisionada por esteiras automatizadas
- Ambiente em núvem - Aws
- Resiliencia
- Proteção das branches principais
- Cobertura de 80% de código
- Disposição de Microserviços

## Evidências:

### Fiap X API

#### Pipeline
![Event Storming](../resources/evidence/fiap-x-api-pipeline.png)

#### Unit Tests

![Event Storming](../resources/evidence/fiap-x-api-unit-test.png)

#### Integration Testes

![Event Storming](../resources/evidence/fiap-x-api-integration-test.png)

### Fiap X Worker

#### Pipeline
![Event Storming](../resources/evidence/fiap-x-worker-pipeline.png)

#### Unit Tests

![Event Storming](../resources/evidence/fiap-x-worker-unit-test.png)

#### Integration Testes

![Event Storming](../resources/evidence/fiap-x-worker-integration-test.png)

### Fiap X Identity

#### Pipeline
![Event Storming](../resources/evidence/fiap-x-identity-pipeline.png)

#### Unit Tests

![Event Storming](../resources/evidence/fiap-x-identity-unit-test.png)

#### Integration Testes

![Event Storming](../resources/evidence/fiap-x-identity-integration-test.png)

### Fiap X Notifications

#### Pipeline
![Event Storming](../resources/evidence/fiap-x-notifications-pipeline.png)

#### Unit Tests

![Event Storming](../resources/evidence/fiap-x-notifications-unit-test.png)

#### Integration Testes

![Event Storming](../resources/evidence/fiap-x-notifications-integration-test.png)

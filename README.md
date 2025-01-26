# FIAP X

## FIAP - Software Architecture Hackaton - Fase 5
Este projeto foi desenvolvido durante a `Fase V` do curso de `Arquitetura de Software` da FIAP como requisito para avaliação.

## Integrantes do Grupo
- Getúlio Magela Silva - RM355427

## Apresentação em Vídeo
- [Assistir no YouTube](link:TODO)

## Diagramas

### Event Storming :[Ver no Miro 👁️](link):
![Event Storming](../docs/resources/event-storming.png)

### Arquitetura Cloud :[Ver no Miro 👁️](link):
![Cloud Architecture](../docs/resources/cloud-architecture.png)

## Serviços:

### Fiap X API
TODO

### Fiap X Worker
TODO

### Fiap X Identity
TODO

### Fiap X Notifications
TODO

## Repositórios da solução:
- Provisionamento de infraestrutura de Kubernetes com terraform: [Ver repositório](link:TODO)
- Provisionamento de infraestrutura de banco de dados MongoDB com terraform: [Ver repositório](link:TODO)
- Serviço de mensageria RabbitMQ dentro do cluster Kubernetes: [Ver repositório](link:TODO)
- Serviço FIAP X Identity: [Ver repositório](link:TODO)
- Serviço FIAP X API: [Ver repositório](link:TODO)
- Serviço FIAP X Worker: [Ver repositório](link:TODO)
- Serviço FIAP X Notification: [Ver repositório](link:TODO)

## CICD e DevOps
- Todos os repositórios estão com esteiras automatizadas para implantação.
- Todos os repositórios possuem proteções na branch principal (main), requisitando Pull Request com duas aprovações e que todos os checks de pipe tenham passado antes de realizar o merge.

## OpenAPI - Swagger
- O serviços FiapXApi e FiapXIdentity possuem disponíveis na rota `/docs` com o serviço em execução.

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
TODO
#### Unit Tests
TODO
#### Integration Testes
TODO


### Fiap X Worker
#### Pipeline
TODO
#### Unit Tests
TODO
#### Integration Testes
TODO


### Fiap X Identity
#### Pipeline
TODO
#### Unit Tests
TODO
#### Integration Testes
TODO


### Fiap X Notifications
#### Pipeline
TODO
#### Unit Tests
TODO
#### Integration Testes
TODO

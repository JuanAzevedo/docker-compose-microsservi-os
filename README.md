# Orquestração dos Microserviços com Docker Compose

Este repositório é responsável por orquestrar os microserviços de eventos e de banco de dados usando Docker Compose.

## Pré-requisitos

- Docker
- Docker Compose

## Configuração e Execução

### Clonagem dos Repositórios

Antes de iniciar, clone todos os repositórios necessários:

```bash
mkdir meu-projeto
cd meu-projeto
git clone https://github.com/JuanAzevedo/docker-compose-microsservicos.git
git clone https://github.com/JuanAzevedo/api_eventos.git
git clone https://github.com/JuanAzevedo/api_database.git
```

### Inicialização
Navegue até o diretório do Docker Compose e execute:
```bash
cd docker-compose-microsservicos
docker-compose up --build
```

Isto irá construir e levantar todos os serviços definidos no arquivo docker-compose.yml.

### Finalização
Para interromper e remover os containers, além de redes e volumes, utilize:
```bash
docker-compose down --volumes --remove-orphans
```
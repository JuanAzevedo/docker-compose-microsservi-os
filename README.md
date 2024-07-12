# Microservices Docker Compose

Este repositório contém a configuração Docker Compose para orquestrar os serviços de eventos e banco de dados.

## Estrutura

Os serviços são organizados em repositórios separados e incluídos aqui como submódulos:
- API de Eventos: [api_eventos](https://github.com/JuanAzevedo/api_eventos.git)
- API de Banco de Dados: [api_database](https://github.com/JuanAzevedo/api_database.git)

## Como Executar

1. Clone este repositório:
   ```bash
   git clone --recurse-submodules https://github.com/JuanAzevedo/docker-compose-microsservicos.git

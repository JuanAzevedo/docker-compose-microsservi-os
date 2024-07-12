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
2. Navegue até o diretório do projeto:
   cd docker-compose-microsservicos
3. Construa e inicie os serviços com Docker Compose:
   docker-compose up --build
   
   Isso iniciará os serviços api_eventos na porta 5000 e api_database na porta 5001. A comunicação entre os serviços ocorre automaticamente através da rede definida no Docker Compose.
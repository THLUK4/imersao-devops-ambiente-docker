# Imersão DevOps - Ambiente Docker (Alura + Google Cloud)

Projeto desenvolvido durante a Imersão DevOps da Alura em parceria com o Google Cloud. O objetivo é criar um ambiente de desenvolvimento completo e portável para uma API em Python utilizando Docker.

## 🚀 Tecnologias Utilizadas

- **Linguagem:** Python
- **Containerização:** Docker & Docker Compose
- **Cloud:** Google Cloud (próximos passos)

## 💻 Como Rodar o Projeto Localmente

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/THLUK4/imersao-devops-ambiente-docker.git](https://github.com/seu-usuario/imersao-devops-ambiente-docker.git)
    cd imersao-devops-ambiente-docker
    ```

2.  **Suba os containers com Docker Compose:**
    ```bash
    docker-compose up --build
    ```

3.  **Acesse a API** em `http://localhost:8000` (ou a porta que você configurou).

## 📂 Estrutura do Projeto

**imersao-devops-ambiente-docker/**

|-- .dockerignore          # Lista de arquivos e pastas para o Docker ignorar durante o build da imagem.
|-- .gitignore             # Lista de arquivos e pastas para o Git ignorar (não enviar ao repositório).
|-- Dockerfile             # "Receita" passo a passo para construir a imagem Docker da sua aplicação.
|-- docker-compose.yml     # Orqaaaauestrador para definir e rodar os serviços da aplicação (ex: a API, um banco de dados).
|-- requirements.txt       # Lista todas as bibliotecas Python que o projeto precisa para funcionar.
|-- README.md              # Documentação principal do projeto (o que é, como instalar, como usar).
|-- escola.db              # Arquivo do banco de dados SQLite.
|
|-- app.py                 # Ponto de entrada principal da aplicação, onde o servidor web é iniciado.
|-- database.py            # Módulo para configurar a conexão com o banco de dados.
|-- models.py              # Define a estrutura das tabelas do banco de dados como classes Python (ex: SQLAlchemy).
|-- schemas.py             # Define a estrutura dos dados de entrada e saída da API (ex: Pydantic).
|
|-- /routers/              # Pasta que organiza os diferentes grupos de rotas (endpoints) da sua API.
|                            (ex: alunos_router.py, cursos_router.py)
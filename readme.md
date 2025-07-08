# Imersão DevOps - Ambiente Docker (Alura + Google Cloud)

Projeto desenvolvido durante a Imersão DevOps da Alura em parceria com o Google Cloud. O objetivo é criar um ambiente de desenvolvimento completo e portável para uma API em Python utilizando Docker.

## 🚀 Tecnologias Utilizadas

- **Linguagem:** Python
- **Containerização:** Docker & Docker Compose
- **Cloud:** Google Cloud (próximos passos)

## 💻 Como Rodar o Projeto Localmente

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/THLUK4/imersao-devops-ambiente-docker.git
    cd imersao-devops-ambiente-docker
    ```

2.  **Suba os containers com Docker Compose:**
    ```bash
    docker-compose up --build
    ```

3.  **Acesse a API** em `http://localhost:8000` (ou a porta que você configurou).

## 📂 Estrutura do Projeto

```
imersao-devops-ambiente-docker/
├── .dockerignore        # Ignora arquivos no build do Docker
├── .gitignore           # Ignora arquivos no versionamento do Git
├── Dockerfile           # Receita para construir a imagem da aplicação
├── docker-compose.yml   # Orquestrador dos serviços (API, DB, etc.)
├── requirements.txt     # Dependências Python do projeto
├── README.md            # Documentação principal
├── escola.db            # Banco de dados SQLite (desenvolvimento)
│
├── app.py               # Ponto de entrada da aplicação (FastAPI)
├── database.py          # Configuração e sessão do banco de dados
├── models.py            # Modelos de dados da aplicação (tabelas)
├── schemas.py           # Schemas para validação e serialização de dados
│
└── /routers/            # Pasta com os endpoints/rotas da API
    └── ... (ex: alunos_router.py, cursos_router.py)
```

# CollabHubBR - Badge System

![GitHub License](https://img.shields.io/github/license/CollabHubBR/bagde-system?labelColor=101010)

Este repositório contém o código-fonte do **Microsserviço de Badges** do **[CollabHubBR](https://github.com/CollabHubBR)**, uma plataforma brasileira para coordenação de projetos open source. Desenvolvido em **Go** com o framework **Fiber**, este serviço gerencia e associa badges, conquistas e marcos para usuários e projetos.

## 📌 Funcionalidades

-   Gestão de badges por usuário e por projeto
-   Registro e recuperação de conquistas
-   Integração com outros microsserviços do CollabHubBR

## 🛠️ Stack Tecnológica

![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)

![Fiber](https://img.shields.io/badge/Fiber-000000?style=for-the-badge&logo=fiber&logoColor=white)

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)

![Docker](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)

![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088ff?style=for-the-badge&logo=github-actions&logoColor=white)

![GitHub](https://img.shields.io/badge/GitHub-fff?style=for-the-badge&logo=github&logoColor=181717)

## 📁 Estrutura de Pastas

```
├── cmd/                  # Arquivo principal para inicialização do app
├── config/               # Configurações da aplicação (env, banco, etc)
├── controllers/          # Handlers HTTP (rotas)
├── models/               # Definições das entidades do sistema
├── repositories/         # Acesso ao banco de dados
├── services/             # Lógica de negócio (core do microsserviço)
├── routes/               # Registro e organização de rotas
├── utils/                # Funções auxiliares e helpers
├── docker-compose.yml    # Docker banco de dados
├── go.mod                # Dependências do projeto
└── README.md             # Documentação
```

## ⚙️ Configuração e Execução

### 1. Clone o Repositório

```bash
git clone https://github.com/CollabHubBR/badges-service.git
cd badges-service
```

### 2. Configure as Variáveis de Ambiente

Crie um arquivo `.env` com as configurações necessárias:

```
DATABASE_URL=postgres://user:password@localhost:5432/badges_db
PORT=3000
```

### 3. Execute Localmente

```
go run cmd/main.go
```

### 4. Docker (opcional)

```
docker build -t collabhub-badges .
docker run -p 3000:3000 --env-file .env collabhub-badges
```

## 🧪 Testes

Para rodar os testes (se implementados):

```
go test ./...
```

## 📌 To-Do

Confira a [lista de tarefas](https://github.com/CollabHubBR/badge-system/blob/main/.github/TODO.md)

## 🤝 Contribuindo

Antes de contribuir, leia os seguintes documentos:

-   [Código de Conduta](https://github.com/CollabHubBR/.github/blob/main/CODE_OF_CONDUCT.md)
-   [Contribuindo](https://github.com/CollabHubBR/.github/blob/main/CONTRIBUTING.md)
-   [Segurança](https://github.com/CollabHubBR/.github/blob/main/SECURITY.md)
-   [Suporte](https://github.com/CollabHubBR/.github/blob/main/SUPPORT.md)

## 📄 Licença

Distribuído sob a licença [MIT](https://choosealicense.com/licenses/mit/). Veja o arquivo `LICENSE` para mais informações.

---

🚀 **CollabHubBR** – Unindo a comunidade open source brasileira!

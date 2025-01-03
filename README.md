# E-Commerce API

![.NET](https://img.shields.io/badge/.NET-9.0-blue?style=flat-square&logo=.net) ![Clean Architecture](https://img.shields.io/badge/Architecture-Clean-blueviolet?style=flat-square) ![Entity Framework Core](https://img.shields.io/badge/EF%20Core-9.0-green?style=flat-square) ![SpecFlow](https://img.shields.io/badge/BDD-ReqnRoll-orange?style=flat-square)

## Versão
![Version](https://img.shields.io/badge/version-1.0.0-blue?style=flat-square)

## Descrição
A **E-Commerce API** é uma aplicação baseada em arquitetura limpa (Clean Architecture),
desenvolvida em **.NET 9**, para gerenciar operações de um e-commerce. A solução foca em
separação de responsabilidades e escalabilidade, utilizando padrões como Repository, Unit of
Work e injeção de dependências.

## Features
- **Cadastro de Produtos**: CRUD completo para gerenciar produtos.
- **Gerenciamento de Usuários**: Sistema de autenticação e autorização com JWT.
- **Checkout**: Integração com serviços de pagamento como Stripe.
- **BDD (Behavior-Driven Development)**: Testes automatizados com ReqnRoll e Gherkin.
- **Logs Estruturados**: Monitoramento usando Serilog.

## Estrutura do Projeto
A solução segue os princípios da arquitetura limpa:
```
ECommerceAPI/
├── src/
│   ├── ECommerce.API/                # Camada de apresentação
│   ├── ECommerce.Application/       # Camada de aplicação
│   ├── ECommerce.Domain/            # Camada de domínio
│   ├── ECommerce.Infrastructure/    # Camada de infraestrutura
├── tests/
│   ├── ECommerce.API.Tests/         # Testes da API 
│   ├── ECommerce.Application.Tests/ # Testes da aplicação
│   ├── ECommerce.Domain.Tests/      # Testes do domínio
│   ├── ECommerce.BDD.Tests/         # Testes BDD
├── README.md                        # Documentação do projeto
└── ECommerceAPI.sln                    # Solução
```

## Tecnologias Usadas
- **Linguagem**: C#
- **Framework**: .NET 9
- **Banco de Dados**: PostgreSQL
- **ORM**: Entity Framework Core
- **Autenticação**: JWT
- **Testes**: ReqnRoll, NUnit
- **Logs**: Serilog

## Como Executar o Projeto
1. Clone o repositório:
   ```bash
   git clone https://github.com/math3ussdl/ECommerceAPI.git
   cd ECommerceAPI
   ```
2. Restaure os pacotes:
   ```bash
   dotnet restore
   ```
3. Configure o banco de dados em `appsettings.json`.
4. Execute as migrações:
   ```bash
   dotnet ef database update --project src/ECommerce.Infrastructure
   ```
5. Execute a API:
   ```bash
   dotnet run --project src/ECommerce.API
   ```

## Autor
**Hugo Lima**  
Desenvolvedor Web
[GitHub](https://github.com/math3ussdl/) | [LinkedIn](https://linkedin.com/in/math3ussdl/)

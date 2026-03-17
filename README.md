# 🛒 Controle de Estoque e Caixa — Loja

Sistema web para gerenciamento de estoque e controle de caixa de pequenas lojas, desenvolvido com **ASP.NET Core MVC** e **Entity Framework Core**.

---

## 🚀 Tecnologias

| Tecnologia | Versão |
|---|---|
| .NET | 10.0 |
| ASP.NET Core MVC | 10.0 |
| Entity Framework Core | 10.0 |
| SQLite | — |
| Razor Pages (Runtime Compilation) | 10.0 |

---

## ✨ Funcionalidades

- 📦 **Controle de Estoque** — Cadastro e gerenciamento de produtos
- 💰 **Controle de Caixa** — Registro de entradas e saídas financeiras
- 🗃️ **Banco de Dados Local** — Armazenamento com SQLite, sem necessidade de servidor externo
- 🔄 **Criação automática do banco** — Estrutura criada na primeira execução via `EnsureCreated()`

---

## 🏗️ Arquitetura

O projeto segue o padrão **MVC (Model-View-Controller)**:

```
ControleEstoqueLoja/
├── Controllers/       # Lógica de requisição e resposta
├── Models/            # Entidades do domínio
├── Views/             # Interface com Razor
├── Data/              # ApplicationDbContext (EF Core)
├── Migrations/        # Histórico de migrações do banco
├── appsettings.json   # Configurações da aplicação
└── Program.cs         # Ponto de entrada e configuração de serviços
```

---

## ⚙️ Como Executar Localmente

**Pré-requisitos:** [.NET 10 SDK](https://dotnet.microsoft.com/download)

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/ControleEstoqueLoja.git
cd ControleEstoqueLoja

# Restaure as dependências
dotnet restore

# Execute o projeto
dotnet run
```

Acesse em: `https://localhost:5001` ou `http://localhost:5000`

> O banco de dados SQLite (`controleestoque.db`) é criado automaticamente na primeira execução.

---

## 📌 Destaques Técnicos

- **Injeção de Dependência** nativa do ASP.NET Core para o `DbContext`
- **Code-First** com Entity Framework Core e migrations versionadas
- **Razor Runtime Compilation** habilitado para agilizar o desenvolvimento
- **Banco de dados embutido** (SQLite) — ideal para deploy simplificado

---

## 📄 Licença

Este projeto foi desenvolvido para fins de estudo e portfólio.

---

> Desenvolvido com C# e .NET 10 🔷

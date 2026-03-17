# 🛒 Controle de Estoque e Caixa

http://controle-estoque-loja.runasp.net

Sistema web para gerenciamento de estoque e caixa de pequenas lojas, desenvolvido com **ASP.NET Core MVC** e **Entity Framework Core**.

## 🚀 Tecnologias

- .NET 10 / ASP.NET Core MVC
- Entity Framework Core 10 (Code-First)
- SQLite
- Razor Views com Runtime Compilation

## ✨ Funcionalidades

- 📦 Cadastro e controle de produtos em estoque
- 💰 Registro de entradas e saídas no caixa
- 🗃️ Banco de dados local (SQLite) criado automaticamente na primeira execução

## ⚙️ Como Executar

**Pré-requisito:** [.NET 10 SDK](https://dotnet.microsoft.com/download)

```bash
git clone https://github.com/seu-usuario/ControleEstoqueLoja.git
cd ControleEstoqueLoja
dotnet run
```

Acesse em `http://localhost:5000` — o banco é criado automaticamente.

## 🏗️ Arquitetura

Padrão MVC com separação em `Controllers`, `Models`, `Views` e `Data` (DbContext). Injeção de dependência nativa do ASP.NET Core.

---

> Desenvolvido com C# e .NET 10 🔷

## ⌨️ Atalhos do Sistema

O sistema possui atalhos de teclado para agilizar o uso no dia a dia do operador de caixa:

| Atalho | Função |
|---|---|
| `Alt + M` | Abre o Menu Administrativo |
| `Alt + C` | Navega para o Caixa |
| `Alt + H` | Navega para o Histórico de Vendas |
| `Alt + E` | Navega para o Controle de Estoque |
| `ESC` | Abre/fecha o painel de ajuda com todos os atalhos |

### Menu Administrativo (Alt + M)

Ao pressionar `Alt + M`, um modal é exibido com as seguintes opções, acessíveis também pelos números do teclado:

| Tecla | Função |
|---|---|
| `1` | 💸 Sangria — retirada de dinheiro do caixa |
| `2` | 📥 Suprimento — entrada de dinheiro no caixa |
| `3` | 🏧 Status do Caixa |
| `4` | 🔒 Fechamento do Caixa |
| `5` | 📊 Relatório do Caixa |
| `6` | 🖨️ Reimprimir última venda |
| `7` | 👥 Gerenciar Vendedores |

# 🛒 Controle de Estoque e Caixa

Sistema web para gerenciamento de estoque e caixa de pequenas lojas, desenvolvido com **ASP.NET Core MVC** e **Entity Framework Core**.

## 🌐 Demo

Acesse o sistema em produção: **[http://controle-estoque-loja.runasp.net](http://controle-estoque-loja.runasp.net)**

> O banco de dados é criado automaticamente na primeira execução.

---

## 🚀 Tecnologias

- .NET 10 / ASP.NET Core MVC
- Entity Framework Core 10 (Code-First)
- SQLite
- Razor Views com Runtime Compilation
- SweetAlert2

---

## 📦 Módulo de Estoque

- Listagem de todos os produtos com busca por nome
- Cadastro de produto com os campos: nome, tipo, quantidade, preço e código de barras
- Edição de produto existente
- Exclusão de produto
- Movimentação de estoque (entrada e saída de quantidade)
- Produtos organizados por tipo: **Granel**, **Prateleira**, **Geladeira** e **Freezer**

---

## 💰 Módulo de Caixa

### Realizando uma Venda
1. Acesse o **Caixa** (`Alt + C`)
2. Busque o produto pelo nome ou leia o código de barras
3. Adicione os itens ao carrinho
4. Informe o método de pagamento e o valor recebido
5. Finalize a venda — o sistema calcula o troco automaticamente
6. O cupom fiscal é gerado para impressão

> ⚠️ **Para registrar uma venda é obrigatório cadastrar ao menos um vendedor antes.** O código do vendedor (cupom) é vinculado à venda.

### Cadastrando um Vendedor
1. Pressione `Alt + M` para abrir o Menu Administrativo
2. Selecione a opção **7 - Vendedores**
3. Clique em **Cadastrar Novo**
4. Preencha o nome e o código (cupom) do vendedor
5. Clique em **Salvar Registro**

---

## 🏧 Menu Administrativo (Alt + M)

| Tecla | Função |
|---|---|
| `1` | 💸 Sangria — retirada de dinheiro do caixa |
| `2` | 📥 Suprimento — entrada de dinheiro no caixa |
| `3` | 🏧 Status do Caixa |
| `4` | 🔒 Fechamento do Caixa |
| `5` | 📊 Relatório do Caixa |
| `6` | 🖨️ Reimprimir última venda |
| `7` | 👥 Gerenciar Vendedores |

---

## ⌨️ Atalhos do Sistema

| Atalho | Função |
|---|---|
| `Alt + M` | Abre o Menu Administrativo |
| `Alt + C` | Navega para o Caixa |
| `Alt + H` | Navega para o Histórico de Vendas |
| `Alt + E` | Navega para o Controle de Estoque |
| `ESC` | Abre/fecha o painel de ajuda com todos os atalhos |

---

## 📋 Histórico de Vendas

- Listagem de todas as vendas realizadas
- Exibe data, total, método de pagamento e vendedor
- Reimpressão de cupom de qualquer venda anterior

---

## 🏗️ Arquitetura

Padrão MVC com separação em `Controllers`, `Models`, `Views` e `Data` (DbContext). Injeção de dependência nativa do ASP.NET Core.

---

> Desenvolvido com C# e .NET 10 🔷

ControleEstoqueLoja Projeto simples de controle de estoque e PDV (caixa) para lojas físicas, construído com ASP.NET Core e Razor Views.

📌 Objetivo Fornecer uma solução leve para gerir produtos, realizar vendas no caixa, controlar suprimentos/sangrias e gerar cupons/relatórios diários de forma prática e local.

🚀 Funcionalidades
•	Gestão básica de produtos (nome, preço, estoque, código de barras).
•	Tela de Caixa com busca por produto (código/ID), entrada de itens e finalização de venda.
•	Registro de vendas com itens, método de pagamento, valor recebido e troco.
•	Impressão de cupom (/Caixa/GerarCupom?id={id}) e relatório diário de vendas.
•	Movimentações de caixa: Suprimento e Sangria.
•	Relatórios e resumo de pagamentos/dinheiro para fechamento do caixa.
•	Endpoints JSON para integração com o front-end (ex.: BuscarPorCodigo(string), ObterResumo(), FinalizarVenda(string, string, string, decimal, decimal, List<ItemVendaSimples>)).

💡 Possível Melhoria Futura (IA) Adicionar assistente IA para:
•	Gerar descrições de produtos ou textos do cupom mais profissionais.
•	Sugerir categorias/preços com base em referências e histórico.

Objetivo: padronizar comunicações e facilitar cadastro por usuários não técnicos.

🛠️ Tecnologias Utilizadas
•	.NET 10 (ASP.NET Core)
•	Razor Views / Controllers (CaixaController.cs, Views/Caixa/*)
•	Entity Framework Core (SQLite por padrão)
•	HTML, CSS, JavaScript (front-end do caixa)

📁 Arquivos importantes
•	CaixaController.cs — lógica do caixa e endpoints.
•	Index.cshtml — tela principal do caixa.
•	GerarCupom.cshtml — template do cupom.
•	ApplicationDbContext / migrações EF — modelo de dados.

📄 Licença Projeto de código aberto para fins educacionais.

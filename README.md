## Sistema de Controle de Estoque

Este repositório contém um projeto simples de **Controle de Estoque de Produtos**, desenvolvido em **C# (Windows Forms)** e utilizando **PostgreSQL** como banco de dados.

## Funcionalidades

- Cadastrar novos produtos
- Adicionar quantidade de produtos no estoque
- Remover quantidade de produtos no estoque
- Listar todos os produtos em um DataGridView

## Estrutura da Tabela no PostgreSQL

```sql
CREATE TABLE produto (
  id_produto SERIAL PRIMARY KEY,
  nome VARCHAR(45) NOT NULL,
  preco DECIMAL(10,2) NOT NULL,
  quantidade INT DEFAULT 0
);
```

##  Arquivo Principal

Todo o código do sistema está consolidado em um único arquivo:

- `ConsolidadoControleEstoque.cs`

Este arquivo contém:
- `Program.cs` (ponto de entrada)
- `Form1.cs` (eventos e lógica)
- `Form1.Designer.cs` (interface da aplicação)

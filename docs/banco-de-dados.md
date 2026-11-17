erDiagram
    PRODUTOS ||--o{ MOVIMENTACOES : "possui"

    PRODUTOS {
        int ID PK
        varchar Nome
        varchar Categoria
        int Quantidade
        int Estoque_Minimo
        decimal Preco
        datetime Data_Cadastro
    }

    MOVIMENTACOES {
        int ID PK
        int Produto_ID FK
        varchar Tipo "Entrada ou Saída"
        int Quantidade
        datetime Data
    }

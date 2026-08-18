# Modelo Dimensional

## Tabela de origem

`Financials_origem`

Cópia de segurança da tabela original Financial Sample. No modelo final do Power BI, a consulta pode permanecer oculta.

## Dimensões

### D_Produtos

- ID_Produto
- Produto
- Média de Unidades Vendidas
- Média do valor de vendas
- Mediana do valor de vendas
- Valor máximo de Venda
- Valor mínimo de Venda

### D_Produtos_Detalhes

- ID_Produto
- Discount Band
- Sale Price
- Units Sold
- Manufacturing Price

### D_Descontos

- ID_Produto
- Discount
- Discount Band

### D_Detalhes

Dimensão complementar para atributos que não foram contemplados nas demais dimensões.

### D_Calendário

- Data_ID
- Date
- Ano
- Mês
- Nome_Mês
- Trimestre
- Semestre

## Fato

### F_Vendas

- SK_ID
- ID_Produto
- Produto
- Units Sold
- Sales Price
- Discount Band
- Segment
- Country
- Salers
- Profit
- Date

## Princípio do modelo

A `F_Vendas` permanece no centro e as dimensões fornecem o contexto para análise. As chaves e relacionamentos finais devem ser validados após a implementação no Power BI Desktop.

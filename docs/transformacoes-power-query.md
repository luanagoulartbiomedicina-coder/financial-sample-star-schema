# Transformações no Power Query

1. Manter a tabela original como `Financials_origem`.
2. Criar cópias da consulta original para as dimensões e para a fato.
3. Remover das cópias as colunas que não pertencem à finalidade de cada tabela.
4. Criar `D_Produtos` usando Agrupar Por.
5. Calcular média de Units Sold.
6. Calcular média, mediana, máximo e mínimo de Sale Price.
7. Calcular média de Manufacturing Price.
8. Criar `D_Produtos_Detalhes`.
9. Criar `D_Descontos`.
10. Criar `D_Detalhes` com os atributos restantes relevantes.
11. Criar a identificação/índice de produto quando necessário.
12. Criar `F_Vendas`.
13. Reorganizar as colunas.
14. Criar `D_Calendário` com DAX.
15. No modelo, estabelecer os relacionamentos entre dimensões e fato.
16. Validar tipos de dados, chaves, duplicidades e granularidade antes da publicação.

## Coluna condicional

Exemplo documentado no material do desafio:

- Carretera → 0
- Montana → 1
- Paseo → 2
- Velo → 3
- VTT → 4
- Amarilla → 5

A regra deve ser aplicada apenas quando essa codificação for necessária para a identificação do produto.

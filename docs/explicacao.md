# Detalhamento da Lógica DAX – Catálogo Power BI

Este arquivo explica a estrutura por trás da medida "Catálogo de Dados" que utiliza funções INFO.VIEW no DAX Studio.

## Visão Geral

O script cria quatro blocos principais:
1. `colunas` – extrai colunas visíveis, chaves e suas descrições
2. `medidas` – lista todas as medidas com tipo e expressão
3. `tabelas` – identifica se a tabela é calculada ou de dados, e o modo de armazenamento
4. `relacionamentos` – identifica relacionamentos ativos/inativos, cardinalidade e direção de filtro

## Principais Expressões

```dax
INFO.VIEW.COLUMNS()
INFO.VIEW.MEASURES()
INFO.VIEW.TABLES()
INFO.VIEW.RELATIONSHIPS()
```

As expressões são combinadas com `SELECTCOLUMNS` e `UNION` para gerar uma única tabela final com a coluna "Categoria" identificando o tipo de objeto (Tabela, Coluna, Medida, Relacionamento).

## Campos Importantes

- `Nome`: Nome do objeto no modelo
- `Descrição`: Vem do próprio modelo + complemento (ex: "Coluna chave de relacionamento.")
- `Tipo`: Tipo de dado e categoria
- `Origem`: Nome da tabela ou origem do relacionamento
- `Expressão`: Para medidas, colunas calculadas ou tabelas DAX
- `Lineage Tag`: Referência interna usada pelo Power BI

## Benefícios

- Geração automatizada e padronizada
- Pronto para exportar e documentar modelos complexos
- Ideal para repositórios, auditorias ou entrega de projetos

## Sugestão de Uso

- Criar um visual do tipo tabela no Power BI com esse catálogo
- Adicionar filtros por Categoria ou Tabela para navegação
- Integrar com botões de ajuda em dashboards
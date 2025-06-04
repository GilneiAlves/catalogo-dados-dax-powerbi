# Catálogo de Dados com DAX no Power BI

Este projeto tem como objetivo gerar automaticamente um **catálogo técnico** dos objetos de um modelo de dados no Power BI utilizando expressões DAX. O catálogo inclui tabelas, colunas, medidas e relacionamentos, com descrições, expressões, tipos e outras informações úteis para documentação e governança de dados.

---

## Motivação

Durante o desenvolvimento de relatórios complexos no Power BI, é comum perder visibilidade sobre a estrutura interna do modelo — especialmente em times com múltiplos analistas. Este catálogo automatizado facilita:

- A documentação técnica do modelo
- O entendimento dos relacionamentos e da lógica do negócio
- A comunicação entre desenvolvedores e usuários
- A rastreabilidade de campos e medidas

---

## Funcionalidades

-  Lista de **tabelas visíveis**, incluindo se são calculadas ou importadas
-  Catálogo de **colunas**, indicando chaves, descrições e tipos
-  Visão de **medidas DAX** com suas expressões
-  Resumo dos **relacionamentos**, com cardinalidade e comportamento de filtro
-  Organização por categoria: Tabela, Coluna, Medida ou Relacionamento

---

##  Como usar

### 1. Abra o Power BI Desktop  
### 2. Crie uma nova medida e cole o script DAX disponível em [`src/catalogo_dados_dax.dax`](src/catalogo_dados_dax.dax)



## Contribuições
Contribuições são muito bem-vindas! Se tiver sugestões de melhorias ou quiser adaptar para outros idiomas ou formatos, sinta-se à vontade para contribuir.

##Contato
Para dúvidas, sugestões ou colaborações, entre em contato:
- Gilnei Alves de Freitas – Analista de Dados Sr.
- [gilnei147@gmail.com](gilnei147@gmail.com)
- [https://www.linkedin.com/in/gilnei-freitas/](https://www.linkedin.com/in/gilnei-freitas/)
# Catálogo de Modelo Power BI

Este repositório apresenta uma solução automatizada para gerar um catálogo de dados de um modelo Power BI diretamente do ambiente DAX Studio, utilizando funções INFO.VIEW.

## Objetivo

Facilitar a documentação de modelos Power BI, trazendo informações essenciais sobre tabelas, colunas, medidas e relacionamentos de forma estruturada.

## Estrutura

- `README.md` – Visão geral do projeto
- `explicacao.md` – Detalhamento da lógica DAX utilizada
- `modelo_exemplo.pbix` – (Opcional) Arquivo PBIX de exemplo
- `/backgrounds/` – Arquivos visuais de fundo usados no projeto

## Como usar

1. Abra seu modelo no DAX Studio.
2. Copie e execute o script DAX disponível em: [`src/catalogo_dados_dax.dax`](src/catalogo_dados_dax.dax).
3. Exporte o resultado para Excel ou insira diretamente em uma nova aba no Power BI.
4. Visualize e filtre os objetos com facilidade.

## Lógica DAX usada

A lógica está detalhada no arquivo `explicacao.md`, e permite explorar:
- Tabelas visíveis
- Medidas criadas
- Colunas com descrição e tipo
- Relacionamentos (com status ativo/inativo)

## Observações

- Evite executar esse script em modelos grandes sem filtro, pois pode ser pesado.
- Campos ocultos são automaticamente ignorados para foco nos objetos relevantes.

## Contato
Sugestões ou melhorias? Fique à vontade para abrir uma issue ou contribuir com um pull request.
- Gilnei Alves de Freitas – Analista de Dados Sr.
- [gilnei147@gmail.com](gilnei147@gmail.com)
- [https://www.linkedin.com/in/gilnei-freitas/](https://www.linkedin.com/in/gilnei-freitas/)

---
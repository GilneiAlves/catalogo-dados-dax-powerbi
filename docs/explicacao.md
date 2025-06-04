#  Explicação da Lógica do Catálogo de Dados

Este documento descreve a lógica por trás da criação do catálogo técnico de objetos DAX no Power BI, explicando passo a passo como as tabelas, colunas, medidas e relacionamentos são capturados, organizados e apresentados.

---

##  Objetivo

A ideia central é usar funções da biblioteca `INFO.VIEW` (disponível em ambientes com uso de tabular editor ou ferramentas de análise de metadados no Power BI) para extrair metadados do modelo. Em seguida, esses metadados são tratados com DAX para montar uma tabela unificada contendo todos os objetos importantes do modelo de dados.

---

##  Componentes do Catálogo

### 1. 🔢 Colunas

```dax
INFO.VIEW.COLUMNS()

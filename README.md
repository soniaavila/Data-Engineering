# Data Engineering - E-commerce

## Trabalho de Engenharia de Dados

Projeto desenvolvido para a disciplina de Engenharia de Dados da UniFECAF.

O objetivo deste trabalho é propor uma arquitetura moderna de dados para um ambiente de e-commerce, contemplando desde a camada transacional (OLTP) até a camada analítica (OLAP), utilizando conceitos de Data Lake, Data Warehouse, ETL/ELT, DataOps, governança e segurança dos dados.

---

## Objetivo

Empresas de e-commerce geram grandes volumes de dados provenientes de vendas, clientes, produtos e sistemas externos. Muitas vezes essas informações encontram-se distribuídas em diferentes fontes, dificultando a geração de análises e relatórios gerenciais.

Como solução, foi proposta uma arquitetura de dados capaz de integrar, armazenar, transformar e disponibilizar informações para análise e apoio à tomada de decisão.

---

## Tecnologias Propostas

### Banco de Dados Transacional (OLTP)

* MySQL
* MySQL Workbench

### Ingestão de Dados

* Airbyte

### Data Lake

* Amazon S3

### Processamento e Transformação (ETL/ELT)

* AWS Glue

### Data Warehouse

* Snowflake

### Visualização e Business Intelligence

* Power BI

### Governança e Segurança

* IAM
* Criptografia de dados
* Controle de acesso baseado em perfis
* Adequação à LGPD

---

## Arquitetura da Solução

Fluxo proposto:

MySQL (OLTP)
↓
Airbyte
↓
Amazon S3 (Data Lake)
↓
AWS Glue (ETL/ELT)
↓
Snowflake (Data Warehouse)
↓
Power BI (Dashboards e Relatórios)

---

## Estrutura do Repositório

```text
database/
 └── schema.sql

diagramas/
 ├── Diagrama_EER.png
 ├── arquitetura_oltp_olap.png
 └── agendamento_automacao.png

dashboard/
 └── dashboard.html

README.md
```

---

## Modelagem Relacional

Foi desenvolvido um banco de dados relacional utilizando MySQL Workbench contendo as entidades:

* Cliente
* Produto
* Pedido
* Item_Pedido

As tabelas foram relacionadas por meio de chaves primárias e estrangeiras, simulando as operações de um ambiente de e-commerce.

---

## DataOps e Monitoramento

A proposta contempla monitoramento das cargas de dados, validação de qualidade das informações, rastreabilidade dos processos e automação das execuções para garantir confiabilidade e disponibilidade dos dados.

---

## Segurança e Governança

A arquitetura proposta considera:

* Controle de acesso aos dados
* Criptografia em armazenamento e transmissão
* Proteção contra acessos não autorizados
* Conformidade com a LGPD
* Monitoramento e auditoria dos processos

---

## Dashboard Analítico

Como demonstração da camada analítica, foi desenvolvido um dashboard contendo indicadores de negócio, faturamento, clientes, produtos vendidos e gráficos analíticos para apoio à tomada de decisão.

---

## Como Executar o Banco de Dados

```sql
mysql -u usuario -p banco_relacional < database/schema.sql
```

---

## Autor

Sonia Avila

Trabalho desenvolvido para a disciplina de Engenharia de Dados - UniFECAF.

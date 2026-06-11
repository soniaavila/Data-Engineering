# Data-Engineering
Trabalho de Data Engineering

# Engenharia de Dados - E-commerce

Este repositório contém o trabalho desenvolvido para a disciplina de **Data Engineering** na UniFECAF.  
O objetivo é propor uma **arquitetura moderna de dados em nuvem** para integrar informações fragmentadas de um e-commerce, garantindo **qualidade, segurança, governança e escalabilidade**.

---

##  Estrutura do Repositório
- `database/schema.sql` → Script SQL para criação das tabelas (Cliente, Produto, Pedido, Item_Pedido) e inserção de dados de exemplo.
- `diagramas/Diagrama_EER.png` → Modelo entidade-relacionamento (OLTP).
- `diagramas/arquitetura.png` → Arquitetura OLAP + Pipeline ETL/ELT.
- `README.md` → Documento explicativo do projeto.

---

##  Banco de Dados
Para recriar o banco de dados localmente:

```bash
mysql -u usuario -p banco_relacional < database/schema.sql

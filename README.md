# **Geração de Relatórios e Análise de Dados de Vendas**

## **Visão Geral**
Este projeto tem como objetivo demonstrar a análise e geração de relatórios de vendas a partir de um banco de dados simulado. Utilizando **MySQL** e a linguagem **SQL**, este projeto é focado em aprender e aplicar junções de tabelas, funções de agregação e filtragem para responder a perguntas estratégicas sobre vendas, clientes, fornecedores e funcionários de uma empresa fictícia.

Este repositório contém as consultas SQL que resolvem 15 questões de negócios essenciais, divididas em três níveis de complexidade.

## **Objetivo**
O objetivo principal do projeto é permitir que os alunos desenvolvam habilidades práticas no uso de SQL, focando em:
- Realizar junções de tabelas para combinar dados de múltiplas fontes.
- Aplicar funções de agregação (como **COUNT()**, **SUM()**, **AVG()**) para gerar métricas de negócios.
- Gerar relatórios detalhados sobre as operações de vendas, desempenho de funcionários e análise de fornecedores.

## **Estrutura do Banco de Dados**
O banco de dados simula as operações de vendas de uma empresa fictícia e contém as seguintes tabelas principais:

| Tabela       | Descrição                                        | Colunas Chave para Relações                  |
|--------------|--------------------------------------------------|----------------------------------------------|
| **Customers** | Detalhes dos clientes (Nome, País, Cidade)      | CustomerID                                  |
| **Employees** | Informações sobre os funcionários de vendas     | EmployeeID                                  |
| **Orders**    | Detalhes dos pedidos (Data, Cliente, Vendedor)  | OrderID, CustomerID, EmployeeID, ShipperID  |
| **Products**  | Produtos vendidos (Nome, Preço, Fornecedor)     | ProductID, SupplierID, CategoryID           |
| **OrderDetails**| Detalhes sobre cada item de um pedido (Quantidade) | OrderID, ProductID                        |
| **Categories**| Classificação dos produtos (Ex: Bebidas)        | CategoryID                                  |
| **Suppliers** | Fornecedores de produtos                        | SupplierID                                  |
| **Shippers**  | Transportadoras que realizam os envios          | ShipperID                                   |

## **Consultas Resolvidas**
O projeto responde a 15 questões de negócios importantes, distribuídas por três níveis de complexidade:

### **Nível Básico**
1. **Clientes na Alemanha**: Liste os nomes dos clientes e os contatos localizados no país 'Germany'.
2. **Produtos da Categoria 'Beverages'**: Liste os produtos e preços da categoria 'Beverages', ordenando por preço.
3. **Detalhes do Funcionário**: Mostre o nome, sobrenome, data de nascimento e as notas de um funcionário específico.

### **Nível Intermediário**
4. **Contagem de Clientes por País**: Mostre a contagem de clientes por país, ordenando em ordem decrescente.
5. **Fornecedores de 'Seafood'**: Liste os fornecedores que fornecem produtos classificados como 'Seafood'.
6. **Produto Mais Caro e Mais Barato**: Encontre o produto mais caro e o mais barato.
7. **Pedidos por Transportadora**: Calcule o número total de pedidos processados por cada transportadora.
8. **Média de Produtos Vendidos por Pedido**: Calcule a quantidade média de produtos vendidos por pedido.
9. **Pedidos por Funcionário**: Liste o nome completo do funcionário e o número total de pedidos que ele processou.
10. **Pedidos em Julho de 1996**: Conte quantos pedidos foram realizados em julho de 1996.

### **Nível Avançado**
11. **Clientes com Mais de 3 Pedidos em Dezembro de 1997**: Liste os nomes dos clientes que fizeram mais de 3 pedidos nesse mês.
12. **Produtos com Baixas Vendas**: Liste os produtos cuja quantidade total vendida é inferior a 50.
13. **Fornecedores no Japão e Categoria 'Seafood'**: Liste os fornecedores localizados no Japão que fornecem produtos na categoria 'Seafood'.
14. **Cálculo da Receita de um Pedido**: Calcule o valor total da receita de um pedido específico (ex: OrderID 10248).
15. **Funcionários Fluentes em Francês em Londres**: Liste os funcionários que falam francês e trabalharam em pedidos feitos por clientes de Londres.

## **Tecnologias Utilizadas**
- **MySQL**: Sistema de gerenciamento de banco de dados relacional utilizado para armazenar e manipular os dados de vendas.
- **SQL**: Linguagem de consulta estruturada utilizada para escrever as consultas que respondem às perguntas de negócios.

## **Como Executar as Consultas**
1. **Pré-requisitos**: Instale o MySQL em sua máquina ou use um serviço de banco de dados MySQL online.
2. **Banco de Dados**: Crie o banco de dados utilizando o script fornecido no repositório (se aplicável).
3. **Consultas SQL**: Execute as consultas SQL fornecidas nos arquivos `.sql` no seu ambiente MySQL.

### Exemplo de Execução de Consulta:

```sql
SELECT CustomerName, ContactName
FROM Customers
WHERE Country = 'Germany';
README.md
Exibindo README.md…
Programação em Banco de Dados
PROGBD 2503NG
Próximas atividades
Nenhuma atividade para a próxima semana!

Escreva um aviso para sua turma
Atividade
Leandro Soares postou uma nova atividade: Importar dados para o banco
Item postado: 20:56
Atribuído

Employees.csv
CSV

OrderDetails.csv
CSV

Orders.csv
CSV

Shippers.csv
CSV

Suppliers.csv
CSV

Customers.csv
CSV

products.csv
CSV

Categories.csv
CSV

MySQL Database.xlsx
Microsoft Excel

Atividade Prática de SQL: Geração de Relatórios e Análise de Dados de Vendas
Documentos Google

README.md
Texto

Adicionar comentário para a turma...

Material
Leandro Soares posto

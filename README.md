#Projeto Módulo de BD - E-commerce (PostgreSQL)

O projeto tem como proposta desenvolver uma modelagem física de um ecommerce, bem como todos os comandos SQL de DDL e DML da modelagem produzida. Este é o desafio desenvolvido durante o módulo de Banco de Dados do curso da Ada no programa Americanas Polo Tech | Trilha de Back-End com Java.

Grupo:
* Bruno de Oliveira
* Ivana Maria Feitosa Silva
* Rachel Lizandra Borborema

## Parte 1 | Modelagem, DDL, DML

* Modelagem
Modelo físico completo referente ao projeto conceitual do ecommerce visto em aula. Entregar o link do github com os arquivos do print do modelo físico completo e o arquivo (.dbs) do DBSchema.

<div style="display: inline_block"><br>
  <img align="center" src="https://github.com/viniciusCornieri/ada-turma-926-bd-po-001/blob/main/modelo_conceitual.png?raw=true" />
<div>

* DDL - Data Definition Language
Para o modelo físico entregue no tópico anterior, entreguem o SQL com todo o DDL necessário para criar esse banco de dados no postgreSql. O SQL pode estar em um arquivo chamado `ecommerce-ddl.sql` no github.

* DML - Data Manipulation Language
Com o banco de dados e tabelas criadas agora é hora de popularmos nosso e-commerce com dados, crie o SQL com a inserção dos seguintes dados: <br>

5 clientes<br>
5 produtos<br>
2 clientes devem ter pelo menos 3 produtos no carrinho<br>
6 pedidos com pelo menos 2 produtos cada um<br>
3 campanhas de cupons<br>
    2 pedidos que utilizaram cupons<br>
2 fornecedores<br>
    Associe os produtos com esses dois fornecedores<br>
2 estoques<br>
    Adicione os produtos cadastrados nos estoque<br>

Entregar também a remoção de 1 cliente que não possua pedidos ou items no carrinho e a atualização da descrição e valor de um produto. 

A entrega pode ser feita no github e estar em um arquivo chamado `ecommerce-dml.sql.`

## Parte 2 | Consultas & Querys
Utilizando o banco de dados da primeira parte do projeto, ou o disponibilizado em sala de aula. Crie consultas SQL para os seguintes problemas:
<ol>
<li>Listar todos os cliente que tem o nome 'ANA'.> Dica: Buscar sobre função Like;</li>
<li>Pedidos feitos em 2023;</li>
<li>Pedidos feitos em Janeiro de qualquer ano;</li>
<li>Itens de pedido com valor entre R$2 e R$5;</li>
<li>Trazer o Item mais caro comprado em um pedido;</li>
<li>Listar todos os status diferentes de pedidos;</li>
<li>Listar o maior, menor e valor médio dos produtos disponíveis;</li>
<li>Listar fornecedores com os dados: nome, cnpj, logradouro, numero, cidade e uf de todos os fornecedores;</li>
<li>Informações de produtos em estoque com os dados: id do estoque, descrição do produto, quantidade do produto no estoque, logradouro, numero, cidade e uf do estoque;</li>
<li>Informações sumarizadas de estoque de produtos com os dados: descrição do produto, código de barras, quantidade total do produto em todos os estoques;</li>
<li>Informações do carrinho de um cliente específico (cliente com cpf '26382080861') com os dados: descrição do produto, quantidade no carrinho, valor do produto;</li>
<li>Relatório de quantos produtos diferentes cada cliente tem no carrinho ordenado pelo cliente que tem mais produtos no carrinho para o que tem menos, com os dados: id do cliente, nome, cpf e quantidade de produtos diferentes no carrinho;</li>
<li>Relatório com os produtos que estão em um carrinho a mais de 10 meses, ordenados pelo inserido a mais tempo, com os dados: id do produto, descrição do produto, data de inserção no carrinho, id do cliente e nome do cliente;</li>
<li>Relatório de clientes por estado, com os dados: uf (unidade federativa) e quantidade de clientes no estado;</li>
<li>Listar cidade com mais clientes e a quantidade de clientes na cidade;</li>
<li>Exibir informações de um pedido específico, pedido com id 952, com os dados (não tem problema repetir dados em mais de uma linha): nome do cliente, id do pedido, previsão de entrega, status do pedido, descrição dos produtos comprados, quantidade comprada produto, valor total pago no produto;</li>
<li>Relatório de clientes que realizaram algum pedido em 2022, com os dados: id_cliente, nome_cliente, data da última compra de 2022;</li>
<li>Relatório com os TOP 10 clientes que mais gastaram esse ano, com os dados: nome do cliente, valor total gasto;</li>
<li>Relatório com os TOP 10 produtos vendidos esse ano, com os dados: descrição do produto, quantidade vendida, valor total das vendas desse produto;</li>
<li>Exibir o ticket médio do nosso e-commerce, ou seja, a média dos valores totais gasto em pedidos com sucesso;</li>
<li>Relatório dos clientes gastaram acima de R$ 10000 em um pedido, com os dados: id_cliente, nome do cliente, valor máximo gasto em um pedido;</li>
<li>Listar TOP 10 cupons mais utilizados e o total descontado por eles;</li>
<li>Listar cupons que foram utilizados mais que seu limite;</li>
<li>Listar todos os ids dos pedidos que foram feitos por pessoas que moram em São Paulo (unidade federativa, uf, SP) e compraram o produto com código de barras '97692630963921';</li>
<li>Faça um relatório de sua escolha, crie uma view para ele e faça uma consulta nessa view;</li>
</ol>

Entregar no github em um arquivo chamado `ecommerce-consultas.sql` as consultas para os problemas anteriores.

## Linguagens e Ferramentas Utilizadas

* PostgreSQL
* Docker
* VSCode
* Dbeaver
* DbSchema


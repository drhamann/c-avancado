# Aula sobre n-layers

## Apresentado conceito, e criado projeto exemplo de camadas usando o contexto de uma pizzaria

- .net 8
- Sqlite

## Aula 3 

Vamos continuar com nossa pizzaria. Agora vamos adicionar novas funcionalidades:
1. Adicionar cliente.
2. Adicionar pizza.
3. Adicionar pedido.
4. Obter todos os clientes.
5. Obter todas as pizzas.
6. Obter todos os pedidos.

Camada de Apresenta��o
1. Adicionar pizzas.
2. Adicionar clientes.
3. Fazer pedidos, associando clientes e pizzas.
4. Exibir informa��es sobre clientes, pizzas e pedidos.

Camada regra de neg�cio	

Entidades 
	1. `Pizza`:	   - Propriedades: `Id`, `Nome`, `Descricao`, `Preco`.
	2. `Cliente`:  - Propriedades: `Id`, `Nome`.
	3. `Pedido`:  - Propriedades: `Id`, `ClienteId`, `PizzasIds` (lista de IDs de pizzas associadas).

Servi�os
	1. `PedidoService`:
	   - Fazer pedidos associando clientes e pizzas.
	   - Adicionar clientes.
	   - Adicionar pizzas.
	   - Obter todos os clientes.
	   - Obter todas as pizzas.
	   - Exibir informa��es sobre clientes, pizzas e pedidos.

Camada Acesso a Dados (DAO)

1. 1. Tabela `Clientes`:   
	1. - Colunas: `Id` (chave prim�ria), `Nome`.
2. Tabela `Pizzas`: 
	1. - Colunas: `Id` (chave prim�ria), `Nome`, `Descricao`, `Preco`.
3. Tabela `Pedidos`:   
	1.	- Colunas: `Id` (chave prim�ria), `ClienteId`, `PizzasIds` (lista de IDs de pizzas associadas).

## Aula 4 e 5 

1. Adicionar cliente.
1.1 O cliente deve ter hist�rico de a��es
2. Adicionar pizza.
2.1 Pizza deve ter dado de cria��o
3. Adicionar pedido.
3.1 O pedido deve ter hor�rio de solicita��o
3.2 O pedido deve ter hor�rio de finaliza��o da prepara��o
3.3 O pedido deve ter hor�rio de sa�da para entrega
3.3 O pedido deve ter hor�rio de finaliza��o da entrega
4. Obter todos os clientes.
5. Obter todas as pizzas.
6. Obter todos os pedidos.
7. Gerar relat�rio em arquivo texto dos pedidos finalizados mostrando os dados de quem pediu, a pizza, hor�rio que o pedido come�ou e hor�rio de finaliza��o da prepara��o, hor�rio que saiu e finalizou a entrega. 
7.1 Deve permitir gerar o relat�rio escolhendo a data inicial e final 
7.2 Deve ter uma op��o de escolher entre arquivo texto e json

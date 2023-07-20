# calculo_pedido

Programa que faz anotações e calcula os pedidos listados.

Diagrama UML
![calculo_pedido](https://github.com/LuizWolff/calculo_pedido/assets/46894743/28634c26-9b13-422b-a3fb-7488b440fb88)

No diagrama UML o Diamante preto chama Associação de composição, no contexto de composição de objeto em sistema, chamamos de composição de uma forma geral, todo tipo de associação que você tenha essa ideia que um objeto tem um ou tem vários do outro. 
O pedido tem um cliente associado a ele, embora a relação entre pedido e cliente não seja de todo parte, o cliente não é parte de um pedido, a gente diz que o pedido tem uma referência para o cliente. Essa ideia de “tem”, ela se aplica na UML, mesmo não sendo o diamante preto que é o símbolo especifico de composição.

Da mesma forma que o item de pedido tem um produto, ele tem uma referência para um produto.

Uma observação, no diagrama não foi preenchido o ID, o código de cada entidade, porque isso é só um exemplo para implementar mais rápido em memória. Quando for implementar essa versão no banco de dados, então vai ser preenchido o ID em todas entidades.
OrderItem é repetido o price: Double para manter um histórico do preço que foi vendido nessa época, se amanhã o preço do produto aumentar, muda o preço do produto mas mantém o histórico do item de pedido “OrderItem”.

=======================================================================

Execução do programa:

O programa vai iniciar com os dados do cliente “Enter cliente data:” em seguida preencher com Name, Email e Birth date, lembrando que esses dados estão no diagrama na classe “Client”. 
Name:
Email:
Birth date (DD/MM/YYYY):

Depois vai ter que entrar com os dados do pedido “STATUS:” é preciso escrever do jeito que está no enumerado que são: 
Enter order data:
Status:

PEDING_PAYMENT (PAGAMENTO PENDENTE)

PROCESSING (EM PROCESSAMENTO)

SHIPPED (ENVIADO)

DELIVERED (ENTREGUE)


Em seguida o programa vai perguntar: How many items to this order (Quantos itens vai ter neste pedido?) 
Logo em seguida o programa vai perguntar o nome do produto, preço do produto e quantidade.

Product name: 

Product Price 

Quantity: 

Depois de preenchido todos os dados, o programa vai mostrar um relatório do pedido calculando todos os dados preenchido.
Order Moment: (momento do pedido DD/MM/YYYY + Horário)

Order status: 

Cliente (Nome, data de nascimento, email)

Order items: (Uma lista com os items preenchido).

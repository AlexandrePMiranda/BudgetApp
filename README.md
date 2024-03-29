# BudgetApp

Ela deve ser capaz de instanciar objetos com base em diferentes categorias de orçamento, como alimentos (food), vestuário (clothing) e entretenimento (entertainment). Quando os objetos são criados, eles são passados com o nome da categoria. A classe deve ter uma variável de instância chamada ledger que seja uma lista. A classe também deve conter os seguintes métodos:

Um métododeposit, que aceita um valor e uma descrição. Se nenhuma descrição for dada, o padrão deverá ser uma string vazia. O método deve acrescentar um objeto à lista ledger na forma de {"amount": amount, "description": description}.
Um método withdraw, semelhante ao método deposit, mas a quantia passada deve ser armazenada no ledger como um número negativo. Se não houver fundos suficientes, nada deve ser adicionado ao ledger. Este método deve retornar True se a retirada acontecer e, caso contrário, False.
Um método get_balance, que retorna o saldo atual da categoria de orçamento com base nos depósitos e retiradas que ocorreram.
Um método transfer, que aceita um valor e outra categoria de orçamento como argumentos. O método deverá adicionar uma retirada com o valor e a descrição "Transfer to [categoria de destino no orçamento]". O método deve, então, adicionar um depósito à outra categoria do orçamento, com o valor e a descrição "Transfer from [categoria de origem no orçamento]". Se não houver fundos suficientes, nada deve ser adicionado ao ledger. Este método deve retornar True se a transferência acontecer e, caso contrário, False.
Um método check_funds que aceita um valor como um argumento. Ele retorna False se o valor for maior que o saldo da categoria do orçamento e, caso contrário, retorna True. Este método deve ser usado tanto pelo método withdraw como pelo método transfer.
Quando o objeto de orçamento for impresso, ele deve mostrar:

Uma linha com título de 30 caracteres em que o nome da categoria é centralizado em uma linha com * caracteres.
Uma lista dos itens no ledger. Cada linha deve mostrar a descrição e o valor. Os primeiros 23 caracteres da descrição devem ser exibidos e, depois, o valor. O valor deve estar alinhado corretamente, conter duas casas decimais e exibir um máximo de 7 caracteres.
Uma linha que exibe o total da categoria.
Aqui está um exemplo de resultado:


![image](https://github.com/AlexandrePMiranda/BudgetApp/assets/135765440/8bc5f7c0-2f28-4a82-bb1c-a9c331e36809)

Além da classe Category, crie uma função (fora da classe) chamada create_spend_chart, que recebe uma lista de categorias como um argumento. Ela deve retornar uma string, que é um gráfico de barras.

O gráfico deve mostrar a porcentagem gasta em cada categoria passada para a função. A porcentagem gasta deve ser calculada apenas com retiradas, não com depósitos. No lado esquerdo do gráfico, deve haver rótulos de 0 a 100. As "barras" no gráfico de barras devem ser feitas com o caractere "o". A altura de cada barra deve ser arredondada para baixo para o 10 mais próximo. A linha horizontal abaixo das barras deve ir dois espaços além da barra final. O nome de cada categoria deve ser escrito verticalmente abaixo da barra. Deve haver um título no topo que diz "Percentage spent by category" (Porcentagem gasta por categoria).

Esta função será testada com até quatro categorias.

Olhe atentamente para o exemplo de resultado abaixo e certifique-se de que o espaçamento do resultado corresponde exatamente ao exemplo.



![image](https://github.com/AlexandrePMiranda/BudgetApp/assets/135765440/74b55098-bc4a-4b85-91a8-d63068ce5479)


Para utilizar Budget app, é só copiar o código em um compilador python, e fzr um código de utilização do app de acordo com as instruções acima.

# Trabalho-1-POO-Java-AcmeRental
Trabalho 1 do segundo semestre da faculdade de Engenharia de Software. Matéria: Programação Orientada a Objetos - Java.

1. Enunciado geral:
A ACMERental é uma empresa que aluga itens para clientes e quer lançar aplicativos
independentes para cada tipo de item alugável.
Você será responsável pelo desenvolvimento de um destes aplicativos.
O analista de sistemas identificou as seguintes classes iniciais, com alguns atributos e
relacionamentos apresentados a seguir.
![image](https://user-images.githubusercontent.com/101745159/191379500-c0bb0311-fe1c-4445-a680-b337be2e0f50.png)
O analista identificou operações básicas iniciais das classes:
• Acervo: classe catálogo que gerencia o cadastro de itens alugáveis:o adicionaAlugavel(Alugavel): recebe como parâmetro um novo item alugável e
cadastra-o no sistema. Não pode haver itens alugáveis com o mesmo código.
Retorna true se o cadastro teve sucesso.
o pesquisaAlugavel(int): retorna o item alugável com o código indicado. Se não
houver item alugável com este código retorna null.
o pesquisaAlugavel(String): retorna uma lista de itens alugáveis com o nome
indicado. Se não houver nenhum item alugável com este nome retorna null.
• Locacoes: classe catálogo que gerencia o cadastro de aluguéis:
o adicionaAluguel(Aluguel): recebe como parâmetro um novo aluguel e
cadastra-o no sistema.
o pesquisaAluguel(String): retorna uma lista de aluguéis com o CPF indicado.
Se não houver nenhum aluguel com este CPF retorna null.
• Aluguel: classe que representa um aluguel por um cliente:
o calculaValorTotal(): calcula o valor total do aluguel pelo número de dias
indicado no atributo ‘periodo’ multiplicado pelo ‘precoDiario’ do item alugável. Se
o número de dias for maior que 7 (sete) há um desconto de 10%. Armazena o
valor calculado no atributo ‘valorFinal’ e retorna o valor calculado.
• ACMERental: classe do aplicativo:
o preCadastra(): pré-cadastra alguns itens alugáveis e alguns aluguéis no
sistema por meio de objetos da classe Acervo e objeto da classe Locacoes.
o executa(): executa o aplicativo por meio de objeto da classe Acervo e objeto da
classe Locacoes.
• Main: classe principal (inicial) do sistema:
o main(String[]): cria um objeto ACMERental, chama o método preCadastra()
deste objeto e depois chama o método executa().
O método executa() deve apresentar uma tela cíclica com o usuário com as opções de:
1. Mostrar todos os dados cadastrados: mostra na tela todas as informações de
todos os itens alugáveis cadastrados no sistema e todos os dados dos seus
respectivos aluguéis. Se não houver nenhum item alugável cadastrado, apresenta
a mensagem “Nenhum item alugavel cadastrado no sistema.”
2. Pesquisar item alugavel pelo codigo: solicita ao usuário um código de um item
alugável. Mostra na tela todos os dados do item alugável e todos os dados dos
respectivos aluguéis. Se não houver participante com o código indicado, apresenta
a mensagem “Nenhum item alugavel encontrado com este codigo.”
3. Pesquisar itens alugaveis pelo nome: solicita ao usuário um nome de item
alugável. Mostra na tela todos os dados de itens alugáveis com o nome indicado e
todos os dados dos respectivos aluguéis. Se não houver nenhum item alugável
com o nome indicado, apresenta a mensagem “Nenhum item alugavel encontrado
com este nome.”
4. Pesquisar alugueis de um cliente: solicita ao usuário um CPF de um cliente.
Mostra na tela todos os dados dos aluguéis do cliente e todos os dados dos
respectivos itens alugados. Se não houver aluguéis com o CPF indicado, apresenta
a mensagem “Nenhum aluguel encontrado com este CPF.”
5. Sair: finaliza a execução do aplicativo.
2. Definição do exercício:
O objetivo do exercício é implementar um sistema que capaz de atender as necessidades
da empresa descrita no enunciado geral, e que atenda as restrições que a seguir:
• Você deve escolher um dos tipos de item alugável para a implementação: “Calçado,
Carro, Ferramenta, Imóvel, Equipamento eletrônico, Equipamento esportivo,
Equipamento médico, Mobília ou Roupa” na área Moodle da disciplina, atividade “escolha
do tipo de item alugável”.• A classe “Alugavel” deve ter pelo menos mais 2 (dois) atributos novos relacionados ao
tipo do item alugável escolhido, com os respectivos métodos de consulta (get) e alteração
(set).
• A classe “Alugavel” deve ter pelo menos 2 (dois) construtores.
• O cadastramento de itens alugáveis e aluguéis ocorrerá diretamente no método
preCadastra() da classe ACMERental que deve ter a codificação da criação
(instanciação) e cadastramento correto de, pelo menos:
o 3 itens alugáveis diferentes.
o 5 aluguéis diferentes.
o 1 dos itens alugáveis deve possuir 3 aluguéis diferentes.
o 2 aluguéis devem ser do mesmo cliente, mas cada um com item alugável diferente.
o 1 dos aluguéis deve ter período de mais de 7 dias.
• Toda entrada e saída de dados com o usuário deve ocorrer apenas na classe
ACMERental.
• A classe “Alugavel” e a classe “Aluguel” devem ter testes unitários com 100% de
cobertura.
• É permitida a criação de novos métodos, atributos e relacionamentos, mas as
informações definidas no diagrama de classes original não podem ser alteradas.
• O diagrama de classes deve ser atualizado conforme as alterações realizadas e deve ser
entregue em arquivo Astah ou PDF.

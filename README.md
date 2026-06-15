O MeuAppCombustivel é um aplicativo desenvolvido em .NET MAUI com a finalidade de auxiliar o usuário na escolha do combustível mais vantajoso para abastecimento. A aplicação utiliza os preços informados de etanol e gasolina para realizar um cálculo simples e indicar qual opção apresenta melhor custo-benefício.

# Funcionamento

A aplicação possui uma interface simples composta por dois campos de entrada, nos quais o usuário informa os valores do etanol e da gasolina. Após preencher os dados, basta pressionar o botão "Calcular" para que o sistema processe as informações.

O evento de clique do botão é tratado no arquivo Code Behind (.xaml.cs) por meio do método responsável pela lógica da aplicação. Inicialmente, os valores digitados são recuperados dos campos da interface e convertidos para um formato numérico adequado para o cálculo.

Em seguida, o sistema compara o preço do etanol com 70% do valor da gasolina, seguindo a regra amplamente utilizada para determinar a melhor opção de abastecimento:

Se o preço do etanol for superior a 70% do preço da gasolina, a gasolina é considerada mais vantajosa.
Caso contrário, o etanol será a melhor escolha.

Após a conclusão do cálculo, o resultado é exibido ao usuário através do método nativo DisplayAlertAsync(), apresentando uma mensagem informativa com a recomendação do combustível mais econômico.

# Conceitos Aplicados

Durante o desenvolvimento deste projeto foram utilizados e praticados os seguintes conceitos:

Criação e configuração de projetos utilizando .NET MAUI;
Estruturação de aplicações multiplataforma;
Separação entre interface gráfica (XAML) e lógica de programação (Code Behind);
Utilização do atributo x:Name para identificação e manipulação de componentes visuais;
Tratamento de eventos de interação do usuário, como o evento Clicked;
Conversão e validação de dados informados pelo usuário;
Uso de métodos nativos para exibição de mensagens e alertas na interface.

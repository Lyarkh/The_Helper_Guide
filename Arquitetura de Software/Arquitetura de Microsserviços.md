#arquitetura #microsserviços
## Resumo
---
Microsserviços é o nome dado a uma arquitetura que estrutura a aplicação criando uma coleção de serviços.   

Quando se fala nesse tipo de arquitetura, basicamente nós pegamos um monolito que seria criado e o dividimos em vários serviços separados e independentes um do outro.   

A ideia é separar os serviços para que cada um acesse uma camada do banco de dados ou somente um acesse algum serviço externo.


## Exemplo para Microsserviços
---
Vou usar o exemplo citado para deixar o entendimento sobre Microsserviços um pouco mais claro, considerando a criação de uma aplicação para uma loja de calçados. 

Neste caso, a diferença é que cada parte da aplicação será um microsserviço.   

No exemplo abaixo, serão cinco:  
-   Autenticação e perfis de usuários (administração, contabilidade, estoque, vendedor);
-   Gráficos para a administração com os dados diários da loja;
-   Compra de produtos;
-   Estoque;
-   Vendas.

Agora, a ideia é imaginar que tudo é separado, um serviço será independente do outro.
Quando um _deploy_ para o servidor for feito para ser disponibilizado o serviço, serão necessários ser feitos 5 _deploys_ separados e que não tem relação nenhuma um com o outro.


## Vantagens dos Microsserviços
---
-   **Altamente testável e manutenível:** tudo é feito de forma separada e mais rápida;
-   **Independência e agilidade:** os _deploys_ de cada microsserviço são totalmente independentes e mais rápidos;
-   **Objetividade:** a organização é feita de acordo com a organização do produto e do negócio;
-   **Flexibilidade:** é possível dividir em equipes para trabalhar de forma separada e totalmente independente em cada serviço.


## Desvantagens dos Microsserviços
---
-   **Quando a arquitetura do sistema é feita, a divisão dos serviços tem que ser feita com muita atenção e cuidado:** isso pode fazer com que se leve um pouco mais de tempo para chegar na divisão perfeita, de forma que no futuro a aplicação não sejam vários sistemas monolíticos separados e com funções que até se repetem;
-   **Há replicação de código de resposta ou de infraestrutura, por exemplo:** o que existe de padrão em um serviço provavelmente existirá nos outros serviços também;
-   **Complexidade no gerenciamento da aplicação:** é um ponto a se tomar muito cuidado para que a organização sempre exista mesmo que novas _features_ sejam implementadas no futuro.
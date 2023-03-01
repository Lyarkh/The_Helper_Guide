
## Resumo
---
Microsserviços é o nome dado a uma arquitetura que estrutura a aplicação criando uma coleção de serviços.   

Quando se fala nesse tipo de arquitetura, basicamente nós pegamos um monolito que seria criado e o dividimos em vários serviços separados e independentes um do outro.   

A ideia é separar os serviços para que cada um acesse uma camada do banco de dados ou somente um acesse algum serviço externo.


## Exemplo para Microserviços
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
#arquitetura #monolitica
## O que é ?
---
A arquitetura monolítica é um sistema único, não dividido, que está feito sobre um único processo, uma única aplicação em que diversos componentes estão ligados à um único programa e plataforma. Em sua maioria até mesmo utilizando uma única linguagem de programação como base.


## Algumas das vantagens da Arquitetura monolítica
---
-   **Mais simples de desenvolver:** a organização fica concentrada em um único sistema;
-   **Simples de testar:** é possível testar a aplicação de ponta a ponta em um único lugar;
-   **Simples de fazer o _deploy_ para o servidor:** a alteração é simplesmente feita e pronto;
-   **Simples de escalar:** como é só uma aplicação, se for preciso adicionar mais itens, é simplesmente ir adicionando o que for necessário.


## Desvantagens da Arquitetura monolítica
---
- **Manutenção:** a aplicação se torna cada vez maior de acordo com o seu tamanho, o código será cada vez mais difícil de entender e o desafio de fazer alterações rápidas e ter que subir para o servidor só cresce;
- **Alterações:** para cada alteração feita, é necessário realizar um novo _deploy_ de toda a aplicação;
- **Linha de código**: uma linha de código que subiu errada pode quebrar todo o sistema e ele ficar totalmente inoperante;
- **Linguagens de programação:** não há flexibilidade em linguagens de programação. Aquela que for escolhida no início do projeto terá que ser seguida, sempre. Se o desenvolvimento de uma nova funcionalidade exigir outra linguagem de programação, existem duas possibilidades: ou todo o código é alterado ou a arquitetura do sistema precisará ser trocada.
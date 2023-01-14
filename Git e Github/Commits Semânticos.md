Commits semânticos são um convenção para manter a padrões de commits.
Utilizar padões de commits é uma ótima maneira de deixar um histórico de commits explícito, facilitando na hora de criação de ferramentas automatizadas. 

O commit semântico informa a intensão do seu commit na hora de utilizar em seu código.

### Títulos para os commits semânticos:

`feat` - os commits do tipo feat indicam que o trecho do código que está adicionando está incluindo um **novo recurso** (se relaciona ao MINOR do [[Versionamento semântico]]).

`fix` - os commits do tipo fix indicam que a parte do código commitado está **resoluções de algum problema** (se relaciona com o PATCH do [[Versionamento semântico]])

`test` -  os commits do tipo test são utilizados quando alguma **alteração em testes** ocorra, seja criando, alterando, modificando ou deletando testes. (Não inclui alterações em código)

`build` - os commits do tipo build são utilizados quando ocorrem modificações em **arquivos de build e depedências**

`docs` - os commits do tipo docs indicam que houve **modificações noa documentação**. Como a modificação do README do seu projeto.

`perf` - os commits do tipo perf servem para indicar qualquer alteração que for feita no código relacionado a **performance**.

`style` - os commits do tipo style indicam que houveram alterações referentes a **formatação de código**. (*exemplo*: linting, indentação, entre outros).

`ci` - os commits do tipo ci indicam mudanças relacionadas a **integração contínua**.

`chore` -os commits do tipo chore indicam  **atualizações de tarefas** de builds, configurações de administrador (*exemplo*: adicionar um pacote no gitignore). Não inclui alterações no código.
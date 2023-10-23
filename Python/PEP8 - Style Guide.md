`tags:` #python #pattern #design 


Documentação referente à [PEP8](https://peps.python.org/pep-0008/).

## Introdução
---
Este documento fala sobre as convensões de códigos criadas e utilizadas para códigos em Python. todos os padrões deste documento foram identificados de convensões passadas já utilizadas e feito a remodelação para seguir as mudanças que vieram surgir com a linguagem.


## Breve Resumo sobre PEP8
---
A PEP8 é uma das PEPs mais conhecidas da comunidade Python, que estabelece um guia de estilo para a escrita de código Python. O objetivo da PEP8 é tornar o código Python mais legível, consistente e fácil de manter.

O guia de estilo da PEP8 abrange aspectos como a formatação de código, o uso de espaços em branco, o uso de nomes de variáveis, a organização de importações, o uso de comentários e outros detalhes importantes da escrita de código Python.


## Alguns Exemplos de orientações da PEP8
---
-   Usar quatro espaços para indentação, em vez de tabulação;
-   Limitar as linhas de código a 79 caracteres;
-   Usar nomes descritivos para variáveis, funções e classes;
-   Usar espaços em branco de forma consistente ao redor de operadores e depois de vírgulas;
-   Usar docstrings para documentar funções e módulos;
-   Organizar as importações em uma ordem específica.
-   Evite importar módulos inteiros, em vez disso, importe apenas as funções, classes ou constantes necessárias. Por exemplo, em vez de `import numpy`, use `from numpy import array` se você precisar apenas da classe `array`.
-   Use espaços em branco para separar classes e funções de outras declarações de código. Por exemplo, inclua duas linhas em branco entre duas classes ou funções diferentes.
-   Use letras maiúsculas separadas por sublinhados para nomear constantes, como `MAX_ITERATIONS` ou `DEFAULT_CONFIG`.
-   Evite usar caracteres não-ASCII em identificadores de código, a menos que seja necessário para fins linguísticos. Use nomes descritivos em inglês sempre que possível.
-   Evite usar identificadores com nomes que sejam muito semelhantes, como `l` (letra minúscula "L") e `1` (número um), pois isso pode levar a confusão.
-   Use uma docstring para documentar cada módulo, função ou classe. A docstring deve começar com uma única linha de descrição, seguida de uma linha em branco e, em seguida, uma descrição mais detalhada. A PEP257 fornece orientações adicionais para a escrita de docstrings.
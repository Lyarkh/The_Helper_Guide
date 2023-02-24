#github #semantico 

## Regra 01 - API pública

No [documento original](https://semver.org/lang/pt-BR/) do versionamento semântico é definido que  qualquer software que esteja utilizando o versionamento semântico *deve* definir uma API pública, seja no código-fonte ou em sua documentação.


## Regra 02 - Formato do número de versão

Obrigatoriamente o versionamento semântico deve ter seu formato de versão conforme x.y.z onde, todos devam ser números inteiros e não negativos e não deve existir zeros à sua esquerda, ou seja, a versão semântica deverá sempre iniciar com 1.

Além do mais cada bloco deverá ter seu nome onde “x” será a versão principal ou maior, “y” a versão secundária ou menor e “z” a versão de correção ou patch.


## Regra 03 - Versões imutáveis

O documento original é bem claro quanto a essa regra onde uma vez determinada e disponibilizada, a versão do software não poderá ser modificada em hipótese alguma. Assim sendo, caso ocorra qualquer necessidade de correção de bug, modificações, atualizações ou nova funcionalidade deverá ser lançada uma nova versão.


## Regra 04 - Desenvolvimento inicial

No desenvolvimento inicial de um software sua primeira versão deverá ser setada como zero, isso deve-se ao fato de que muita coisa poderá mudar a qualquer momento antes do seu lançamento e com isso sua versão inicial não pode e nem deve ser considerada estável.

Em outras palavras, um software com sua versão inicial definida poderá mudar a qualquer hora porém, não quer dizer que versões anteriores ou dependências não poderão ser utilizadas em projetos.


## Regra 05 - Versão 1.0.0

Uma API pública poderá ser considerada “definida” a partir da versão 1.0.0 ou seja, versões futuras deverão ser baseadas ou dependentes dessa versão ou conforme ela é modificada.

Assim sendo, uma versão 1.0.0 por exemplo, nunca poderá ser baseada em uma versão 0.8.0 da API pública. Porém versões superiores deverão de alguma forma ser dependentes da versão 1.0.0.


## Regra 06 - Versão de remendo ou patch version

Essa regra define que a versão de remendo, correção ou patch deverá indicar a correção de um ou mais bugs que se mantém compatível com a versão anterior. Ou seja, uma versão 1.0.1 corrige um problema na versão 1.0.0 e será totalmente compatível com a mesma.


## Regra 07 – Versão secundária ou minor version

O conceito de versão secundária mostra que a correção está sendo lançada relacionada com o versionamento anterior de correção (patch). Essa versão secundária apenas poderá ser implementada sob as seguintes condições:
- Quando forem adicionadas novas funcionalidades, porém ainda assim compatíveis com as versões anteriores.
- Quando houver depreciação de alguma funcionalidade já publicada.
- Quando houverem novas funcionalidades ou melhorias introduzidas ao código.

Além disso sempre que houver o lançamento de uma versão secundária para correção de bugs de versões anteriores a numeração da versão de remendo deverá ser zerada. Por exemplo, um projeto lançado na versão 1.0.6 que teve sua versão secundária publicada para correção de algum bug será setado para 1.1.0 e não 1.1.6.


## Regra 08 – Versão principal ou major version

Em outras palavras, sempre que alterações incompatíveis com versões anteriores forem implementadas na versão principal da API pública as versões menores e de alterações deverão ser resetadas para 0 (zero).

Seguindo texto original da documentação, é dito o seguinte:
*“Major version X (X.y.z | X > 0) MUST be incremented if any backwards incompatible changes are introduced to the public API. It MAY include minor and patch level changes. Patch and minor version MUST be reset to 0 when major version is incremented”.*


## Regra 09 – Versão de pré-lançamento ou pré-release

A nona regra trata de versões de pré-lançamento e explica que:

Uma versão de pré-lançamento será indicada quando um hífen e uma séries de identificadores separados por pontos estiverem presentes logo após a versão do patch. Esses identificadores deverão conter apenas caracteres alfanuméricos ASCII e hífen (0-9A-Za-z). Além disso os identificadores NÃO DEVEM estar vazios e NEM incluir zeros à sua esquerda.

Embora não seja obrigatório nos números de versão padronizados por versionamento semântico, podem ajudar em algumas situações.


## Regra 10 – Dados de build

A décima regra é apenas mais uma regra adicional, portanto pode ser classificada como opcional. Segundo essa regra, é possível, se necessário adicionar informações extras de build junto à versão utilizando o caractere “+” seguido de informações adicionais separadas por pontos e que contenham apenas caracteres alfanuméricos e hífen. Podem ser adicionados como dados de build por exemplo o timestamp de quando o build foi criado ou até mesmo um hash do commit ou arquivos de build.


## Regra 11 – Precedência de versões

Na décima primeira regra é falado sobre algo muito importante e utilizado por gerenciadores de dependências como o Bower e o Composer por exemplo. Em resumo essa regra define a ordem em que as versões do versionamento semântico deverá ter. No caso do versionamento semântico essa ordem será numérica (1.0.0 < 2.0.0 < 3.0.0 < 3.1.0) e assim por diante. Além disso essa ordem poderá contar com algumas características adicionais.

- cada identificador deverá ser comparado da esquerda para a direita
- identificadores compostos serão comparados numericamente
- identificadores contendo letras ou hífens serão comparados lexicalmente conforme a organização da tabela ASCII onde A < a < b
- Caso os identificadores estejam misturados entre numéricos e não-numéricos os não-numéricos terão precedência aos numéricos
- Caso os identificadores estejam misturados entre numéricos e não-numéricos os não-numéricos terão precedência aos numéricos
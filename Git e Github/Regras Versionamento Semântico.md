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
`tags:` #devops #automacao

O makefile sempre são compostos por regras (_rules_). Cada regra contém 3 elementos.
 - O **alvo (target)**
 - Os **pré-requisitos**
 - As **instruções ( recipe)**

```python
# Alvo Pré-requisitos 
target ... : prerequisites ... 
# Instruções 
	recipe 0 
	recipe 1 
	recipe 2 
	...
```

A partir de uma regra, seu funcionamento deve ser entendido da seguinte maneira:
	Para gerar o alvo, é necessário existirem os pré-requisitos e executar todas as instruções.


### Falando especificamente de cada um dos elementos
---

### Alvo

O alvo (_target_) é o nome que identifica uma regra. Ele pode ser também o conjunto de arquivos ou apenas um arquivo resultante do processo de compilação daquela regra à qual pertence. Um arquivo binário executável, por exemplo


### Pré-requisitos

Os pré-requisitos (_prerequisites_) são o todas as dependências obrigatórias para que o alvo possa ser gerado. Ou seja, os arquivos de código fonte, por exemplo.


### Instruções

As instruções (_recipes_) são o conjunto de comandos que devem ser executados para gerar o alvo. Um exemplo seria executar o programa [GNU gcc](https://gcc.gnu.org/) para compilar um arquivo de código. 

<font color='red' >Obs: Um detalhe importante sobre as instruções é que elas devem ser indentadas com tabs e nunca espaços. É uma restrição do formato _Makefile_. </font>

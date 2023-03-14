#DevOps #automação

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
Criação de ambientes  virtuais em python são essenciais para o desenvolvimento de aplicações e programas.  Que pode fazer com que as bibliotecas instaladas em nossa máquina não entre em  conflito de versões com as bibliotecas dos projetos.

Existe diversas formas de se criar ambientes virtuais em python. Uma das mais famosas e mais utilizadas é o `venv`.

venv é um módulo do python que ajuda na criação de ambiente virtuais, o gerenciador de pacotes mais utilizado em conjunto é o `pip`.

A criação de um ambiente virtual `venv` e feito da seguinte maneira:

Abra o `bash`, `PowerShell` ou o seu prompt de comando/terminal de sua preferência e digite o seguinte comando:

```bash
	python -m venv venv
```

Para ativação do utilize o seguinte comando:

No PowerShell:
```bash
	venv/Scripts/Activate.ps1
```

No CMD:
```bash
	venv/Scripts/activate.bat
```

Logo após feito o ambiente virtual, e ativado, pode-se baixar as dependências sem nenhum conflito com nenhum projeto a parte ou bibliotecas instaladas no próprio sistema.


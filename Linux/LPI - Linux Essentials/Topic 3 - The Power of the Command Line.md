
## 3.1 Archiving Files on the Command Line (weight: 2)

O arquivamento de arquivos na linha de comando envolve a criação de um único arquivo que contém um ou mais arquivos ou diretórios. Isso é útil quando você precisa transferir um grande número de arquivos ou diretórios ou quando deseja compactá-los para economizar espaço em disco.

O comando `tar` é comumente usado para criar e manipular arquivos de arquivamento. Para criar um novo arquivo de arquivamento, use o seguinte comando:

```bash
tar -cvf archive.tar file1 file2 directory1
```

Neste comando, a opção `-c` indica ao `tar` para criar um novo arquivo de arquivamento, `-v` significa "verbose" e exibe a lista de arquivos sendo arquivados, e `-f` especifica o nome do arquivo de arquivamento. É possível substituir `archive.tar` por qualquer nome desejado para o arquivo de arquivamento. `file1`, `file2` e `directory1` são os arquivos e diretórios que você deseja arquivar.

Para extrair os arquivos de um arquivo de arquivamento, use o seguinte comando:

```bash
tar -xvf archive.tar
```

A opção `-x` indica ao `tar` para extrair os arquivos, e o resto do comando especifica o nome do arquivo de arquivamento que você deseja extrair.

O comando `tar` também pode ser usado para comprimir arquivos usando o gzip ou o bzip2. Para isso, basta adicionar a opção `-z` para gzip ou `-j` para bzip2 ao comando `tar`. Por exemplo:

```bash
tar -czvf archive.tar.gz file1 file2 directory1
```

Neste comando, a opção `-z` indica que o arquivo deve ser compactado com o gzip e o arquivo resultante será nomeado como `archive.tar.gz`. É possível substituir `file1`, `file2` e `directory1` pelos arquivos e diretórios que você deseja arquivar.
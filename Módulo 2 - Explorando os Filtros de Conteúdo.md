### Comandos Linux

#### Filtros

- `grep "laranja" /home/edilson/filtros_de_conteudo/arquivo1`: Procura por linhas que contenham a palavra "laranja" no arquivo1.
- ![egrep1](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/74eae3e5-344d-4408-aa88-f4f22fdbe468)
- `grep -v "laranja" /home/edilson/filtros_de_conteudo/arquivo1`: Exclui linhas que contenham a palavra "laranja" no arquivo1, ou seja, retorna todas as linhas que não contêm "laranja".
- ![egrep -v 1](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/312d2b85-7cf2-4431-be39-92f07442472e)
- ![egrep -v 2](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/1fe38fe5-b25a-4c67-b4bf-40f8000a40e3)
- `grep -r "laranja" /home/edilson/filtros_de_conteudo/arquivo1 | cat`: Procura recursivamente por "laranja" em arquivo1 e exibe os resultados, mesmo que seja vazio. O comando `cat` é usado para evitar que `grep` pause a saída em caso de grandes volumes de dados.
- ![egrep 3](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/4726f9df-e935-44d1-9747-d8a62061fd87)


### `wc`: Conta o número de linhas, palavras e caracteres de entrada.

- `ls -l | wc -l`: Conta o número de linhas resultantes do comando "ls -l", ou seja, o número total de arquivos e diretórios listados.
- `ls -l /home/edilson | grep ^d | wc -l`: Conta o número de diretórios no diretório "/home/edilson". O `ls -l` lista os detalhes de todos os arquivos e diretórios, o `grep ^d` filtra apenas as linhas que começam com "d", indicando diretórios, e o `wc -l` conta o número de linhas resultantes.
- `ls -l | wc -w`: Conta o número de palavras resultantes do comando "ls -l", ou seja, o número total de arquivos e diretórios listados.
- `ls -l | wc -c`: Conta o número de caracteres resultantes do comando "ls -l", ou seja, o tamanho total da saída do comando "ls -l" em bytes.
- ![egrep 3](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/fc838428-6f07-4c41-b911-a752424fb5b7)


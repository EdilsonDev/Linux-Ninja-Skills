### Filtros de Conteúdo

#### GREP : O grep é uma ferramenta de busca por padrões em arquivos de texto.

- `grep "laranja" /home/edilson/filtros_de_conteudo/arquivo1`: Procura por linhas que contenham a palavra "laranja" no arquivo1.
- ![egrep1](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/2ab02265-9ac7-4be1-b906-1d64eaabe556)
- `grep -v "laranja" /home/edilson/filtros_de_conteudo/arquivo1`: Exclui linhas que contenham a palavra "laranja" no arquivo1, ou seja, retorna todas as linhas que não contêm "laranja".
- ![egrep -v 1](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/312d2b85-7cf2-4431-be39-92f07442472e)
- ![egrep -v 2](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/1fe38fe5-b25a-4c67-b4bf-40f8000a40e3)
- `grep -r "laranja" /home/edilson/filtros_de_conteudo/arquivo1 | cat`: Procura recursivamente por "laranja" em arquivo1 e exibe os resultados, mesmo que seja vazio. O comando `cat` é usado para evitar que `grep` pause a saída em caso de grandes volumes de dados.
- ![egrep 3](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/4726f9df-e935-44d1-9747-d8a62061fd87)


#### WC : Conta o número de linhas, palavras e caracteres de entrada.

- `ls -l | wc -l`: Conta o número de linhas resultantes do comando "ls -l", ou seja, o número total de arquivos e diretórios listados.
- `ls -l /home/edilson | grep ^d | wc -l`: Conta o número de diretórios no diretório "/home/edilson". O `ls -l` lista os detalhes de todos os arquivos e diretórios, o `grep ^d` filtra apenas as linhas que começam com "d", indicando diretórios, e o `wc -l` conta o número de linhas resultantes.
- `ls -l | wc -w`: Conta o número de palavras resultantes do comando "ls -l", ou seja, o número total de arquivos e diretórios listados.
- `ls -l | wc -c`: Conta o número de caracteres resultantes do comando "ls -l", ou seja, o tamanho total da saída do comando "ls -l" em bytes.
- ![wc](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/4ba67cb5-db73-4c1c-8615-1d64ec11e4eb)

#### TR: Traduz e/ou deleta caracteres da entrada padrão, exibindo o resultado como saída.
- `ls -la | tr edilson "*"`: Lista todos os arquivos e diretórios no diretório atual, incluindo arquivos ocultos, com detalhes. Em seguida, substitui todas as ocorrências das letras 'e', 'd', 'i', 'l', 's' e 'o' por '*' nos resultados exibidos.
- ![tr](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/660fb772-5f7a-4a35-8c9d-a10063cea722)
  
#### SED: Filtra e transforma texto.

- `ls -la | sed 's/edilson/ninja /g'`: Lista todos os arquivos e diretórios no diretório atual, incluindo arquivos ocultos, com detalhes. Em seguida, substitui todas as ocorrências de "edilson" por "ninja" nos resultados exibidos.
- ![sed](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/bef953ac-4058-4475-b24e-12fc9b0f458a)

#### DIFF: Compara o conteúdo de dois arquivos e mostra as diferenças entre eles.

- `diff arquivo_x arquivo_y`: Compara o conteúdo dos arquivos "arquivo_x" e "arquivo_y" e exibe as diferenças entre eles.
- ![diff](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/6ef5ce62-969f-4099-988c-14c6d9168237)

#### SORT: Ordena alfabeticamente um arquivo específico ou a entrada padrão.

- `tree | sort`: Exibe a estrutura de diretórios e arquivos de forma hierárquica usando o comando "tree", e então ordena alfabeticamente as saídas usando o comando "sort".
- ![sort](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/e2159c50-4c95-447b-b729-1c32644ce6a2)


#### AWK: Exibe partes ou seções de cada linha de um arquivo específico ou da entrada padrão.

- `ls -la | awk '{if (NR>1) $3=gensub(/edilson/, "ninja", "g", $3); print $0}'`: Lista todos os arquivos e diretórios no diretório atual, incluindo arquivos ocultos, com detalhes. Em seguida, substitui todas as ocorrências de "edilson" por "ninja" no terceiro campo (proprietário) dos resultados exibidos, exceto na primeira linha.
- ![awk](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/70301262-b02c-4130-aae5-45efe49f1162)

- `ls -la | awk '{$3=gensub(/edilson/, "ninja", "g", $3); print $0}'`: Lista todos os arquivos e diretórios no diretório atual, incluindo arquivos ocultos, com detalhes. Em seguida, substitui todas as ocorrências de "edilson" por "ninja" no terceiro campo (proprietário) dos resultados exibidos.
- ![awk2](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/92c483c5-2739-4701-944c-1895f033c66a)


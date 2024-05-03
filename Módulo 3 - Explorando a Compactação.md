### Compactadores

#### ZIP E UNZIP: O comando 'zip' comprime arquivos e diretórios em um arquivo compactado, ao passo que 'unzip' extrai arquivos desse arquivo compactado.

- `zip -r backup.zip /home/edilson`: Compacta o diretório /home/edilson e todos os seus conteúdos em um arquivo zip chamado backup.zip.
- ![zip](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/10acb829-61d7-4923-8564-67ee1dbbbcbf)
  
- `unzip backup.zip -d /home/edilson/backup/safestorage/`: Extrai os arquivos do arquivo zip backup.zip para o diretório /home/edilson/backup/safestorage/.
- ![unzip](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/efdfd62a-f65d-4949-9548-15835cdf92b0)

#### TAR: O comando tar é utilizado para agrupar, compactar e extrair arquivos em formato tar.

##### Compactando
- `tar czf backup.tar.gz safestorage`: Compacta o diretório safestorage em um arquivo backup.tar.gz.
- ![tar](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/27de6fe2-469c-4ebc-a106-5189335c1fbe)

- `tar cf backup_empacotado.tar safestorage/`: Empacota o conteúdo do diretório safestorage em um arquivo backup_empacotado.tar.
- ![tar2](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/e3de0572-0e62-4188-a006-61c2ad613648)

##### Descompactando

- `tar xzf backup.tar.gz`: Extrai os arquivos do arquivo backup.tar.gz no diretório atual.
- ![untar](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/03dcd118-e834-44ba-b7a0-de9152384d6f)

- `tar -xvf backup_empacotado.tar -C backup/`: Extrai os arquivos do arquivo backup_empacotado.tar no diretório backup/.
- ![untar2](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/b71d306b-abe7-4849-b8f6-c4ea060b61c9)

Ao usar o comando "tar" para compactar/descompactar, temos a opção de escolher entre três tipos de compactadores:

- "gzip" → extensão ".tar.gz" (amplamente utilizado e eficiente na compressão);
- "bzip2" → extensão ".tar.bz2";
- "compress" → extensão ".tar.Z".

### Sintaxe:

tar <opções> [arquivo] <opções || caminho_a_ser_compactado>

- `c`: Compacta dados em um novo arquivo.
- `x`: Extrai o conteúdo de um arquivo compactado.
- `t`: Lista o conteúdo de um arquivo compactado.
- `v`: Mostra na tela o que está sendo compactado ou descompactado.
- `p`: Preserva as permissões do arquivo original.
- `r`: Adiciona arquivos ao pacote "tar".
- `z`: Usa o compressor "gzip".
- `Z`: Usa o compressor "compress".
- `j`: Usa o compressor "bzip2".
- `f`: Especifica que o alvo é um arquivo (o padrão é dispositivo de fita).


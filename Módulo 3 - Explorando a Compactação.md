### Compactadores

#### ZIP E UNZIP: O comando 'zip' comprime arquivos e diretórios em um arquivo compactado, ao passo que 'unzip' extrai arquivos desse arquivo compactado.

- `zip -r backup.zip /home/edilson`: Compacta o diretório /home/edilson e todos os seus conteúdos em um arquivo zip chamado backup.zip.
- ![zip](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/10acb829-61d7-4923-8564-67ee1dbbbcbf)
- `unzip backup.zip -d /home/edilson/backup/safestorage/`: Extrai os arquivos do arquivo zip backup.zip para o diretório /home/edilson/backup/safestorage/.
- ![unzip](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/efdfd62a-f65d-4949-9548-15835cdf92b0)

#### TAR:

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

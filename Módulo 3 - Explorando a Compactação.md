### Compactadores

#### ZIP E UNZIP: O comando 'zip' comprime arquivos e diretórios em um arquivo compactado, ao passo que 'unzip' extrai arquivos desse arquivo compactado.

- ![zip](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/546d0995-30df-4c7b-80eb-d16c30747462)
- ![unzip](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/45361914-3c1a-484e-9d07-bb9dc2ef916d)

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

### Comandos Básicos Linux

#### Dicas de Terminal

- Setas: Acessa comandos anteriores.
- SHIFT + PGUP/PGDOWN: Visualiza histórico.
- CTRL+A: Move cursor para o início da linha.
- CTRL+E: Move cursor para o fim da linha.
- CTRL+L: Limpa tela.
- CTRL+R: Busca por comandos anteriores.
- TAB: Auto completar comandos.
- ~ (til): Atalho para diretório pessoal.

#### Alternância entre Terminais

- ALT + F1 a F6: Modo texto.
- ALT + F7: Terminal gráfico.
- CTRL+ALT+F1 a F6: Gráfico para texto.
- Comandos para encerrar terminal/sessão: `exit`, `logout`, CTRL + D.
- Comandos para desligar o sistema: `shutdown -h now`, `init 0`, `halt`, `poweroff`.
- Comandos para reiniciar o sistema: `reboot`, `init 6`, CTRL + ALT + DEL.

#### Diretórios do Linux

- `/`: Raiz do sistema.
- `/boot`: Inicialização.
- `/etc`: Configurações e serviços.
- `/bin`, `/sbin`: Comandos básicos e administração.
- `/var`: Logs e dados.
- `/root`: Usuário root.
- `/home`: Diretório de usuários.
- `/dev`: Dispositivos.
- `/lib`: Bibliotecas.
- `/proc`: Sistema de arquivos do kernel.
- `/usr`: Arquivos de usuários.

#### Comandos de Ajuda

- `man comando`
- `comando --help`
- `date`, `cal 2020`
- `clear` ou `CTRL + L`

#### Navegação

- `ls`, `cd`, `pwd`

#### Manipulação de Arquivos/Diretórios

- `mkdir`: Cria diretório.
- ![mkdir](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/2d31f20a-c866-4174-b2a7-b40abfd33569)
- `rmdir`: Apaga diretório vazio.
- ![rmdir](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/53df29a9-4bd4-4eda-a9f7-c7d44eed2b91)
- `rm`: Apaga arquivo/diretório.
- ![rm](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/7a8525b7-907c-40b9-b495-90e9b072ba67)
- `mv`: Move ou renomeia.
- ![mv](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/77d09af3-5eb6-463b-b7b9-43b7e0784acb)
- `cp`: Copia.
- ![cp](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/3c7ff4fd-7617-4bc7-97c6-c8624ad41884)
- `touch`: Cria arquivo de texto.
- ![touch](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/8df7afc8-3dc2-4d4d-a0f2-5ad735d0899f)
- `ln`: Cria Links simbólicos ou "rígidos".
- ![link](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/a8f98614-e7c1-451a-b759-68f458e36052)
- `find`: Procura arquivos.
- ![find](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/3cab1f0c-34e9-4938-8eac-8dbf2c1c62de)
- `du`: Mostra espaço em disco.
- ![du](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/51464b51-5cbf-4b3a-9098-7e258b3597fb)
- `tree`: Mostra estrutura de diretórios.
- ![tree](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/59e154f8-cea4-46c2-ba7f-e7d52832ba06)

### Comando `ls -lah`

- **Primeira coluna**: Tipo e permissões do arquivo.
  - `d`: Diretório.
  - `-`: Arquivo comum.
  - `l`: Link.
  - `b`: Dispositivo de blocos.
  - **Permissões**: `r` (leitura), `w` (escrita), `x` (execução).
- **Segunda coluna**: Total de inodes.
- **Terceira coluna**: Usuário proprietário.
- **Quarta coluna**: Grupo proprietário.
- **Quinta coluna**: Tamanho do arquivo.
- **Sexta coluna**: Data de modificação.
- **Sétima coluna**: Nome do arquivo ou diretório.

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
- -![rmdir](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/2810a5a8-2eb6-46a4-a9c2-b94621974827)
- `rm`: Apaga arquivo/diretório.
- ![rm](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/7a8525b7-907c-40b9-b495-90e9b072ba67)
- `mv`: Move ou renomeia.
- ![mv](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/77d09af3-5eb6-463b-b7b9-43b7e0784acb)
- `cp`: Copia.
- ![cp](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/faea8f24-ba1f-4aea-98e9-30bc5c8ddc13)
- `touch`: Cria arquivo de texto.
- ![touch](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/8df7afc8-3dc2-4d4d-a0f2-5ad735d0899f)
- `ln`: Cria Links simbólicos ou "rígidos".
- ![link](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/58a18a64-4e00-4a7a-ac12-591ae090959d)
- `find`: Procura arquivos.
- ![find](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/b0a5e245-26a6-427b-ae84-914232de8fde)
- `du`: Mostra espaço em disco.
- ![du](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/dd3beff4-735a-48c6-9b59-cb280a7110b7)
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
- **Sétima coluna**: Nome do arquivo ou diretório. <br/>
![ls la](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/8a73f353-9002-4f49-83d2-6fea4167199e)

### Visualizadores de texto

- `cat`: Concatena e exibe arquivos.
- `more`: Exibe conteúdo com rolagem por página.
- `less`: Exibe conteúdo com rolagem e busca.
- `head`: Exibe as primeiras linhas de um arquivo.
- `tail -f`: Exibe as últimas linhas de um arquivo em tempo real. <br/>
![1](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/4db72c8a-9fc4-4d42-8322-d087a5bdccd1)

### Redirecionadores

- `ls > /home/edilson/allow_file`: Substituição.
- ![sub](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/3654e512-fcfe-4973-96ce-60262e8c54ec)
- `ls -la >> /home/edilson/allow_file`: Adiciona ao final do texto.
- ![add](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/91783743-838d-4363-92f9-1b2d9d6a40ec)
- `< /home/edilson/allow_file less`: Exibe o conteúdo do arquivo.
- ![es](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/bcd42c23-89a2-4f66-9c8d-8ce418120178)
- `cat >> allow_file << EOF`: Adiciona texto ao arquivo até encontrar "EOF".
- ![EOF](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/b8bb6a33-f96f-4cfa-b0d4-c425e5bcb3f7)
- `find / -name group 2> /home/edilson/allow_file > /home/edilson/allow_file`: Procura por arquivos chamados "group" em todo o sistema e redireciona a saída de erro para /home/edilson/allow_file, resultando em um arquivo vazio ou truncado devido à ordem das redireções.
- ![2](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/d2ecec2c-7e5b-4a27-b5d1-5cfeb02ae6ac)
- ![3](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/c6a728a2-fa2c-49d7-b419-da78767d1cfe)





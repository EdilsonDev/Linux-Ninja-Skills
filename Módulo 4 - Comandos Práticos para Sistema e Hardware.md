### Gerenciando Sistema e Hardware

#### Informações do sistema

- `uname -a`: Exibe informações do sistema, incluindo o nome do kernel, nome do host, versão do kernel, data de compilação, arquitetura do sistema e informações do processador.
  (Para identificar a distribuição, normalmente há um arquivo importante localizado em "/etc".)
- ![uname](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/889e92ae-b3d4-47cf-91d6-92c3313ecd7e)
- `uptime`: Mostra há quanto tempo o sistema está rodando, bem como a carga média durante diferentes intervalos de tempo.
- ![uptime](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/9e2cdb01-0568-478c-a53b-a43f4299ce60)
- `w`: Exibe uma lista de usuários atualmente conectados ao sistema, bem como informações sobre a carga média e os processos em execução de cada usuário.
- `who`: Mostra uma lista de usuários conectados ao sistema.
- `whoami`: Retorna o nome do usuário atualmente logado.
- ![logon](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/6e440687-ac12-4993-8fe0-981b820c08af)

#### Informações de memória

- `free -m`: Exibe informações sobre o uso da memória RAM do sistema em megabytes.
- `free -s 20`: Exibe informações sobre o uso da memória RAM do sistema em intervalos de 20 segundos.
- ![free](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/4ea5a78d-5127-47ec-b6a9-6fc7d5bd4e30)

#### Informações de rede

- `sudo nmcli connection delete eth0`: Remove a conexão de rede Ethernet "eth0" usando o NetworkManager.
- ##### OBS. Antes de executar o comando, verifique se o `dhclient` está instalado. Se não estiver, você pode instalá-lo executando o seguinte comando em distribuições derivadas do Debian: `sudo apt update && sudo apt install isc-dhcp-client`, ou em distribuições derivadas do CentOS: `sudo yum install -y dhclient`.
- `sudo dhclient eth0`: Renova o endereço IP da interface de rede Ethernet "eth0" usando o cliente DHCP.
- ![delete and dhclient](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/edf78a3a-7b9f-4129-a890-c41e1f9b1824)

- `ip address ou ifconfig`: Exibe todas as informações de endereço IP das interfaces de rede.
- ![ipaddress](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/7269f226-7281-4c2b-8a7d-9cfe48c2aedc)

- `ip address list eth0`: Exibe informações detalhadas sobre o endereço IP da interface de rede Ethernet "eth0".
- `ip address flush dev eth0`: Remove todos os endereços IP da interface de rede Ethernet "eth0".
- ![list and flush](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/2c2bb1bb-417f-4ee7-a4f7-6fd796ec225e)

- `sudo route add default gw 10.1.1.1`: Adiciona uma rota padrão com um gateway de rede especificado (10.1.1.1) usando o comando "route".
- `sudo route del default gw 10.1.1.1`: Remove a rota padrão com o gateway de rede especificado (10.1.1.1) usando o comando "route".
- `route -n`: Exibe a tabela de roteamento do sistema.
- ![default gw](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/6d810e0d-ff2b-4fa1-b32e-33351c34d9af)

- `ip route`: Exibe informações detalhadas sobre a tabela de roteamento do sistema usando o utilitário "ip".
- ![iproute](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/96ace1cd-a4c4-4afb-9925-4b0b5b2d1c0b)

##### OBS. Configurações feitas com os comandos 'ifconfig', 'ip address' e 'route' são temporárias e serão perdidas após a reinicialização do computador

#### Informações sobre Hardware

- `dmesg`: Exibe mensagens do kernel, que podem incluir informações de inicialização do sistema e eventos relacionados ao hardware.
- ![dmesg1](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/f7f45f09-22f6-415c-bf22-9d45688ea494)
- ![dmesg2](https://github.com/EdilsonDevops/Linux-Ninja-Skills/assets/96980587/66c5cc88-e159-438c-833b-0a9d702d5782)
- `lspci`: Lista todos os dispositivos PCI conectados ao sistema, fornecendo informações detalhadas sobre cada um deles.
- `lsmod`: Lista todos os módulos do kernel carregados no sistema.
##### OBS. 'insmod [arquivo] <opções>': Carrega um módulo do kernel especificado a partir de um arquivo, `rmmod <nome_do_modulo>': Remove um módulo do kernel carregado.
- `cat /proc/cpuinfo`: Exibe informações sobre a CPU do sistema, como modelo, velocidade e recursos.
- `cat /proc/scsi/scsi`: Fornece informações sobre dispositivos SCSI, SATA ou SAS conectados ao sistema.
- `fdisk -l`: Lista todas as partições de disco no sistema, incluindo detalhes como tamanho, tipo de sistema de arquivos e rótulo.

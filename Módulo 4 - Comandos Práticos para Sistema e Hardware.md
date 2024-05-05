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
- `sudo dhclient eth0`: Renova o endereço IP da interface de rede Ethernet "eth0" usando o cliente DHCP.
- `ip address`: Exibe todas as informações de endereço IP das interfaces de rede.
- `ip address list eth0`: Exibe informações detalhadas sobre o endereço IP da interface de rede Ethernet "eth0".
- `ip address flush dev eth0`: Remove todos os endereços IP da interface de rede Ethernet "eth0".
- `sudo route add default gw 10.1.1.1`: Adiciona uma rota padrão com um gateway de rede especificado (10.1.1.1) usando o comando "route".
- `sudo route del default gw 10.1.1.1`: Remove a rota padrão com o gateway de rede especificado (10.1.1.1) usando o comando "route".
- `route -n`: Exibe a tabela de roteamento do sistema.
- `ip route`: Exibe informações detalhadas sobre a tabela de roteamento do sistema usando o utilitário "ip".

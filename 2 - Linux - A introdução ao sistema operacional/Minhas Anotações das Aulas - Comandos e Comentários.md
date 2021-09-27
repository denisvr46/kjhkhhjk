# Linux - A introdução ao sistema operacional



* Linux é um Kernel. É o que da vida ao computador, é o que faz a intermediação entre o hardware e o sistema operacional.

* multitarefa/multiusuário

* Gnone é a interface gráfica do Ubuntu.

  
### Conhecendo o terminal Linux e seus atalhos

> ###### crtl + alt + t
Abre o terminal

> ###### ~
É a pasta pessoal, pasta home

> ###### pwd
Mostra a pasta que vc esta

> ###### ls
Lista o que tem no diretório

> ###### ls diretorio
Lista o que tem no diretório especificado

> ###### ls -l
Lista arquivos e diretórios com detalhes

> ###### mkdir pasta
Cria uma pasta

> ###### cd ..
Retorna um diretório anterior

> ###### cd / 
Retorna pro diretório raiz

> ###### man comando
Retorna o manual do comando exemplo " man ls "

> ###### comando --help
Retorna o manual de ajuda no idioma do computador

> ###### -a --all
Quando é usado a abreviação do comando é apenas um traço a palavra inteira é 2 traços

> ###### history
Lista todos os comandos usados nessa sessão do terminal

> ###### !!
Faz a mesma coisa que o comando "history"  lista todos os comandos usados nessa sessão do terminal

> ###### mv nomeantigo nomenovo
> ###### mv arquivo.txt arquivonovonome.txt
O comando mv altera o nome também

> ###### cp arquivo.txt /home/denis
Copia o arquivo para outra pasta

> ###### rmdir diretório 
Remove diretório

> ###### rm arquivo.txt
Remove arquivo


### Comandos para manipulação de arquivos e textos e redirecionamento

* Nano editor de arquivo 

> ###### nano nome arquivo.txt
Abre o arquivo.txt no editor nano

* no nano o simbolo "^" do menu significa control e o "m" siginifica alt

> ###### cat arquivo.txt
Exibe o que contem no arquivo.txt no próprio terminal

> ###### tac arquivo.txt
Pega o arquivo.txt de tras pra frente(linhas) e exibe 

> ###### head arquivo.txt
Exibe as 10 primeiras linhas 

> ###### tail arquivo.txt
Exibe as 10 ultimas linhas 

> ###### head teste.txt > arquivocomhead.txt
O operador ">" cria um arquivo novo baseado nas 10 primeiras linhas nesse caso por causa do head

> ###### cal
Exibe o calendário

> ###### date
Mostra a data hora daquele instante

* O operador ">" cria um arquivo baseado em um outro
* O operador ">>" concatenas arquivos 
* cat arquivo_um.txt >> arquivo_dois.txt
  Onde o cat arquivo_um.txt pega o conteúdo e insere no arquivo_dois.txt

> ###### cat arquivo_um.txt | grep palavra
Procura no arquivo_um.txt a palavra grep o "|" concatena comando e o grep localiza palavra

> ###### cat arquivo.txt | more
O "| more" faz a paginação de um arquivo, exibindo o texto em pequenas partes

> ###### cat arquivo.txt | less
O "| less faz o mesmo que o more,a paginação de um arquivo, exibindo o texto em pequenas partes

> ###### cat  arquivo_um.txt & cat arquivo_dois.txt
Exibe os dois arquivos no terminal em duas saidas separadas

> ###### cat arquivo_um.txt && cat arquivo_dois.txt
Exibe os dois arquivo no terminal em uma unica saida do terminal

> ###### mkdir pasta && cd linux
Aqui o operador && cria a pasta e já vai para este diretório

> ###### file arquivo.txt
O comando file serve para informar o tipo do arquivo

> ###### whatis comando
Ele exibe o que o comando faz

> ###### find diretorio -name arquivo.txt
O comando find busca e exibe o caminho de um arquivo que deseja procurar

> ###### rm -r*
Remove todos arquivos de um diretório

> ###### rm -r arquivo.txt
Apaga o arquivo.txt

> ###### rm aquivo.zip
Apaga o arquivo

> ###### rm -r compactar*
Remove todos arquivos do diretório que comecem com compactar

> ###### rm -r *zip
Remove todos arquivos que são do formato zip

### Diretórios do Linux e Comandos de Sistema


> ###### echo -e "denis\n"
Imprime o texto com quebra de linha sendo que o parametro "-e" é o que permite isso e "\n" o comando de quebra de linha

> ###### lscpi
Lista as placas pci do computador (placa de rede som)

> ###### lsusb
Lista os dispositivos usb

> ###### arch
Mostra a arquitetura do sistema

> ###### uname
Mostra o kernel usado

> ###### uname -r
Mostra a versão do kernel

> ###### uname -m
Mostra a arquitetura do kernel

> ###### free
> Mostra a memoria

> ###### lscpu
Lista as informações de cpu

> ###### lshw
Lista todos hardwares do sistema

> ###### du -h diretorio | more
Mostra a utilização do hd

> ###### cat /etc/passwd
Mostra todos usuarios do sistema

> ###### reboot 
Reinicia a maquina

> ###### shutdown - h now
Desliga o computador agora

* bash terminal

  

### Fundamentos de Rede e Comandos de Rede



* **Rede de computadores** é um conjunto de equipamentos interligados de maneira a trocarem informações e compartilharem recursos, como arquivos,impressoras,modems,softwares e outros equip.
* Cada equipamento é um nó, sao pontos de rede.
* **Rede Wan** de área mundial, geograficamente distribuída
* **Rede Man** são redes metropolitas, englobam cidades
* **Rede Lan** São redes locais, em um unico predio, redes de casa
* **Protocolos (IP,ICMP,DNS)** É a linguagem utilizada pelos dispositivos para que consigam se entender
* **IP** Números que identificam seu computador na rede
* **ICMP** Objetivo prover mensagens de controle na comunicação entre nós
* **DNS** Identifica endereços IP
* **Interface de rede** É um software ou hardware que faz a comunicação em uma rede de computadores
No linux elas estão na pasta /dev 
eth0 - placa
* **Interface Loopback** Permite fazer uma conexão com vc mesmo
O IP 127.0.0.1 é um exemplo de loopback



> ###### ifconfig
> Faz parte do comando net-tools
> inet é o endereço ip na minha rede local
> netmask é o numero que separa a rede publica da rede privada
> broadcast é como se fosse um endereço publico da rede local
> inet6 é o endereço ipv6, ele é hexadecimal
> ether é o endereço mac, é o endereço da placa de rede

> ###### hostname
> Obtém informações sobre o computador na rede

> ###### hostaname - I
> Obtém o endereço IP na rede

> ###### hostname - i
> Obtém o endereço IP de loopback

> ###### w
> Obtém as informações detalhadas sobre o usuario do computador na rede

> ###### who
> Obtém as informações de como estamos logados

> ###### whoami
> Obtém as informações do nome do usuário logado

> ###### ping www.google.com
> Obtém as informações se um whost esta ativo
> Ping é um pacote de requisição
> ping www.google.com -w 4
> Faz um ping com 4 requisições

> ###### dig www.google.com
> Obtém informações sobre o DNS 

> ###### dig www.google.com +short
> Mostra o ip do google 

> ###### traceroute www.google.com
> Traça a rota da sua maquina até o endereço desejado, qual o caminho dos nós até la

> ###### whois www.pudim.com
> mostra informações sobre o endereço 

> ###### finger 
> Mostra todas informações sobre o usuario logado (Nome, endereço, tempo logado, etc)
>
> 

### Fuçando no Linux com comandos diversos



> ###### ls -a
> lista os arquivos e diretorios ocultos

> ###### history
> Mostra os comandos executados

> ###### history -c
> Limpa o historico de comandos

> ###### alias abreviacao='history'
> Transforma/Apelida o comando no caso history para abreviacao

> ###### nl arquivo.txt
> Conta o numero de linhas de um arquivo

> ###### wc - l arquivo.txt
> Igual o nl, Conta o numero de linhas de um arquivo.

> ###### wc -w arquivo.txt
> Conta o numero de palavras no arquivo

> ###### wc -m arquivo.txt
> Exibe o numero de caracteres no arquivo

> ###### cmp arquivos.txt arquivo2.txt
> compara arquivos

> ###### diff arquivos.txt arquivo2.txt
> mostra a diferença entre arquivos

> ###### sort -n arquivo.txt
> Ordena o arquivo em ordem numerica

> ###### last reboot
> Mostra todas informações de reinialização do sistema

> ###### route -n
> Mostra todas tabelas de roteamento do nosso kernel

> ###### time
> Mostra o tempo de um processo

> ###### time traceroute www.google.com.br
> Mostra o tempo que demorou o comando

> ###### uptime
> Mostra o tempo que o sistema esta em execução

> ###### init 0
> Desliga maquina

> ###### telinit 0
> Desliga maquina

> ###### halt
> desliga maquina

> ###### seq 1 10
> Imprime uma sequencia de 1 a 10

> ###### which
> exibe o caminho de um programa

> ###### whereis
> exibe o caminho do programa e seu manual(man)

> ###### logout
> Finaliza sessão

> ###### https://bellard.org/jslinux/
> Maquina virtual do linux em java script



### Controle de usuários, grupos e permissões


> ###### sudo adduser usuario
> adiciona um usuario

> ###### su nomeusuario
> troca de usuario

> ###### passwd nomeusuario
> mudasenha

> ###### lastlog
> Mostra as informações de log de usuario, quando conectou

> ###### last
> Exibe listagem de entrada e saida de um usuario no sistema

> ###### logname
> Mostra o nome do usuario atualmente logado

> ###### id
> Vai exibir todos identificadores de usuario

> ###### cat /etc/passwd
> Exibe todos usuarios 

> ###### userdel -r nomeusuario
> Remove usuario e pasta pessoal dele

* GRUPOS: Permitem organizar usuarios e definir permissões de acesso e diretorio de forma + facil

> ###### cat /etc/group
> Esse arquivo mostra todos os grupos de usuario

> ###### groups
> Mostra os grupos que o usuario logado pertence.

> ###### sudo addgroup nomegrupo
> cria um grupo

> ###### sudo adduser usuario grupo
> adiciona um usuario ao um grupo

> ###### gpasswd -a usuario grupo
> adiciona um usuario ao um grupo

> ###### gpasswd -d usuario grupo
> Remove usuario de um grupo

> ###### groupdel grupo
> Remove um grupo




* **PERMISSÕES**: Servem para arquivos e diretórios restringir acessos como: Leitura, escrita e execução
r - read (leitura)
w - write (escrita)
x - eXecution (execução)

* owner grupo outros

* d diretorio

* -arquivo

  

> ###### ls -lh
> Verifica permissões em um diretorio(data,tamanho,usuarios..)

> ###### drwxr-xr-x 
(d)diretório 
(rwx) dono (leitura,escrita,execução) 
(r-x) grupo so tem permissão de leitura e execução
(r-x) outros tem permissão de leitura e execução

> ###### -rw-rw-r--
(-)arquivo
(rw-) dono tem permissão de leitura e escrita
(rw-) grupo tem permissão de leitura e escrita
(r--) outros permissão de leitura

> ###### chmod numeroOctal arquivoOuDiretorio
> Muda a permissão de um arquivo ou diretorio

### Compactação, Descompactação e Arquivamento




* **COMPACTADORES**: São programas que diminuem o tamanho de um arquivo ou diretorio

  

* #### GZIP  - Compactador do linux

> ###### gzip.arquivo.txt
> Compacta o arquivo.txt e gera um arquivo chamado arquivo.txt.gz

> ###### gzip -9 arquivo.txt
> Compacta o arquivo.txt com uma taxa de -9 que é a maxima do gzip e gera um arquivo chamado arquivo.txt.gz o

> ###### gunzip arquivo.txt.gz
> Descompacta o arquivo.txt.gz


* #### ZIP

> ###### zip arquivo.zip arquivo.txt
> Compacta usando o zip

> ###### zip arquivo.zip arquivo.txt aquivo2.txt arquivo3.txt
> Compacta os 3 arquivos em um unico

> ###### unzip arquivo.zip
> Descompacta o arquivo zip


* #### BZIP2

> ###### bzip2 arquivo.txt
> Compacta o arquivo usando o bzip2

> ###### bzip2 -d arquivo.bz2
> descompacta o arquivo no formato .bz2


* #### RAR

É necessario instalar (sudo apt install rar)

> ###### rar a arquivo.rar arquivo.txt
> compacta o arquivo no formato rar ("a" é o parametro de compactação)

> ###### rar x arquivo.rar
> Descompata o arquivo.rar ("x" é o parametro de descompactação)



* **ARQUIVADORES**: Junta varios arquivos em um só mas pode ser usado em conjunto ao um compactador.
* **tar**, é o principal arquivador do linux.
* 

> ###### tar -cf arquivo.txt.tar arquivo.txt arquivo2.txt arquivo3.txt
> Gera o arquivamento desses 3 arquivos.

> ###### gzip arquivos.tar
> compacta o arquivo que foi arquivado.

> ###### tar -xvf arquivo.txt.tar.gz
> descompacta/desarquiva o arquivo.

> ###### tar -xvf arquivo.txt.tar.gz -C ~/Documentos
> descompacta/desarquiva o arquivo  na pasta documentos.



### Gerenciamento de Pacotes


* **PACOTES** 
> São programas colocados dentro de um arquivo identificados por sua extensão
> Incluem arquivos necessarios para instalação de programa
> Possuem extensão .deb .rpm entre outros

* **GERENCIADORES**
> Gerenciadores de pacotes são sistemas que possuem resolução automatica de dependencias de pacotes
> Metodo facil de instalação de pacotes
> Exemplos: dpgk apt e yum



**apt**

> Gerenciador de pacotes
> sudo apt install pacote (instala)
> sudo apt upgrade pacote (atualiza)
> sudo apt remove pacote  (remove)

> ###### sudo apt update && apt upgrade 
> Atualiza o sistema

* Site para download de pacotes
> pkgs.org
> rpm.pbone.net



**dpkg**

> Instala pacotes do tipo .deb 
>
> ###### sudo dpkg -i pacote.deb

> ###### sudo dpkg -I pacote.deb
> Obtém informações do pacote

> ###### sudo dpkg -r pacote 
>
> O nome do pacote consta no comando "sudo dpkg -I pacote.deb" linha "Package"
> Remove pacote




* **FEDORA**

  

**RPM**

> rpm - gerenciador de pacotes

> ###### sudo rpm -ivh pacote.rpm
> Instala um pacote

> ###### sudo rpm -ivh --nodeps pacote.rpm
> Caso tenha um problema de dependecia no pacote usar --nodeps

> ###### rpm -U pacote.rpm
> Atualiza um pacote

> ###### rpm -e pacote.rpm
> Remove um pacote

**YUM**

> yum- gerenciador de pacotes

> ###### sudo yum install pacote
> Instala um pacote

> ###### sudo yum update pacote
> Atualiza o pacote

> ###### yum remove pacote
> Remove pacote








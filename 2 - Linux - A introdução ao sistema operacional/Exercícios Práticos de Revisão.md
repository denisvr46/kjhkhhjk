# Exercícios Práticos de Revisão



* ###  Lista 1 - Conhecendo o terminal Linux e seus atalhos



1) ###### Abra o Terminal
    crtl + alt + t
2. ###### Crie uma Pasta de nome Ubuntu dentro da Pasta Documentos
    mkdir ubuntu

3. ###### Mova esta Pasta para o diretório Pessoal
    mv ubuntu/ ~

4. ###### Crie um arquivo vazio de nome teste.txt dentro da Pasta Ubuntu
    touch teste.txt

5. ###### Renomeie este Arquivo como linux.txt
    mv teste.txt linux.txt

6. ###### Crie uma cópia deste arquivo na Pasta Downloads
    cp linux.txt /home/denis/Downloads

7. ###### Exiba todos os comandos digitados no Terminal
    history

8. ###### Execute a ajuda do comando ls
    ls --help

9. ###### Execute o manual do comando mv
    man mv

10. ###### Pare a execução do manual
    ctrl+z

11. ###### Saia do Terminal utilizando sequência de teclas
    crtl+q

12. ###### Exclua a pasta Ubuntu
    rmdir Ubuntu

13. ###### Exclua o arquivo linux.txt 
    rm linux.txt

14. ###### Limpe o terminal
    clear

15. ###### Utilize o comando para sair do terminal
    exit
    
    

* ### Lista 2 - Comandos para manipulação de arquivos e textos e redirecionamento



1. ######  Crie uma pasta de nome Exercícios e Acesse a mesma
mkdir Exercícios && cd Exercícios 

2. ######  Crie um arquivo vazio de nome lista_nomes.txt
touch lista_nomes.txt

3. ######  Abra este arquivo com o Editor Nano
nano lista_nomes.txt

4. ######  Digite 20 Nomes de Pessoas Conhecidas incluindo o seu, pulando de linha para cada nome inserido.

5. ######  Salve o arquivo

6. ######  Exiba os 10 primeiros Nomes da Lista
head lista_nomes.txt

7. ######  Exiba os 10 ultimos Nomes da Lista
tail lista_nomes.txt

8. ######  Procure no texto o seu nome
cat lista_nomes.txt | grep denis
ou
grep denis lista_nomes.txt

9. ######  Crie um Arquivo chamado setembro.txt com a saida do comando cal.
cal setembro 2020 > setembro.txt

10. ######  Adicione o conteúdo do arquivo setembro.txt ao arquivo lista_nomes.txt
cat setembro.txt >> lista_nomes.txt

11. ######  Exiba o arquivo lista_nomes.txt com paginação
less lista_nomes.txt

12. ######  Exiba o caminho do arquivos setembro.txt
find ~ -name setembro.txt
~ porque o arquivo estava na pasta home

13. ######  Exiba o tipo do arquivo lista_nomes.txt
file lista_nomes.txt

14. ######  Exiba a explicação do comando ls
whatis ls

15. ######  Renomeie o Arquivo lista_nomes.txt para arquivo.txt
mv lista_nomes.txt arquivo.txt

16. ######  Limpe o Terminal
clear

17. ######  Saia do Terminal
    exit

    

* ### Lista 3 - Diretórios do Linux e Comandos de Sistema




1) ###### Exiba todos os hardwares que existem na máquina com paginação
lshw | more

2) ###### Salve a saída do comando anterior no arquivo minhamaquina.txt
lshw | more >> minhamaquina.txt

3) ###### Exiba informações sobre a memória física e virtual na sua máquina
free

4) ###### Adicione a saída do comando anterior ao arquivo minhamaquina.txt
free >> minhamaquina.txt

5) ###### Exiba todas as placas PCI conectadas
lspci

6) ###### Adicione a saída do comando anterior ao arquivo minhamaquina.txt
lspci >> minhamaquina.txt

7) ###### Exiba todos dispositivos USB conectados
lsusb

8) ###### Adicione a saída do comando anterior ao aqrquivo minhamaquina.txt
lsusb >> minhamaquina.txt

9) ###### Exiba as informações sobre o processador
lscpu

10) ###### Adicione a saída do comando anterior ao arquivo minhamaquina.txt
lscpu >> minhamaquina.txt

11) ###### Exiba o nome do Kernel
uname

12)  ###### Adicione a saída do comando anterior ao arquivo minhamaquina.txt
uname >> minhamaquina.txt

13) ###### Exiba a versão do Kernel
uname -r

14)  ###### Adicione a saída do comando anterior ao arquivo minhamaquina.txt
uname -r >> minhamaquina.txt

15) ###### Exiba a arquitetura do Kernel
uname -m 
ou comando
arch

16) ###### Adicione a saída do comando anterior ao arquivo minhamaquina.txt
arch >> minhamaquina.txt

17) ###### Abra o arquivo minhamaquina.txt
cat minhamaquina.txt | more

18. ###### Desligue a Máquina
    reboot
    
    

* ### Lista 4 - Fundamentos de Rede e Comandos de Rede

  


1) ###### Crie um arquivo de aularedes.txt
touch aularedes.txt

2) ###### Exiba o número de IP da rede no terminal
hostname -I

3) ###### Adicione a saída do comando anterior ao arquivo aula redes.txt
hostname -I >> aularedes.txt

4) ###### Exiba o número de IP Loopback no terminal
hostname -i

5) ###### Adicione a saída do comando anterior ao arquivo aula redes.txt
hostname -i >> aularedes.txt

6) ###### Exiba Informações DNS sobre o host www.pudim.com.br
dig www.pudim.br

7) ###### Adicione a saída do comando anterior ao arquivo aula redes.txt
dig www.pudim.br >> aularedes.txt

8) ###### Exiba Informações do Usuário logado na rede
w

9) ###### Adicione a saída do comando anterior ao arquivo aula redes.txt
w >> aularedes.txt

10) ###### Execute um teste no host www.pudim.com.br com 6 pacotes
ping www.pudim.com.br -w 6

11) ###### Adicione a saída do comando anterior ao arquivo aula redes.txt
ping www.pudim.com.br -w 6 >> aularedes.txt

12) ###### Trace a Rota do seu computador até o host www.pudim.com.br
traceroute www.pudim.com.br

13) ###### Adicione a saída do comando anterior ao arquivo aula redes.txt
traceroute www.pudim.com.br >> aularedes.txt

14) ###### Exiba Informações sobre Interfaces de Rede e Endereços IP no terminal
ifconfig

15) ###### Adicione a saída do comando anterior ao arquivo aula redes.txt
ifconfig >> aularedes.txt

16) ###### Limpe o terminal
clear

17) ###### Imprima o arquivo aularedes.txt com paginação no terminal
cat aularedes.txt | more



* ### Lista 5 - Controle de usuários, grupos e permissões

  

1) ###### Crie um usuário chamado teste
sudo adduser teste

2) ###### Crie um grupo chamado grupoteste
sudo addgroup grupoteste

3) ###### Adicione o usuário teste ao grupoteste
sudo adduser teste grupoteste

4) ###### Troque a senha do usuário teste
sudo passwd teste

5) ###### Troque o usuário atual para o usuário teste
su teste

6) ###### Exiba os grupos do usuário teste
groups

7) ###### Exiba todos os usuarios do sistema
cat /etc/passwd

8) ###### Exiba todos os grupos do sistema
cat /etc/group

9) ###### Delete o usuário teste
sudo userdel -r teste

10) ###### Delete o grupo grupoteste
sudo groupdel grupoteste

11) ###### Troque para o usuario root
sudo su

12) ###### Crie um arquivo de nome teste.txt
touch teste.txt

13) ###### Edite o arquivo teste.txt com o nome desse curso
14) ###### Mude as permissões do arquivo teste.txt para 111
chmod 111 teste.txt

15) ###### Saia do usuario root para seu computador
su usuario

16) ###### Tente exibir o arquivo teste.txt no terminal
cat teste.txt

17) ###### Desligue o computador pelo terminal
shutdown -h now



* ### Lista 6 - Compactação, Descompactação e Arquivamento

  

1) ###### Crie um arquivo chamado compactar.txt
touch compactar.txt

2. ###### Edite este arquivo com os nomes dos compactadores

3) ###### Compacta este arquivo em zip
zip compactar.zip compactar.txt

4) ###### Descompacte o arquivo
unzip compactar.zip

5) ###### Compacte o arquivo com rar
rar a compactar.rar compactar.txt

6) ###### Descompacte este arquivo
rar x compactar.rar 

7) ###### Compacte este arquivo com gzip
gzip compactar.txt

8) ###### Descompacte este arquivo
gunzip compactar.txt.gz

9) ###### Compacte este arquivo com bzip2
bzip2 compactar.txt

10) ###### Descompacte este arquivo
bzip2 -d compactar.txt.bz2

11) ###### Realize o arquivamento deste arquivo com tar
tar -cf compactado.tar compactar.txt

12) ###### Compacte o arquivamento com gzip
gzip compactado.tar

13) ###### Descompacte este arquivo
tar -xvf compactado.tar.gz compactar.txt

14) ###### Remover todos arquivos do diretorio que começem com compactar
rm -r compactar*

14)  ###### Remover todos arquivos que são do formato zip
rm -r *zip

15) ###### Saia do terminal
exit

16) ###### Exiba o arquivo compactar.txt
cat compactar.txt

18. ###### Execute o comando init 0 para desligar o sistema 
    init 0

    


* ### Lista 7 - Gerenciamento de Pacotes

  

1) ###### Instale o wireshark com o gerenciador apt
sudo apt install wireshark

2) ###### Atualize o wireshark
sudo apt upgrade wireshark

3) ###### Remova o wireshark
sudo apt remove wireshark

4) ###### Atualize o sistema
sudo apt update

5) ###### Baixe e instale o pacote deb do postegresql
sudo dpkd -i postegresql.deb

6. ###### Remova o postgresql
  sudo dpkd -I postegresql (Para pegar o nome do pacote)
  sudo dpkg -r postgresql (para remover o pacote)

  


* ###### No FEDORA 

  

7) ###### Va para o Fedora
8) ###### Baixe o pacote postegresql com o gerenciador de pacotes rpm
sudo rpm -ivh --nodeps postegres.rpm

9) ###### Remova o pacote postegresql com gerenciador rpm
sudo yum postgresql

10) ###### Com o gerenciador yum instale o pacote postgresql
sudo yum install postgresql

11) ###### Remova o pacote postgresql com gerenciador yum 
sudo yum remove postgresql

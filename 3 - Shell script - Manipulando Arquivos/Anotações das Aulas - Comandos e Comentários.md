#  Shell script - Manipulando Arquivos



##### Shell Script

* **SHELL** é uma interface de usuário para acessar os seriços de um sistema
* **SCRIPT** é uma linguagem de programação que executa no sistema em tempo de execução, utilizdada para automação
* Principais linguagens, Bash e .sh

> ###### cd
> É um acronimo para change directory

> ###### cd /
> Abre o diretorio raiz do sistema

> ###### cd ~
> Abre o diretorio corrente do usuario (home)

> ###### cd..
> Volta o diretorio

> ###### cd .
> Representa o diretorio atual

> ###### ls
> É um comando de lista os arquivos

> ###### ls -l
> Lista o conteudo em coluna detalhada

> ###### ls -a
> Lista o conteudo até os arquivos ocultos

> ###### ls -s
> Lista o conteudo com tamanho alocado de cada arquivo, em bloco

> ###### cat
> É um acronimo para concatenate (concatenar)
> Cria arquivos
> Unir arquivos
> Exibe arquivos

> ###### cat arquivo1 > aquivo2
> Coloca o resultado em um outro arquivo

> ###### ">"
É um redirecionador de saida

> ###### | more
> Para parar a rolagem da tela e permitir a navegação

> ###### | less
> Para parar a rolagem da tela e permitir a navegação

> ###### touch
> Usadio para criar arquivos vazios ou alterar data e hora do arquivo

> ###### touch arquivo1.txt arquivo2.txt arquivo3.txt arquivo4.txt 
> Cria multiplos arquivos

> ###### touch -a arquivo.txt
> Muda a hora de acesso

> ###### touch -m arquivo.txt
> Muda a hora da modificação

> ###### touch -c arquivo.txt
> Muda a hora de acesso sem criar um novo arquivo

> ###### touch -t 202012081159.30 arquivo.txt
> Define a hora especifica de acesso e modificação
> CCYYMMDDhhmm.ss
> (CC-Dois primeiros digitos do ano / YY - dois digitos seguentes do ano)
> (MM - Mês / DD - Dia / hh - hora / mm - Minuto / ss- Segundo)

> ###### mv
> Move e renomeia arquivos e diretorios

> ###### -i 
> Confirme antes de substituir
> mv -i arquivo.txt diretorio

> ###### -n
> Sem substituição caso já exista no diretorio a ser enviado
> mv -n arquivo.txt diretorio

> ###### -b
> Substitui pelo backup
> mv -b arquivo.txt diretorio

> ###### -u
> Substitui o arquivo de destino 
> mv -u arquivo.txt diretorio

> ###### cp
> Permite copiar arquivos ou diretorios para outro local

> ###### cp -r /home/usuario/diretorio novodiretorio
> Copia um diretorio para outro local
> Para copiar diretorio é necessario o parametro -r

> ###### cp -r . diretorio
> Copia apenas os arquivos da pasta atual "." e move para o diretorio

> ###### -i
> Sem confirmação de existencia
> cp -i arquivo.txt /home/usuario/diretorio

> ###### -v
> Sem ela no terminal não aparece nenhuma saida
> cp -v arquivo.txt /home/usuario/diretorio

> ###### -l
> Cria hard links em vez de copiar os arquivos

> ###### -s 
> Cria links simbolicos em vez de copiar os arquivos

> ###### -u 
> Copia apenas quando o arquivo de origem for mais novo que o de destino ou quando o arquivo destino não exisir

> ###### mkdir nomediretorio
> Cria diretorios

> ###### rm arquivo.txt
> Remove arquivos

> ###### rm -f arquivo.txt
> Remove o arquivo forçadamente

> ###### find
> Procura arquivos

> ###### find ./ -type f -name "nome arquivo"
> Procura tudo que esta na pasta atual "."

> ###### find ./ -type f -name "nome*"
> Procura tudo que esta na pasta atual "." e que contem a palavra "nome" no nome do arquivo

> ###### find ./ -type f -name ".*"
> Procura tudo que é arquivo oculto na pasta

> ###### diff
> Faz a comparação entre arquivos e diretorios

> ###### diff arquivo1.txt arquivo2.txt
> Faz a comparação entre os arquivos
> Caso seja identico não mostrara nada

> ###### rmdir diretorio
> Remove diretorio vazio

> ###### rm -rf diretorio
> Remove diretorios que contem conteudo

> ###### env
> Comando que trabalha com as variaveis de ambiente
> Exibe todas variaveis de ambiente

> ###### PS1
> Prompt da linha de comandos

> ###### HOME 
Diretorio "/home" de um usuario

> ###### PATH
Lista de diretorios vasculhados quando um comando é executado

> ###### variavel=nomevariavel
> ###### export nomevariavel
> ###### $nomevariavel
> Cria uma variavel e exporta como variavel de ambiente e $ para acessar a variavel


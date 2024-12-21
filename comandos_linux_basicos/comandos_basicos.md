Listagem ( Utilizado para ver qual o conteudo dentro de uma pasta):

```
ls
```
Mostrar informações do processador:
```
lscpu
```
Mostrar informações de conexões/dispositivos usb
```
lsusb
```
Mostrar informações das linhas PCi que estão se comunicando com o seu computador:
```
lspci
```
Mostrar o disco, a estrutura do seu sistema no formato meio arvore/bloco
```
lsblk
```
_____________________________________________________________________________________________________
Manual ( Exibe manual dos comandos):
```
man 
```
```
Ex: man ls
```
_____________________________________________________________________________________________________
Ajuda (mostra resumo de um comando):
```
--help
```
```
Ex: ls --help
```
_____________________________________________________________________________________________________
Limpar (Limpa tudo que esta no terminal):
```
Clear

Ctrl + L
```
_____________________________________________________________________________________________________
Criar diretórios(pastas):
```
mkdir
```
```
Ex: mkdir minhaPasta1
```
Criando varias pastas ao mesmo tempo, apenas adicione um espaço entre os nomes :
```
Ex: mkdir minhaPasta1 minhaPasta2 minhaPasta3
```
Criar pastas com nomes compostos com espaços, utiliza-se aspas duplas ou simples:
```
Ex: mkdir "minha pasta 1"
```
_____________________________________________________________________________________________________
Acessar para dentro de diretorios(pastas):
```
cd minhaPasta1
```

Acessar diretorios com nomes compostos utilize as aspas:
```
Ex: cd "minha pasta 1"
```
Ou as barras entre as palavras e espaço:
```
Ex:cd minha\ pasta\ 1/
```
_____________________________________________________________________________________________________
Mostrar diretório ( Mostra o caminho completo da pasta que você está):
```
pwd
```
Pode-se entender também o pwd só de olhar esse comando que aparece padrão ao abrir o terminal:
```
Ex: monica@monica-Inspiron-5458:~$

monica = usuario
@ = na
monica-Inspiron-5458 = diretorio/pasta
~  = pasta principal/Home
$ = usuario tradicional 
ou
#  = usuario root
```
_____________________________________________________________________________________________________
Mostrar usuario atual: 
```
whoami
```

Pode-se inserir arquivos dentro desse usuario:
```
Ex: whoami >> curso.txt
```

Editar arquivos de textos dentro do terminal:
```
Ex: nano curso.txt
```
Abaixo no terminal terá opções do que pode fazer com esse arquivo:

```
Ex:
ctrl + x : para sair e salvar o arquivo
s : para sim
enter
```

Temos um outro comando que nos ajuda a saber o que há dentro de um arquivo sem precisar abrir a interface do nano, é o cat. 
(cat) concatena arquivos, mais para ler documentos pequenos ele funciona muito bem.

```
Ex: cat curso.txt
```
_____________________________________________________________________________________________________
Remover arquivos:
```
rm
```
```
Ex: rm curso.txt
```

Para remover diretorios (pastas):
```
rmdir
```
```
Ex: rmdir minhaPasta1
```

Remover recursivamente e forçadamente, se você tentar remover um diretorio com arquivos dentro ele não deixará com aqueles outros comandos, então precisamos forçar se temos certeza que queremos remover arquivos e pastas ao mesmo tempo.

```
rm -rf
```
Alerta: tome muito cuidado com esse comando se usar como da forma abaixo apagará todo seu disco rigido
```
rm -rf /
```
_____________________________________________________________________________________________________
Saber o nome da maquina:
```
hostname

cat /etc/hostname
```

Saber todas as interfaces de IP que tem na máquina:
```
hostname -i

hostname -I
```
_____________________________________________________________________________________________________
Saber todas as informações do IP, mac, placa de rede …:
```
ip a
```

Filtrar as saidas de informações de uma forma mais organizada:
```
grep
```
```
Ex: ip a | grep inet

Filtrando tudo que tenha inet (é onde tem as interfaces de rede)
```
Se sabe o nome da sua interface(ip a), você pode filtrar diretamente ela e trará as informações que tem dentro dela:
```
Ex:ip a | grep wlp6s0
```
_____________________________________________________________________________________________________
Verificar se está com conexão de rede. Ele responde se está conectado e com quantos milisegundos.
```
ping
```
```
Ex:ping google.com.br
```
_____________________________________________________________________________________________________
Para saber quanto de RAM / Processador meu computador está utilizando.<br>
Em gigabytes:

```
free -h
```
Em megabytes:
```
free -m
```
_____________________________________________________________________________________________________
Mostrar monitor do sistema:
```
top
```
Mostrar monitor do sistema com visual melhor:
```
htop
```
_____________________________________________________________________________________________________
Mostrar processos rodando:
```
ps
```
Mostrar lista de tudo que está rodando:
```
ps aux
```
Procurar algum processo que queremos que seja finalizado a execução:
```
Ex: ps aux | grep nome_do_arquivo
```
Uma forma resumida de ver os processos é utilizar o pgrep, que vai diretamente apenas em processos em execução:
```
Ex: pgrep nome_do_arquivo
```
Finalizando a execução de um processo:
```
kill
```
16565 é o PID do processo que será finalizado:
```
Ex: kill 16565
```
_____________________________________________________________________________________________________
Mostrar o quanto de espaço livre tem no PC:
```
df -h
```
_____________________________________________________________________________________________________
Mostrar a versão do kernel:
```
uname

uname -r
```
_____________________________________________________________________________________________________
Escanear o disco, mostrar em ordem de pastas com maior utilização e onde estão esses arquivos:
```
ncdu
```
_____________________________________________________________________________________________________
Mostrar todo o historico dos comandos no terminal:
```
history
```
_____________________________________________________________________________________________________
Modificar teclado para PT abnt2:
```
setxkbmap -model abnt2 -layout br
```
_____________________________________________________________________________________________________
<br>

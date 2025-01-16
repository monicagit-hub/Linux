# Como instalar o Wine

Para instalar o Wine, comece adicionando alguns pacotes essenciais:


```bash
sudo apt install software-properties-common apt-transport-https curl -y
```

Agora, adicione o suporte à arquitetura de 32 bits em seu sistema, com o seguinte comando no Terminal (Ctrl+Alt+T):

```bash
sudo dpkg --add-architecture i386
```

Em seguida, adicione o repositório dos desenvolvedores, começando pelas chaves de acesso:

```bash
sudo mkdir -pm755 /etc/apt/keyrings
```

Depois:

```bash
sudo wget -O /etc/apt/keyrings/winehq-archive.key https://dl.winehq.org/wine-builds/winehq.key
```

Agora, instale o repositório do WineHQ:

```bash
sudo wget -NP /etc/apt/sources.list.d/ https://dl.winehq.org/wine-builds/ubuntu/dists/lunar/winehq-lunar.sources
```

Atualize a biblioteca de aplicativos:

```bash
sudo apt update
```

E instale o Wine (aqui indicado, por segurança, a versão estável):

```bash
sudo apt install --install-recommends winehq-stable winetricks
```



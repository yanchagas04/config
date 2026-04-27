#  Guia de Configuração ⚙️

Esse guia serve para eu ter acesso fácil aos comandos que precisarei executar caso precise reinstalar o sistema novamente. Como uso o CachyOS como distro Linux, preciso fazer tudo levando em conta o gerenciador de pacotes **PACMAN**

## 1. Configuração do CachyOS 🐧

### Instação dos aplicativos

Para instalar todos os softwares que eu uso:
- Visual Studio Code (OSS)
- Discord
- Steam
- Solaar (controlar dispositivos Logitech)
- LACT (controle da GPU)
- Gerenciador de Discos (utilizo o do Gnome)

```
    sudo pacman -S code
    sudo pacman -S discord
    sudo pacman -S steam
    sudo pacman -S solaar
    sudo pacman -S lact
    sudo pacman -S gnome-disk-utility
```

## 2. Configurações do Niri e Noctalia 🌙🦉

### 2.1. Niri

O Niri é um *tiling window manager* muito brabo, porém as configurações só podem ser feitas através dos arquivos de configuração. Por isso, o diretório de configuração `/niri` está aqui nesse repositório.

### 2.2. Noctalia

Além disso, é preciso configurar o Noctalia, que é o *shell* que roda por cima do Niri. Isso tudo é feito via interface gráfica, mas ele gera um JSON muito brabo que também tá aqui como `noctalia.json`.

## 3. Favoritos do Navegador

Também coloquei aqui no repositório um arquivo contendo meus favoritos salvos para poder pegar a qualquer momento e importar em um navegador.

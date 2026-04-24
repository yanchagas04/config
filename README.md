#  Guia de Configuração ⚙️

Esse guia serve para eu ter acesso fácil aos comandos que precisarei executar caso precise reinstalar o sistema novamente. Como uso o Fedora como distro Linux, preciso fazer tudo levando em conta o gerenciador de pacotes **RPM**

## 1. Configuração do Fedora 🐧

### 1.1. Habilitar repositórios

Para permitir a instalação de outros aplicativos, os repositórios Free e Non-Free precisam ser inseridos. Além disso, o repositório de outras ferramentas que utilizo também precisam ser inseridos para poder fazer a instalação

```
    sudo dnf install https://mirrors.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm https://mirrors.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm
    sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
    sudo dnf copr enable scottames/ghostty
    sudo dnf copr enable xxmitsu/mesa-git
    sudo dnf copr enable ilyaz/LACT
```

**OBS:** Para pesquisar por repositórios COPR, entre em no site do [**Fedora Copr**](https://copr.fedorainfracloud.org/coprs/)

### 1.2. Instação dos aplicativos

Para instalar todos os softwares que eu uso:
- Visual Studio Code
- Discord
- Steam
- Solaar (controlar dispositivos Logitech)
- Ghostty (emulador de terminal)
- LACT (controle da GPU)

```
    sudo dnf install code
    sudo dnf install discord
    sudo dnf install steam
    sudo dnf install ghostty
    sudo dnf install solaar
    sudo dnf install lact
```

## 2. Configuração do Terminal (Ghostty) 👻

### 2.1. Aplicando tema

Só aplico um tema que eu gosto, o restante das configurações já me satisfaz

    theme = Dark+

### 2.2. Busca de outros temas

Para ver os outros temas que existem

    ghostty +list-themes

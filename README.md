# Guia de Configuração ⚙️

Esse guia serve para eu ter acesso fácil aos comandos que precisarei executar caso precise reinstalar o sistema novamente.

# Windows 🪟

## Instação do Windows

Para realizar um _Debloat_ no sistema, a instalação é feita com um arquivo de configuração para remover aplicativos que a microsoft enfia no rabo do usuário. Além disso, também são feitas algumas pré-configurações para deixar o Windows do jeito que gosto de utilizar, como:

- Remover os pins do menu iniciar
- Remover os ícones da barra de tarefa
- Remover os widgets
- Criação automática de conta
- Utilização do menu de contexto antigo

Tudo isso está no `autounattend.xml`, que é o arquivo de configuração de instalação do Windows

## Instalação de Aplicativos

Para instalação facilitada, uso o [**Winget**](https://winget.run/), que é o gerenciador de pacotes do Windows. Pra quem está acostumado com a facilidade de instalar pacotes no ambiente Linux, é uma ferramenta extremamente necessária e poderosa.

- Fiz um bat com os comandos para instalar tudo, cujo conteúdo também pode ser copiado aqui:

  ```bat
  @REM Drivers e Utilitários
  winget install Wacom.WacomTabletDriver
  winget install 7zip.7zip
  winget install Logitech.GHUB
  winget install Logitech.OptionsPlus
  winget install OBSProject.OBSStudio
  winget install Discord.Discord
  winget install Hibbiki.Chromium
  winget install Blip
  winget install shinchiro.mpv
  winget instal GameSir.GameSirConnect
  winget instal Asus.ArmouryCrate

  @REM Softwares e Linguagens de Programação
  winget install Microsoft.PowerShell
  winget install Git.Git
  winget install Github.cli
  winget install Microsoft.VisualStudioCode
  winget install Golang.Go
  winget install Python.Python.3.12
  winget install Python.Python
  winget install Postman.Postman
  winget install Insomnia.Insomnia
  winget install Docker.DockerCLI

  @REM Jogos
  winget install EpicGames.EpicGamesLauncher
  winget install Valve.Steam
  ```

## Drivers de Vídeo e Configuração do Adrenalin

Drivers disponíveis na [página de suporte da AMD](https://www.amd.com/pt/support/download/drivers.html)

- Para configurar a GPU, importamos o perfil salvo em `amd-adrenalin-profile.xml`

## Configuração do Git e credenciais do GitHub

Com as novas ferramentas de CLI do GitHub, esse processo ficou extremamente fácil, primeiro configuramos o Git, para assim podermos autenticar nossa conta do GitHub.

- Para configurarmos o usuário do Git, rodamos os seguinte comandos

  ```bash
  git config --global user.name "Seu nome"
  git config --global user.email seuemail@mail.com
  ```

- Já para se autenticar, usaremos o GitHub CLI

  ```bash
  gh auth login
  ```

  **\*OBS**: Esse comando permite que você realize a autenticação direto pelo navegador no qual posusi sua conta do GitHub logada.\*

## Configuração do VSCode

Para aplicar minhas configurações de VSCode basta importar o perfil `vscode-profile.code-profile`

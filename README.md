# Useful-Software
Useful software a programmer must have. Some of them includes how-to-install steps.

# Windows

## 1. Visual Studio Code
Download: https://code.visualstudio.com/
### Themes.
    Favorite:
    Name: Monokai Pro
    Id: monokai.theme-monokai-pro-vscode
    Description: ✨ Professional dark & light theme + icon pack, from the author of the original Monokai color scheme.
    Version: 2.0.2
    Publisher: monokai
    VS Marketplace Link: https://marketplace.visualstudio.com/items?itemName=monokai.theme-monokai-pro-vscode

    Name: Atom One Dark Theme
    Id: akamud.vscode-theme-onedark
    Description: One Dark Theme based on Atom
    Version: 2.3.0
    Publisher: Mahmoud Ali
    VS Marketplace Link: https://marketplace.visualstudio.com/items?itemName=akamud.vscode-theme-onedark

### Icons Theme.
    Name: Material Icon Theme
    Id: PKief.material-icon-theme
    Description: Material Design Icons for Visual Studio Code
    Version: 5.14.1
    Publisher: Philipp Kief
    VS Marketplace Link: https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme

### Extensions.
Name: Live Server
    Id: ritwickdey.LiveServer
    Description: Launch a development local Server with live reload feature for static & dynamic pages
    Version: 5.7.9
    Publisher: Ritwick Dey
VS Marketplace Link: https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer

    Name: HTML CSS Support
    Id: ecmel.vscode-html-css
    Description: CSS Intellisense for HTML
    Version: 2.0.11
    Publisher: ecmel
VS Marketplace Link: https://marketplace.visualstudio.com/items?itemName=ecmel.vscode-html-css

    Name: Prettier - Code formatter
    Id: esbenp.prettier-vscode
    Description: Code formatter using prettier
    Version: 11.0.0
    Publisher: Prettier
VS Marketplace Link: https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode

    Name: WSL
    Id: ms-vscode-remote.remote-wsl
    Description: Open any folder in the Windows Subsystem for Linux (WSL) and take advantage of Visual Studio Code's full feature set.
    Version: 0.88.5
    Publisher: Microsoft
VS Marketplace Link: https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-wsl

## 2. Chrome
Download: https://www.google.com/intl/en_uk/chrome/
### Extensions.
    Name: Colour Picker Tool - Geco.
    Description: Grab colours from web pages, colour picker, colour history.
    Version: 1.0.10
    Publisher: geco-picker.com
Chrome Extension Link: https://chromewebstore.google.com/detail/colour-picker-tool-geco/eokjikchkppnkdipbiggnmlkahcdkikp

    Name: Grammarly: AI Writing and Grammar Checker App
    Description: Improve your writing with all-in-one assistance—including generative AI, grammar check, and more.
    Version: 14.1209.0
    Publisher: grammarly.com
Chrome Extension Link: https://chromewebstore.google.com/detail/grammarly-ai-writing-and/kbfnbcaeplbcioakkpcpgfkobkghlhen

    Name: Sound Booster - increase volume up
    Description: Sound Booster helps boost volume video or music on any tab! Increase volume and bass booster, equalizer. Volume control.
    Version: 1.0.9
    Publisher: sound-ultimate.com
Chrome Extension Link: https://chromewebstore.google.com/detail/sound-booster-increase-vo/nmigaijibiabddkkmjhlehchpmgbokfj

## 3. WSL
**You must be running Windows 10 version 2004 and higher (Build 19041 and higher) or Windows 11**
    
    How to install? 
    Open terminal (Windows + R > type "cmd", press enter)
    Write "wsl --install"
    This command will enable the features necessary to run WSL.
    If you get "WslRegisterDistribution failed with error: 0x80370102" error, you must enable Virtual Machine Platform in BIOS.
    
More details here: https://learn.microsoft.com/en-us/windows/wsl/install

**Must have:** 
    
    Windows Subsystem for Linux (https://www.microsoft.com/store/productId/9P9TQF7MRM4R?ocid=pdpshare)
    Ubuntu (https://www.microsoft.com/store/productId/9PDXGNCFSCZV?ocid=pdpshare)

## 4. Git
Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

Downloads

    Windows x32
    https://github.com/git-for-windows/git/releases/download/v2.47.1.windows.1/Git-2.47.1-32-bit.exe

    Windows x64
    https://github.com/git-for-windows/git/releases/download/v2.47.1.windows.1/Git-2.47.1-64-bit.exe

More details: https://git-scm.com/

## 5. Windows Terminal
The Windows Terminal is a modern, fast, efficient, powerful, and productive terminal application for users of command-line tools and shells like Command Prompt, PowerShell, and WSL. Its main features include multiple tabs, panes, Unicode and UTF-8 character support, a GPU accelerated text rendering engine, and custom themes, styles, and configurations.

    Download: https://www.microsoft.com/store/productId/9N0DX20HK701?ocid=pdpshare

## 6. Discord.
Discord is great for playing games and chilling with friends, or even building a worldwide community. Customise your own space to talk, play, and hang out.

    Download: https://discord.com/

# Linux / WSL
## 1. Zsh
Zsh is a shell designed for interactive use, although it is also a powerful scripting language.
Install: 

    1. sudo apt install zsh
    2. zsh --version
    3. chsh -s $(which zsh) OR sudo lchsh $USER (FEDORA)
        Note that this will not work if Zsh is not in your authorized shells list (/etc/shells) or if you don't have permission to use chsh. If that's the case you'll need to use a different procedure.
        If you use lchsh you need to type /bin/zsh to make it your default shell.
    4. Log out and log back in again to use your new default shell.
    5. Test that it worked with echo $SHELL. Expected result: /bin/zsh or similar.
        If nothing happens, type "logout" and login again. This time, when you open the terminal, terminal will open zsh setup. Continue as desired.
    6. Test with $SHELL --version. Expected result: 'zsh 5.8' or similar

## 2. OhMyZsh
Oh My Zsh is an open source, community-driven framework for managing your zsh configuration.
### Prerequisites:
1. Zsh should be installed (v4.3.9 or more recent is fine but we prefer 5.0.8 and newer). If not pre-installed (run zsh --version to confirm), check the following wiki instructions here: Installing ZSH
2. curl or wget should be installed
3. git should be installed (recommended v2.4.11 or higher)

### Basic Installation.
Oh My Zsh is installed by running one of the following commands in your terminal. You can install this via the command-line with either *curl*, wget or another similar tool.

curl
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

wget
```
sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

fetch
```
sh -c "$(fetch -o - https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### Using Oh My Zsh
### Plugins
Oh My Zsh comes with a shitload of plugins for you to take advantage of. You can take a look in the plugins directory and/or the wiki to see what's currently available.

### Enabling Plugins
Once you spot a plugin (or several) that you'd like to use with Oh My Zsh, you'll need to enable them in the .zshrc file. You'll find the zshrc file in your $HOME directory. Open it with your favorite text editor and you'll see a spot to list all the plugins you want to load.
```
vi ~/.zshrc
```
For example, this might begin to look like this:
```
plugins=(
  git
  bundler
  dotenv
  macos
  rake
  rbenv
  ruby
)
```
### Must have Plugins
```git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions```
```git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting```

Edit .zshrc to include plugins plugins=(git zsh-autosuggestions zsh-syntax-highlighting)
``` nano .zshrc```

More details about Oh My Zsh (Themes, plugins, etc): https://github.com/ohmyzsh/ohmyzsh?tab=readme-ov-file#using-oh-my-zsh

### Preferred Theme:
jonathan
Installing theme: 
```
nano .zshrc
```
manually replace **ZSH_THEME="robbyrussell"** with desired theme. In our case, it will be jonathan. Output: ZSH_THEME="jonathan"
```CTRL+X, Y, Enter```

Relog to apply all changes.

## Nerd Fonts.
https://github.com/ryanoasis/nerd-fonts/tree/master/patched-fonts/FiraMono
Select desired. 
In my case it's Regular > Download **FiraMonoNerdFont-Regular.otf**
Open it, and install it. 

## Powerlevel10k

```git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k```

    nano .zshrc
    change ZSH_Theme="jonathan" to ZSH_Theme="powerlevel10k/powerlevel10k"
    CTRL+X, Y, Enter
    relog & follow the setup.
    Personal Prefferences: ynn311132234421n1y (Will make sense when running setup)
    relog.


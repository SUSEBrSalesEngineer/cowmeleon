# Título

## Instalação
Instalação do [ZSH](https://www.zsh.org/) e do Fuzzy Finder (necessário para utilização do plugin fzf)
```bash
sudo zypper install zsh fzf
```

Instalação do [Oh My ZSH](https://ohmyz.sh/)
```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Instalação dos plugins custom
```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting

git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

## Configuração
Ativação dos plugins
```bash
omz plugin enable zsh-autosuggestions zsh-syntax-highlighting suse fzf common-aliases extract
```

Listando os temas
```bash
omz theme list
```

Alterando o tema
```bash 
omz theme set random
```

Todas as instalações de configurações e temas ficam no diretório `~/.oh-my-zsh`.

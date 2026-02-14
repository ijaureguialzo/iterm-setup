# iTerm setup

Configuración personalizada de [iTerm](https://iterm2.com/) con [Oh My Zsh](https://ohmyz.sh/).

## Instalación

1. Instalar las [Command Line Tools](https://developer.apple.com/documentation/xcode/installing-the-command-line-tools)
   de Xcode:

    ```shell
    xcode-select --install
    ```

2. Instalar [iTerm](https://iterm2.com/).
3. Instalar [Oh My Zsh](https://ohmyz.sh/).

    ```shell
    sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
    ```

4. Instalar el tema [Powerlevel10k](https://github.com/romkatv/powerlevel10k)

    ```shell
    git clone --depth=1 https://github.com/romkatv/powerlevel10k.git "${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k"
    ```

5. Desactivar el mensaje de último login:

    ```shell
    touch ~/.hushlogin
    ```

6. Reemplazar el fichero `~/.zshrc` por el [personalizado](./zshrc).
7. Importar la [configuración de iTerm](./configuracion.itermexport).
8. Instalar la fuente [Meslo Nerd Font](./fonts) parcheada para Powerlevel10k.

## Notas

Actualizar Powerlevel10k:

```shell
git -C "${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k" pull
```

## Referencias

- [iTerm2](https://iterm2.com/)
- [Oh My Zsh](https://ohmyz.sh/)
- [Powerlevel10k](https://github.com/romkatv/powerlevel10k)
- [iTerm2 Material Design](https://github.com/MartinSeeler/iterm2-material-design)

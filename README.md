# dotfiles / Config Files

> Config files for applications and services I use,

- alacritty
- powerlevel10k

## Other Tips

### Powershell

1. Set Alias
    ```powershell
    Set-Alias -Name wsl2 -Value C:\Windows\system32\wsl.exe
    ```

### alacritty

1. Config location
    - Windows
        ```powershell
        %APPDATA%\alacritty\alacritty.toml
        ```
    - Other Locations
        ```bash
        $XDG_CONFIG_HOME/alacritty/alacritty.toml
        ```

        ```bash
        $XDG_CONFIG_HOME/alacritty.toml
        ```

        ```bash
        $HOME/.config/alacritty/alacritty.toml
        ```

        ```bash
        $HOME/.alacritty.toml
        ```

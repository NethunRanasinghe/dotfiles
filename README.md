# dotfiles / Config Files

> Config files for applications and services I use,

- alacritty
- powerlevel10k

## Other Tips

### Powershell

1. Set Alias

    - Temporary
        ```powershell
        Set-Alias -Name wsl2 -Value C:\Windows\system32\wsl.exe
        ```
    
    - Permenant
        1. Check if you have a profile script
            ```powershell
            Test-Path $profile
            ```
            
        1. Create a profile script (if necessary/if above returns 'false')
            ```powershell
            New-Item -Path $profile -ItemType File -Force
            ```

        1. Edit the profile
            ```powershell
            Set-Alias -Name YourAlias -Value CommandToRun
            ```

        1. Reload the profile
            ```powershell
            . $profile
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

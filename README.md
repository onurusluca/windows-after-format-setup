# My Windows 10/11 After Format Setup and Settings

- Mouse sensitivity settings
- Updates, restart
- Change to dark mode
- Customization, wallpaper etc.
- Remove unnecessary apps
- Add browser
- Night light setting
- Scaling and font size
- Power mode
- Clean after format files
- Disable all options on privacy
- Show file extensions and hidden files
- Clean startup menu
- Restart
- Update from store
- Add Windows PowerToys
- Install GPU Drivers
- Browser settings are automatic

## Development Environment

### Windows Terminal

- Set WT as default
- Download ohmyposh from Microsoft Store
- Add MesloLGM NF font
- New-Item -Path $PROFILE -Type File -Force
- notepad $PROFILE
- Add: `oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH/spaceship.omp.json" | Invoke-Expression [NetServicePointManager]::SecurityProtocol = [NetServicePointManager]::SecurityProtocol -bor [NetSecurityProtocolType]::Tls12`
- If below error then open PowerShell as admin and run this code: `Set-ExecutionPolicy RemoteSigned`
    > cannot be loaded because running scripts is disabled on this system

- User WSL: <https://www.groovypost.com/howto/install-windows-subsystem-for-linux-in-windows-11/>
- Add Vscode, sign in settings are automatic
- <https://nodejs.org/en/> restart, node -v, npm -v if problem: add env variables path+ C:\Program Files\nodejs
- npm install -g pnpm
- Install GIT <https://git-scm.com/> add to path C:\Program Files\Git\cmd C:\Program Files\Git\bin
- Enter identity info:
  - git config --global user.email 'email'
  - git config --global user.name 'username'

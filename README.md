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
- Install Explorer Patcher

## Development Environment

- User WSL: <https://www.groovypost.com/howto/install-windows-subsystem-for-linux-in-windows-11/>
- Add Vscode, sign in settings are automatic
- <https://nodejs.org/en/> restart, node -v, npm -v if problem: add env variables path+ C:\Program Files\nodejs
- npm install -g pnpm
- Install GIT <https://git-scm.com/> add to path C:\Program Files\Git\cmd C:\Program Files\Git\bin
- Enter identity info:
  - git config --global user.email 'email'
  - git config --global user.name 'username'

### Windows Terminal

- Set WT as default
- Download ohmyposh from Microsoft Store
- Add MesloLGM NF font
- New-Item -Path $PROFILE -Type File -Force
- notepad $PROFILE
- Add: `oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH/spaceship.omp.json" | Invoke-Expression [NetServicePointManager]::SecurityProtocol = [NetServicePointManager]::SecurityProtocol -bor [NetSecurityProtocolType]::Tls12`
- If below error then open PowerShell as admin and run this code: `Set-ExecutionPolicy RemoteSigned`
    > cannot be loaded because running scripts is disabled on this system

**Windows Terminal Settings:**

    {
      "$help": "https://aka.ms/terminal-documentation",
      "$schema": "https://aka.ms/terminal-profiles-schema",
      "actions": [
        {
          "command": "find",
          "keys": "ctrl+shift+f"
        },
        {
          "command": "paste",
          "keys": "ctrl+v"
        },
        {
          "command": {
            "action": "copy",
            "singleLine": false
          },
          "keys": "ctrl+c"
        },
        {
          "command": {
            "action": "splitPane",
            "split": "auto",
            "splitMode": "duplicate"
          },
          "keys": "alt+shift+d"
        }
      ],
      "alwaysOnTop": false,
      "copyFormatting": "none",
      "copyOnSelect": false,
      "defaultProfile": "{61c54bbd-c2c6-5271-96e7-009a87ff44bf}",
      "profiles": {
        "defaults": {
          "backgroundImage": "ms-appdata:///roaming/cool-bg.gif",
          "backgroundImageOpacity": 0.20000000000000001,
          "backgroundImageAlignment": "bottomRight",
          "backgroundImageStretchMode": "none",
          "font": {
            "face": "MesloLGM NF",
            "size": 10
          },
          "opacity": 80,
          "useAcrylic": true
        },
        "list": [
          {
            "commandline": "%SystemRoot%\\System32\\WindowsPowerShell\\v1.0\\powershell.exe",
            "guid": "{61c54bbd-c2c6-5271-96e7-009a87ff44bf}",
            "hidden": false,
            "name": "Windows PowerShell"
          },
          {
            "commandline": "%SystemRoot%\\System32\\cmd.exe",
            "guid": "{0caa0dad-35be-5f56-a8ff-afceeeaa6101}",
            "hidden": false,
            "name": "Command Prompt"
          },
          {
            "guid": "{2c4de342-38b7-51cf-b940-2309a097f518}",
            "hidden": false,
            "name": "Ubuntu",
            "source": "Windows.Terminal.Wsl"
          },
          {
            "guid": "{b453ae62-4e3d-5e58-b989-0a998ec441b8}",
            "hidden": false,
            "name": "Azure Cloud Shell",
            "source": "Windows.Terminal.Azure"
          }
        ]
      },
      "schemes": [
        {
          "background": "#282C34",
          "black": "#282C34",
          "blue": "#61AFEF",
          "brightBlack": "#5A6374",
          "brightBlue": "#61AFEF",
          "brightCyan": "#56B6C2",
          "brightGreen": "#98C379",
          "brightPurple": "#C678DD",
          "brightRed": "#E06C75",
          "brightWhite": "#DCDFE4",
          "brightYellow": "#E5C07B",
          "cursorColor": "#FFFFFF",
          "cyan": "#56B6C2",
          "foreground": "#DCDFE4",
          "green": "#98C379",
          "name": "One Half Dark",
          "purple": "#C678DD",
          "red": "#E06C75",
          "selectionBackground": "#FFFFFF",
          "white": "#DCDFE4",
          "yellow": "#E5C07B"
        },
      ],
      "useAcrylicInTabRow": true
    }

<body>
    <div align="left">
        <h1 align="left">🍨 Scoopet 🍨</h1>
        <p>
            <a>
                <img
                    src="https://img.shields.io/github/workflow/status/Ovler-Young/Personal-scoop/Excavator.svg"
                />
            </a>
            <a>
                <img
                    src="https://img.shields.io/github/languages/code-size/Ovler-Young/Personal-scoop.svg"
                />
            </a>
            <a>
                <img
                    src="https://img.shields.io/github/repo-size/Ovler-Young/Personal-scoop.svg"
                />
            </a>
            <a>
                <img
                    src="https://img.shields.io/github/license/Ovler-Young/Personal-scoop"
                />
            </a>
        </p>
    </div>
    <p></p>
    <div>
        <p>
            A Bucket for the Best Windows Package Manager
            <a href="https://github.com/ScoopInstaller/Scoop"> Scoop </a>:
            For my personal use.
        </p>
        <p align="left">
            <a href="README.md">English</a> |
            <a href="README_CN.md">简体中文</a>
        </p>
    </div>
</body>

For ones familiar with Scoop:

```powershell
scoop bucket add scoopet https://github.com/Ovler-Young/Personal-scoop
```

# :running: To Start

## :bike: Install Scoop

### :computer: Step 1: Enable remote policy in PowerShell

```powershell
Set-ExecutionPolicy RemoteSigned -scope CurrentUser
```

### :gear: Step 2: Customize your Scoop directory

```powershell
$env:SCOOP='Your_Scoop_Path'
[Environment]::SetEnvironmentVariable('SCOOP', $env:SCOOP, 'User')
```

> If you skip this step, all user installed Apps and Scoop itself will live in `c:/users/user_name/scoop`.

### :hammer: Step 3: Download and install Scoop

```powershell
Invoke-Expression (New-Object System.Net.WebClient).DownloadString('https://get.scoop.sh')
```

### :book: Step 4: Glance at quick-start by `scoop help`

For more information, please visit Scoop official site at 👉 https://scoop.sh/ 👈

## :car: Install Apps from this bucket

### :train: Step 1: Install Aria2 to accelerate downloading

```powershell
scoop install aria2
```

### :ticket: Step 2: Install Git to add new repositories

```powershell
scoop install git
```

if you are using VPN, you need to turn off aria2 before installing Apps

```powershell
scoop config aria2-enabled false
```

### :airplane: Step 3: Add this wonderful bucket and update, mo-mo-da~ :kiss:

```powershell
scoop bucket add scoopet https://github.com/Ovler-Young/Personal-scoop
scoop update
```

### :rocket: Step 4: Install Apps

- Check the exact name of App by `scoop search`

```powershell
scoop search <app_name>
```

- Install Apps with assistance of plugin `scoop-completion`

```powershell
scoop install scoop-completion
scoop install <app_name>
```

> to use `scoop-completion`, just to hit `tab` after initial letters of App names

### :100: Step 5: List the official recommended buckets by `scoop bucket known`

```powershell
scoop bucket known

main [default]
extras [strongly recommended]
versions
nightlies
nirsoft
php
nerd-fonts
nonportable
java
games
jetbrains
```

## :m: Trivial

### Tweak with Parameters in Aria2

```powershell
scoop config aria2-enabled true
scoop config aria2-retry-wait 4
scoop config aria2-split 16
scoop config aria2-max-connection-per-server 16
scoop config aria2-min-split-size 4M
```

## :star: Summary

### Research Tools

|          App          | Auto-Update ? | Original ?                                                          |
| :-------------------: | :-----------: | ------------------------------------------------------------------- |
|    TBD     |       ×       | ×                                                                   |

### Development Auxillary

|                  App                  | Auto-Update ? | Original ?                                                               |
| :-----------------------------------: | :-----------: | ------------------------------------------------------------------------ |
|    TBD     |       ×       | ×                                                                   |

### Daily Work

|       App        | Auto-Update ? | Original ?                                                |
| :--------------: | :-----------: | --------------------------------------------------------- |
|    TBD     |       ×       | ×                                                                   |

### Social & Entertainment

|      App      | Auto-Update ? | Original ?                                                |
| :-----------: | :-----------: | --------------------------------------------------------- |
|    TBD     |       ×       | ×                                                                   |

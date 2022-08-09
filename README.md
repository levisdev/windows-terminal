# This is my windows terminal settings

## How to setup???

1. Backup your settings.
2. Open PowerShell as Administrator.
3. Delete existing settings directory
   ```ps1
   Remove-Item -Path $Env:LocalAppData\Packages\Microsoft.WindowsTerminal_8wekyb3d8bbwe\LocalState -Force –Recurse
   ```
4. Clone this repo:
   ```bash
   git clone https://github.com/levisdev/windows-terminal.git
   ```
5. Create symlink to default directory:
   ```ps1
   New-Item -ItemType SymbolicLink -Path "$Env:LocalAppData\Packages\Microsoft.WindowsTerminal_8wekyb3d8bbwe\LocalState" -Target "path\to\this\repo"
   ```
6. Enjoy! :))

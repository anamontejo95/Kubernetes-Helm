En mi caso la instalación de Helm la haré en Windows10, por ello antes de instalarlo voy a instalar la herramienta Chocolatey.

## Instalar Chocolatey  
Primero tenemos que comprobar la política de ejecución (por defecto suele ser restricted) y poner AllSigned.  
Get-ExecutionPolicy  
Set-ExecutionPolicy AllSigned
A continuación, con el siguiente comando instalamos Chocolatey:  
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))

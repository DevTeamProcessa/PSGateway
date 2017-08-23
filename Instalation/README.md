# Instalación de PSGateway

## Requisitos del sistema


* Sistemas operativos soportados
- Windows Server 2008 R2 SP1, 2012 y 2012 R2
- Windows 7 SP1, 8.1 y 10
* PowerShell versión 5 o superior (puede instalar [Windows Management Framework 5.1](https://www.microsoft.com/en-us/download/details.aspx?id=54616) para obtener PowerShell 5)
* Microsoft .NET Framework
- WMF 5.1 requiere Microsoft .NET Framework 4.5 o superior. Puede instalar Microsoft .NET Framework 4.5 o superior siguiendo las instrucciones [aquí](https://docs.microsoft.com/en-us/dotnet/framework/install/guide-for-developers).

## Instalando PSGateway

1. Abra una ventana de PowerShell como usuario administrador y registre el repositorio de Nuget de Gerencia Técnica.
```powershell
Register-PSRepository -Name 'Processa GT' -SourceLocation 'http://proget:8020/nuget/PowerShell' -InstallationPolicy Trusted
```

2. Instale el módulo desde el Repositorio
```powershell
Install-Module -Name 'PSGateway' -Repository 'Processa GT'
```

## Actualizando PSGateway

Si el módulo ya está instalado solo tiene que actualizarlo. 

1. Asegurese de tener registrado el repositorio de Nuget de Gerencia Técnica.
```powershell
Get-PSRepository -Name 'Processa GT'
```

2. Actualice el módulo desde el Repositorio
```powershell
Update-Module -Name 'PSProcessa' -Force

## Desinstalando PSGateway

1. Abra una ventana de PowerShell como usuario administrador

2. Ejecute el comando
```
Uninstall-Module PSProcessa
```
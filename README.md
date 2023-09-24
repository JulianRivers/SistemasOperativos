# SistemasOperativos

## WinRE

Sistema de recuperación de windows

### Configuración de inicio

esto es lo que hace el SO al iniciar el encendido

- **Fase 1:** Carga del firmware debe existir un MBR (Master boot record) y debe ser valido
- **Fase 2**: Administrador de arranque de windows WBM windows boot manager  el archivo que se encarga de esto es `C:\Windows\Boot\EFI\bootmgfw.efi`
  ![elegir-so](capturas/elegir-so.png)
- **Fase 3:** Carga del archivo WinLoad.exe: ubicación `C:\Windows\System32\winload.exe`
  - **funciones:** cargar el software de MS, los controladores principales y el kernel de windows
- **Fase 4:** Gestión del sistema: carga interfaz de usuario y el resto de software

## Configuración de arranque de windows

se puede ver con el comando `BCDEdit`
![BCDEdit](capturas/BCDedit.png)

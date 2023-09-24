# Sistema de recuperación de windows

## Configuración de inicio

esto es lo que hace el SO al iniciar el encendido

- **Fase 1:** Carga del firmware debe existir un MBR (Master boot record) y debe ser valido
- **Fase 2**: Administrador de arranque de windows WBM windows boot manager  el archivo que se encarga de esto es `C:\Windows\Boot\EFI\bootmgfw.efi`
  ![elegir-so](/capturas/winRE/elegir-so.png)
- **Fase 3:** Carga del archivo WinLoad.exe: ubicación `C:\Windows\System32\winload.exe`
  - **funciones:** cargar el software de MS, los controladores principales y el kernel de windows
- **Fase 4:** Gestión del sistema: carga interfaz de usuario y el resto de software

## Configuración de arranque de windows

se puede ver con el comando `BCDEdit`
![BCDEdit](/capturas/winRE/BCDedit.png)

## WinRE

(Entorno de Recuperación de Windows)Proporciona opciones de recuperación en caso de que el sistema operativo tenga problemas o no se inicie correctamente.

WinRE inicia automáticamente cuando:

▷ Dos intentos fallidos de iniciar Windows.

▷ Dos apagados inesperados consecutivos que ocurren dentro de los dos minutos posteriores a la finalización del arranque.

▷ Dos reinicios consecutivos del sistema dentro de los dos minutos posteriores a la finalización del arranque.

▷ Un error de Secure Boot (salvo algún problema relacionado con Windows Boot Manager)

▷ Un error de BitLocker en dispositivos táctiles.

### Consideraciones de seguridad WinRE

▷ Si los usuarios abren el menú de las opciones de arranque desde Windows y seleccionan la herramienta WinRE, ellos deben proveer el nombre de usuario y contraseña de una cuenta local con privilegios de administrador.

▷ De manera predeterminada, la red esta deshabilitada en WinRE.

En el administrador de discos se puede ver el espacio designado para este sistema:

![espacio designado para winRE](/capturas/winRE/partición-recuperación.png)

## Verificar el estado del WinRE

![estado-winRE](/capturas/winRE/winRE.png)

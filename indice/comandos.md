# comandos

## Administración

`resmon` - monitor de recursos

`perfmon` - monitor de rendimiento

`regedit` - editor de registro(ver clave de producto)

`dxdiag` - recopila información detallada sobre hardware y software

`taskmgr` - administrador de tareas

`diskmgmt.msc` - administrador de discos

`control` - panel de control

`services.msc` - servicios

`taskschd.msc` - programador de tareas

## winRE

`reagentc/info` - Verificar estado de winRE

`BCDEdit` - para ver info del administrador de arranque de windows y el cargador de arranque

## Para saber información del sistema

`systeminfo` Esta herramienta muestra información de configuración del sistema
    operativo de un equipo local o remoto, incluidos los niveles de
    Service Pack.

`msinfo32` muestra información detallas del sistema, en hardware y software

## Formas de filtrar información

`comando | more` - Esto mostrará las primeras 10 líneas y luego te permitirá avanzar página por página o presionar "Q" para salir.

`find` y `findstr`: Estos comandos se utilizan para buscar cadenas de texto en la salida de otro comando. Puedes usarlos para filtrar la información que contiene ciertas palabras clave o patrones. Por ejemplo, para buscar "error" en la salida de un comando:

```bash
comando | find "error"
comando | findstr "patron"
```

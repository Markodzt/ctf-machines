# MF0486 - Examen Práctico

Este documento resume los retos y soluciones del examen práctico correspondiente a la máquina MF0486.

## Descripción general

El objetivo de esta máquina fue realizar un test de penetración completo, abarcando las fases de enumeración, explotación y escalada de privilegios.

### Descripción del proyecto

El proyecto me ha parecido muy interesante y didáctico. Permite aplicar una amplia variedad de técnicas de pentesting en un entorno simulado realista. Además, combina aspectos técnicos con análisis forense y de comportamiento del sistema, lo cual añade valor desde una perspectiva profesional.

### Parte más compleja

La parte más compleja fue identificar la ubicación del archivo malicioso (`Whte rbt.obj`), ya que se encontraba escondido dentro de un directorio oculto con un espacio como nombre (` `). Esto dificultó la navegación mediante comandos comunes, y fue necesario utilizar herramientas como `find` `sudo` `cat` y `ls` para visualizar correctamente los nombres de los directorios y poder acceder a ellos.

## Contenido

- Informe detallado y walkthrough: [MF0486_ExP_Di_zitti_marco.md](https://github.com/Markodzt/ctf-machines/blob/main/MF0486_%20Examen_Practico/MF0486_ExP_Di_zitti_marco.md)

- Capturas de pantalla y evidencias del proceso de explotación

## Resumen

- Reconocimiento y escaneo inicial
- Identificación y explotación de vulnerabilidades
- Acceso inicial y escalada de privilegios
- Obtención de flags y documentación de hallazgos

### Comandos empleados y su justificación

- `nmap` – para escanear puertos y servicios del host.
-  navegador web – para interactuar con servicios HTTP y detectar posibles archivos públicos.
- `grep`, `cat` – para analizar archivos de logs y buscar actividad sospechosa o relacionada con IPs externas.
- `find` – esencial para localizar archivos ocultos o sospechosos por nombre, extensión o fecha de modificación.
- `ssh` – utilizado para el acceso remoto cuando se encontraron credenciales válidas.
- `gpg` – para manejar archivos cifrados.
- `ls -lb` – para inspeccionar nombres de archivo con caracteres no visibles o especiales.
- `uname` - para encotrar versión del kernel, nombre etc...
- `sudo` – requerido para acceder a rutas protegidas.

---

*Para más detalles, consulta el archivo del walkthrough enlazado arriba.*



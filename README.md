# Kamaleon 2: Descargar por listas

[Español] | [English](README.en.md)

Este repositorio tiene como objetivo documentar y preservar el conocimiento sobre el uso de **Kamaleon 2**, utilizada en la década de los 2000 para la gestión, partición y camuflaje de archivos grandes.

![Interfaz de Unión - Selección](kamaleon-merge-1.png)

## ¿Qué era Kamaleon 2?

En una era donde los servicios de almacenamiento en la nube eran limitados y las velocidades de conexión eran bajas, Kamaleon permitía a los usuarios:
1. **Partir archivos grandes**: Dividir archivos en trozos más pequeños (ej. 1.44MB para disquetes o tamaños personalizados para servidores de hosting).
2. **Camuflaje (Pieles)**: Disfrazar las partes de un archivo como si fueran otros tipos de archivos (comúnmente imágenes .jpg) para evitar filtros de contenido o simplemente por discreción.
3. **Generación de Listas**: Crear archivos `.lst` o `.txt` con las URLs de descarga para ser procesadas por gestores de descarga.

## Contenido del Repositorio

- `kamaleon2.zip`: Archivo comprimido que contiene el programa original ejecutable.
- `Ayuda/`: Contiene los archivos originales del tutorial de ayuda del programa en español (HTML e imágenes).
- `Ejemplo/`: Ejemplo práctico.

---

# Guía de Uso 

Esta guía detalla los procesos principales del software Kamaleon 2 basándose en su documentación original.

## 1. Partir un Archivo
El proceso de partición permite dividir un archivo grande en partes más pequeñas.

1. **Selección**: Presionar el botón de "Archivo Origen" y seleccionar el archivo a procesar.
2. **Seguridad**: Opcionalmente, se puede establecer una contraseña para la unión posterior.
3. **Tipo de Partición**:
   - **Fijas**: Especificar el tamaño exacto en Bytes.
   - **Aleatorias**: Definir un rango (mínimo/máximo) para que cada parte tenga un tamaño distinto.
4. **Camuflaje (Pieles)**:
   - Se pueden usar "Pieles" para que las particiones parezcan archivos normales (como imágenes).
   - Kamaleon incrusta la información real dentro de estos archivos de fachada.
5. **Formato de Nombres**: Se puede elegir un nombre base o generar nombres aleatorios para las partes.

## 2. Unir un Archivo
Para recuperar el archivo original:

1. **Localización**: Es fundamental encontrar el **Último Archivo** de la serie de particiones. Este archivo "Principal" contiene los metadatos al final de su estructura.

![Interfaz de Partición](kamaleon-main-file.png)

2. **Verificación**: El programa realizará un chequeo minucioso para confirmar que todas las partes están presentes y no están dañadas.

![Interfaz de Unión - Progreso](kamaleon-merge-2.png)

3. **Destino**: Seleccionar la carpeta donde se reconstruirá el archivo original.

## 3. Generar Lista de Descarga
Útil para compartir archivos alojados en servidores web.

1. **Cargar Metadatos**: Seleccionar el último archivo de las particiones ya subidas.
2. **Configurar URL**: Introducir la URL base del servidor (ej. `http://misitio.com/archivos/`).
3. **Rangos**: Si los archivos están en diferentes servidores, se pueden configurar múltiples direcciones y rangos de partes.
4. **Archivo Final**: Se genera un archivo `.lst` o `.txt` compatible con la mayoría de los gestores de descarga.

![Generador de Listas](list.png)

## Gestores de Descarga
Históricamente se usaban programas como FlashGet o GetRight. Actualmente, se recomienda:
- **[JDownloader 2](https://jdownloader.org/)**: Soporta la importación de listas de enlaces y facilita la descarga por lotes.
- **[aria2](https://aria2.github.io/)**: Una utilidad de descarga multiprotocolo y multifuente ligera para la línea de comandos.

![aria2 Ejemplo](aria2.png)

## Compatibilidad y Requisitos
Kamaleon 2 es un software antiguo (Legacy) diseñado originalmente para Windows XP y 7. Sin embargo:
- **Windows 10**: Ha sido testeado exitosamente en **Windows 10 LTSC 21H2 (Compilación 19044.6456)**.
- **Linux**: Se recomienda el uso de **Wine** para ejecutar el binario `kamaleon2.zip`.
- **Otros**: En sistemas Windows modernos, si experimentas errores, intenta ejecutar el programa en "Modo de compatibilidad para Windows XP (Service Pack 3)".

---

## Ejemplo Práctico: Big Buck Bunny
Para este ejemplo práctico, se ha utilizado el cortometraje de **dominio público** (licencia Creative Commons) **Big Buck Bunny**. Este archivo ha sido procesado siguiendo este procedimiento:

1. **Partición**: El video original se ha dividido en múltiples partes de tamaño reducido.
2. **Camuflaje**: Cada parte ha sido "camuflada" utilizando imágenes (Pieles) para demostrar cómo se ocultaba el contenido real.

### Enlaces de Descarga del Ejemplo
Puedes copiar la siguiente lista de enlaces para usarlos en tu gestor de descargas (como JDownloader):

<pre>
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb001.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb002.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb003.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb004.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb005.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb006.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb007.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb008.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb009.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb010.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb011.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb012.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb013.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb014.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb015.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb016.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb017.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb018.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb019.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb020.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb021.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb022.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb023.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb024.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb025.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb026.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb027.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb028.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb029.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb030.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb031.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb032.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb033.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb034.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb035.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb036.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb037.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb038.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb039.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb040.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb041.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb042.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb043.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb044.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb045.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb046.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb047.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb048.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb049.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb050.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb051.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb052.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb053.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb054.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb055.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb056.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb057.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb058.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb059.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb060.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb061.jpg
https://raw.githubusercontent.com/Seechain/kamaleon2/main/Ejemplo/BigBuckBunny_512kb062.jpg
</pre>

También puedes descargar los archivos de lista directamente:
- [BigBuckBunny_512kb.txt](BigBuckBunny_512kb.txt)
- [BigBuckBunny_512kb.lst](BigBuckBunny_512kb.lst)

---


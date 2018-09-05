En el siguiente documento les mostraré algunos comandos y su uso.

Local : Sólo se necesitan archivos y documentos locales para operar. Las lee directamente de tu base de datos local.

Remote : Mostrará los nombres de cada uno de los remotos que tienes especificados.

Init : Crea un nuevo repositorio de git.

Clone: Hace una copia desde su central del código a la computadora.

Add : Recibe la ruta de un archivo

Commit : Identifica los cambios hechos en dicho ambiente de trabajo. Trabaja en tu repositorio local.

Push : Es un comando que sube los cambios hechos en tu ambiente de trabajo a una rama de trabajo tuya y/o de tu equipo remota. Trabaja a nivel de repositorio, es decir con tu repositorio remoto.

Pull : Es una abreviación de git fetch seguido de git merge FETCH_HEAD.
Baja los cambios de la rama determinada y la actualiza contra tu repositorio local.

Merge : Sirve para fucionar otra rama a tu rama activa.

~~~~FASES DE GIT~~~
Para entender mejor git, se explica mejor dividiendolo por fases, las cuales serán presentadas a continuación:

1.Untracked: En esta fase no se lleva un regristro de ese archivo(s).

2.Tracked : Esos archivos ya se están registrando (cambios).

3.Modified: Ese archivo está siendo modificado.

4.Staged : Archivo que ya añadiste para hacer un snapshot o un commited. Es un registro de tiempo.

5.Commited: Archivo que ya se respaldó o se le hizo un snapshot en el tiempo.

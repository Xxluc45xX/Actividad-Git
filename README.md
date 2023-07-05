# Actividad-Git
Actividad Git


**1.Investigación básica de Git:**
	
**A)¿Qué es Git y para qué se utiliza?** <br><br>
Git es un sistema de control de versiones distribuido, lo que significa que un clon local del proyecto es un repositorio de control de versiones completo. Estos repositorios locales plenamente funcionales permiten trabajar sin conexión o de forma remota con facilidad.

**B)¿Cuáles son las principales características de Git?** <br><br>
Git tiene la característica de ser un sistema de control de versiones con repositorios distribuidos. Esto quiere decir que cada uno de los integrantes de un proyecto tiene una copia exacta del repositorio y no solamente una copia de los archivos con los que haya trabajado.

**C)¿Qué es un sistema de control de versiones?** <br><br>
Los sistemas de control de versiones son software que ayudan a realizar un seguimiento de los cambios realizados en el código a lo largo del tiempo. A medida que un desarrollador edita el código, el sistema de control de versiones toma una instantánea de los archivos.

**¿Cuál es la diferencia entre Git y otros sistemas de control de versiones?** <br><br>
A diferencia de la mayoría de los otros sistemas de control de versiones, git almacena cada versión guardada como una 'instantánea' en lugar de una lista de los cambios realizados en cada archivo.


**2) Instalación y configuración de Git:** <br><br>

**A)Investiga cómo instalar Git en diferentes sistemas operativos (Windows, macOS, Linux)** <br><br>
**Windows:** <br>
Descarga el instalador oficial de Git para Windows desde el sitio web oficial: https://git-scm.com/download/win 
Ejecuta el archivo descargado y sigue las instrucciones del instalador.Asegúrate de seleccionar las opciones deseadas durante la instalación, como agregar Git al PATH y elegir la línea de comandos predeterminada (Git Bash o el símbolo del sistema de Windows).Haz clic en "Siguiente" en cada paso y luego en "Finalizar" para complt dageeretar la instalación.Para verificar que la instalación se realizó correctamente, abre una ventana de línea de comandos y escribe "git --version". Debería mostrarte la versión instalada de Git.<br><br>
**macOS:** <br><br>
Hay varias formas de instalar Git en macOS. La opción más sencilla es utilizar Homebrew, un administrador de paquetes para macOS.Abre la Terminal (puedes encontrarla en la carpeta "Utilidades" dentro de "Aplicaciones").Instala Homebrew si aún no lo tienes, siguiendo las instrucciones en el sitio web oficial de Homebrew: https://brew.shUna vez instalado Homebrew, ejecuta el siguiente comando en la Terminal: "brew install git"Espera a que la instalación se complete. Una vez finalizada, puedes verificar la versión instalada de Git ejecutando "git --version" en la Terminal.<br><br>
**Linux:** <br><br>
La forma exacta de instalar Git puede variar según la distribución de Linux que estés utilizando. A continuación, te mostraré cómo instalar Git en dos distribuciones populares:
**Ubuntu y Debian:** <br><br>
Abre una terminal.Ejecuta el siguiente comando: "sudo apt-get update"Luego, ejecuta el siguiente comando: "sudo apt-get install git"Espera a que la instalación se complete. Una vez finalizada, puedes verificar la versión instalada de Git ejecutando "git --version" en la terminal.<br><br>-
**B)Explica los pasos para configurar tu nombre de usuario y dirección de correo electrónico en Git.** <br><br>
Configura tu nombre de usuario ejecutando el siguiente comando:<br><br>
arduino
git config --global user.name "Tu nombre de usuario"
Reemplaza "Tu nombre de usuario" con tu nombre real o el nombre que deseas utilizar en tus commits de Git.
Configura tu dirección de correo electrónico ejecutando el siguiente comando:
arduino<br><br>
git config --global user.email "tuEmail.com"
Reemplaza "tu-correo-electronico@tuEmail.com" con tu dirección de correo electrónico real asociada a tu cuenta de Git.
Verifica la configuración ejecutando los siguientes comandos:
lua<br><br>
git config --global user.name
git config --global user.email
Deberían mostrar el nombre de usuario y la dirección de correo electrónico que acabas de configurar.
Ahora has configurado tu nombre de usuario y dirección de correo electrónico en Git a nivel global. Esto significa que se utilizarán en todos los repositorios Git en tu sistema. Si deseas configurar valores diferentes para un repositorio específico, puedes omitir la opción --global en los comandos anteriores y ejecutarlos dentro del directorio del repositorio en cuestión.<br><br>
**3.Comandos básicos de Git:** <br><br>
**A)Investiga los comandos git init, git add, git commit y git status. Explica qué hacen y cómo se utilizan.** <br>

**git init:**
Este comando se utiliza para inicializar un nuevo repositorio Git en un directorio.
Para usarlo, ve al directorio de tu proyecto en la línea de comandos y ejecuta git init.
Esto creará una carpeta oculta llamada .git que contendrá todos los archivos y metadatos necesarios para el control de versiones en Git.<br><br>
**git add:** <br><br>
El comando git add se utiliza para agregar cambios o archivos al área de preparación (también conocida como "staging area") de Git.
Puedes agregar archivos individuales utilizando git add nombre-del-archivo o agregar todos los archivos modificados en el directorio actual con git add .Esto prepara los cambios para ser incluidos en el próximo commit.<br><br>
**git commit:** <br><br>
git commit se utiliza para crear un nuevo commit (instantánea) que contiene los cambios preparados en el área de preparación.
Un commit es una unidad lógica de cambios en Git y representa un punto en la historia del proyecto.
Para realizar un commit, ejecuta git commit -m "Mensaje del commit" donde "Mensaje del commit" describe brevemente los cambios realizados en el commit.
Después de ejecutar el comando, los cambios se guardarán en el repositorio de Git.<br><br>
**git status:** <br><br>
git status muestra el estado actual del repositorio de Git, incluyendo los archivos modificados, agregados o eliminados, y si están preparados para el commit o no.
Te brinda información sobre qué archivos han sido modificados y aún no se han agregado, y qué archivos han sido agregados pero no se han confirmado con un commit.
Puedes ejecutar git status en cualquier momento para obtener una visión general del estado de tu proyecto.<br><br>
**B)Describe los comandos git log y git diff para ver el historial de cambios y las diferencias entre versiones, respectivamente.**



**Git Log**<br><br>
El comando git log muestra el historial de commits en el repositorio. Proporciona información detallada sobre los commits realizados, como el autor, la fecha, el mensaje del commit y un identificador único (hash).Al ejecutar git log en la línea de comandos, se mostrará una lista de commits en orden cronológico inverso (el commit más reciente aparece primero).Puedes navegar por el historial del commit utilizando las teclas de flecha


**git diff:** <br><br>
El comando git diff muestra las diferencias entre versiones, ya sea entre commits, entre el área de preparación (staging area) y el último commit, o entre un commit y el directorio de trabajo actual.Cuando ejecutas git diff, se muestran las líneas modificadas, agregadas o eliminadas en los archivos que han cambiado.Por ejemplo, git diff sin ningún argumento muestra las diferencias entre el directorio de trabajo actual y el área de preparación.También puedes utilizar opciones adicionales con git diff para mostrar diferencias específicas, como --staged para comparar el área de preparación y el último commit, o especificar commits específicos para comparar.Este comando es útil para revisar y comprender los cambios realizados en tus archivos antes de confirmarlos con un commit.<br><br>
**4.Trabajando con repositorios remotos:** <br><br>
**A) Investiga cómo clonar un repositorio remoto con git clone** <br><br>
1.Abre una terminal o línea de comandos en el directorio donde deseas clonar el repositorio.<br>
2.Obtén la URL del repositorio remoto que deseas clonar. Por lo general, la URL se encuentra en la plataforma de alojamiento del repositorio, como GitHub, GitLab o Bitbucket.<br>
3.En la terminal, ejecuta el siguiente comando: <br>
bash
git clone <URL_del_repositorio>
Reemplaza <URL_del_repositorio> con la URL que obtuviste en el paso anterior. Por ejemplo:
bash
git clone https://github.com/usuario/repositorio.git
Presiona Enter para ejecutar el comando. Git comenzará a clonar el repositorio remoto en tu directorio local.Dependiendo del tamaño del repositorio y la velocidad de tu conexión a Internet, el proceso de clonación puede llevar algún tiempo.Una vez completado el proceso de clonación, tendrás una copia completa del repositorio remoto en tu directorio local. Puedes realizar cambios, crear nuevas ramas, hacer commits y más en esta copia local.<br><br>
**B.Explica cómo trabajar con ramas utilizando los comandos git branch, git checkout y git merge.** <br><br>
Trabajar con ramas es una parte fundamental de Git y te permite desarrollar nuevas características, experimentar cambios y colaborar de manera eficiente en proyectos. Los comandos principales para trabajar con ramas son git branch, git checkout y git merge. Aquí tienes una explicación de cada uno y cómo se utilizan:<br><br>
**git branch:** <br><br>
El comando git branch se utiliza para administrar y ver las ramas en un repositorio.Para ver todas las ramas existentes en el repositorio, ejecuta git branch sin ningún argumento.Para crear una nueva rama, ejecuta git branch <nombre-de-la-rama>. Por ejemplo, git branch nueva-rama creará una nueva rama llamada "nueva-rama".Puedes eliminar una rama utilizando git branch -d <nombre-de-la-rama>. Ten en cuenta que no podrás eliminar una rama si tienes cambios pendientes en ella.El comando git branch -a muestra todas las ramas, tanto locales como remotas. <br><br>
**git checkout:** <br><br>
El comando git checkout se utiliza para cambiar entre ramas o crear una nueva rama y cambiar a ella al mismo tiempo.Para cambiar a una rama existente, ejecuta git checkout <nombre-de-la-rama>. Por ejemplo, git checkout nueva-rama cambiará a la rama llamada "nueva-rama".Si deseas crear una nueva rama y cambiar a ella al mismo tiempo, puedes utilizar git checkout -b <nombre-de-la-rama>. Por ejemplo, git checkout -b mi-rama creará una nueva rama llamada "mi-rama" y cambiará a ella.<br><br>
**git merge:** <br><br>
El comando git merge se utiliza para fusionar cambios de una rama en otra.Primero, asegúrate de estar en la rama de destino, es decir, la rama en la que deseas incorporar los cambios.Ejecuta git merge <nombre-de-la-rama> para fusionar los cambios de <nombre-de-la-rama> en la rama actual.Git intentará combinar automáticamente los cambios, pero en algunos casos puede surgir un conflicto. Si esto ocurre, deberás resolver manualmente los conflictos antes de completar la fusión.Una vez que se completa la fusión, los cambios de la rama fusionada se incorporan a la rama de destino.<br><br>
**C. Investiga cómo subir tus cambios locales a un repositorio remoto con git push.** <br><br>
Asegúrate de haber realizado los commits necesarios en tu repositorio local. Los cambios que desees subir deben estar confirmados mediante commits.
Verifica que estás en la rama correcta desde la cual deseas realizar el push. Puedes usar el comando git branch para mostrar todas las ramas y verificar en cuál te encuentras actualmente. Si necesitas cambiar de rama, puedes utilizar el comando git checkout <nombre-de-la-rama>.
Asegúrate de tener configurada correctamente la URL del repositorio remoto. Puedes utilizar el comando git remote -v para mostrar las URL configuradas para el repositorio remoto. Si aún no tienes una configurada, puedes usar el comando git remote add origin <URL_del_repositorio> para agregar una nueva URL. Reemplaza <URL_del_repositorio> con la URL correcta del repositorio remoto.<br><br>
Una vez que estés en la rama correcta y tengas configurada la URL del repositorio remoto, ejecuta el siguiente comando:
php
git push <nombre-remoto> <nombre-rama>
Reemplaza <nombre-remoto> con el nombre del repositorio remoto (por lo general, "origin") y <nombre-rama> con el nombre de la rama local que deseas subir al repositorio remoto. Por ejemplo:
css
git push origin main
Esto enviará los cambios realizados en la rama local "main" al repositorio remoto llamado "origin".
Dependiendo de la configuración del repositorio remoto, se te puede solicitar que ingreses tus credenciales (como tu nombre de usuario y contraseña) para autenticarte antes de que los cambios se suban correctamente.<br><br>
**5 Colaboración en Git:** <br><br>
**A. Investiga cómo trabajar en equipo en un repositorio remoto utilizando ramas y fusiones.** <br><br>

Trabajar en equipo en un repositorio remoto utilizando ramas y fusiones en Git es una práctica común y eficiente. Aquí tienes los pasos generales para trabajar en equipo de esta manera:<br><br>
1. Clona el repositorio remoto: Comienza clonando el repositorio remoto en tu máquina local utilizando el comando `git clone <URL_del_repositorio>`. Esto creará una copia local del repositorio en tu directorio de trabajo.<br>

2. Crea una rama de trabajo: Antes de comenzar a trabajar en una nueva característica o solución, crea una nueva rama utilizando el comando `git checkout -b <nombre-de-la-rama>`. Elige un nombre descriptivo para la rama que refleje el objetivo de tu trabajo.<br>

3. Sincroniza con el repositorio remoto: Antes de fusionar tu rama con la rama principal, es importante sincronizar con el repositorio remoto. Utiliza `git pull` para obtener los cambios más recientes del repositorio remoto y asegurarte de que estás trabajando sobre la última versión.<br>

4.Realiza los cambios y realiza commits: Realiza los cambios necesarios en tu rama de trabajo y realiza commits con git commit para guardar tus cambios de manera lógica y separada. Es una buena práctica hacer commits frecuentes y atómicos para mantener un historial de cambios limpio y comprensible.<br>

**B. Explica qué son las solicitudes de extracción (pull requests) y cómo se utilizan para revisar y aprobar cambios.**  <br><br>


  Las solicitudes de extracción, también conocidas como "pull requests", son una función de las plataformas de alojamiento de repositorios como GitHub, GitLab y Bitbucket. Permiten a los desarrolladores proponer cambios en un repositorio sin fusionarlos directamente en la rama principal. Los pasos para utilizar las solicitudes de extracción son:<br>

1. Crear una nueva rama para realizar los cambios.<br>
2. Realizar commits y subir la rama al repositorio remoto.<br>
3. Abrir una solicitud de extracción, describiendo los cambios realizados.<br>
4. Revisar y comentar los cambios propuestos.<br>
5. Realizar ajustes según los comentarios recibidos.<br>
6. Aprobar y fusionar la solicitud de extracción en la rama principal.<br><br>

Las solicitudes de extracción facilitan la revisión y la colaboración, permitiendo que los cambios sean discutidos y mejorados antes de su incorporación al repositorio principal. Proporcionan un historial claro de los cambios y las conversaciones relacionadas con ellos.<br>

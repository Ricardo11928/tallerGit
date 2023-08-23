# Soluciona el siguiente cuestionario.

**_(Valor por pregunta : 5pts)_**
## Opción Múltiple:

1. **¿Qué comando se utiliza para clonar un repositorio remoto?**
    * git clone
    ---
1. **¿Cuál es el propósito del comando `git pull`?**
   * Descargar y fusionar cambios desde un repositorio remoto.
    ---
1. **¿Cuál es el comando para crear una nueva rama en Git?**
   * git checkout
    ---
1. **¿Qué hace el comando `git status`?**
    * Muestra el estado de los archivos en el repositorio.
    ---
1. **¿Cómo se deshacen los cambios no confirmados en Git?**
   * git revert

## Verdadero/Falso:

1. **En Git, cada confirmación se identifica por un hash único.**
   * Verdadero
    ---
2. **Git es un sistema de control de versiones centralizado.**
   * Falso
    ---
3. **El comando `git merge` se utiliza para crear una nueva rama.**
   * Falso
    ---
4. **El comando `git stash` se utiliza para descartar permanentemente los cambios locales.**
   * Falso
    ---
5.  **Git es únicamente útil para programadores y no tiene aplicaciones en otros campos.**
    *  Falso

# Preguntas Abiertas:

1.  **_Describe el proceso de resolución de conflictos en Git cuando se fusionan dos ramas._**
    * Una vez se funcionan dos ramas que tienen conflictos (Cambios dentro del mismo archivo en ambas ramas)
    Se debe resolver el conflicto manualmente, revisando las lineas que fueron afectadas y haciendo los ajustes correspondientes
    Finalmente se realiza un commit confirmando que se solventaron los conflictos.
    ---
2. **_¿Por qué es importante crear confirmaciones (`commits`) atómicas y descriptivas en Git?_**
   * Es importante crear commits atomicos y descriptivos para que a la hora de realizar un Pull Request el Reviewer pueda saber que fue lo que se altero en el proyecto
   En esta misma linea, tambien es importante para poder identificar de manera mas rapida problemas con la aplicacion.
    ---
3. **_Explica el concepto de ramificación (`branching`) en Git y cómo puede ser beneficioso en el desarrollo de software._**
   * Las ramas en git son extensiones del proyecto principal, generalmente utilizadas para realizar cambios. Esto es extremandamente
   beneficioso en el desarrollo de software ya que, con un flujo de trabajo bien implementado, permite la posibilidad de llevar
   varios desarrollos o implementacioens al mismo tiempo de manera organizada.
    ---
4. **_¿Qué es un repositorio remoto en Git y cómo se conecta a un repositorio local?_**
   * Un repositorio remoto de git es un repositorio de git que se encuentra alojado en el internet, normalmente en un servicio centralizado como Github, GitLab o Bitbucket
   y este se puede conectar a un repositorio local clonando el repositorio que se encuentra remoto a traves de sistemas de verificacion de seguridad HTTPS o SSH
    ---
5. **_Menciona algunos posibles casos de uso para el archivo `.gitignore`._**
   * El archivo .gitignore es importante para excluir o no permitir que usuarios modifiquen ciertos archivos. Por lo general son archivos sensitivos como variables de entorno,
   claves, archivos de configuracion, etc.
    ---
6. **_¿Qué es un conflicto de fusión (`merge conflict`) y cómo se resuelve?_**
   * Un merge conflict ocurre cuando se intenta mezclar dos ramas en donde se modificaron los mismos archivos. Para solucionar esto
   se creara una rama `...| MERGING` en donde se debe identificar manualmente cual es el conflicto y hacer los ajustes correspondientes.
   Para culminar con un commit y volver a subir los cambios.
    ---
7. **_¿Cómo se crea una etiqueta (`tag`) en Git y en qué escenarios se suele utilizar?_**
   * En git los tags se pueden crean con la etiqueta `tag -a` o directamente desde un servicio como Github donde te permiten agregar los tags desde una interfaz grafica. Estos suelen utilizarse para llevar un mejor control de versionamiento en cuanto a los cambios que se hacen dentro del proyecto.
    ---
8. **_Describe el flujo de trabajo básico en Git, desde la creación de un repositorio hasta la colaboración en equipo._**
   * Podemos crear un repositorio remoto, ya sea publico o privado, con una rama principal. Damos acceso a los distintos miembros los cuales queremos que colaboren. Posteriormente creamos distintas ramas de trabaja las cuales vamos a tener en nuestros repositorios locales que seran una clonado de la rama principal del repositorio remoto. Luego de realizar las modificaciones deseados se procede a subir los cambios al repositorio remoto y se actualizan los cambios con la rama prinicpal.
    ---
9.  **_¿Cuál es el propósito del comando `git rebase` y cuáles son sus implicaciones?_**
    * El comando `git rebase` se utiliza para poder apuntar el `HEAD` o ultimo commit a un commit distinto al ultimo generado en la linea del tiempo. Esto puede implicar que vayan a existir cambios o versiones mas actualizadas al `HEAD` dentro del proyecto.
    ---

10. **_Explica qué es el flujo de trabajo Gitflow y cómo se estructuran las ramas en este enfoque._**
    * El flujo de trabajo Gitflow se basa en un marco estandarizado de trabajo en donde existen ramas especiales para cada tipo de desarrollo que se requiera y las mismas lleven un orden en el ciclo de vida del desarrollo. Normalmente se estructura con una rama prinicpal **main** en donde se encuentra la version estable mas actualizada del proyecto. Luego existe una rama **develop** que es de donde nacen todas las ramas de trabajo **feature** o **bugfix** que son las que se utilizan para el desarrollo de nuevas funcionalidades o cambios. Tambien existen estructuras **hotfix** que se utilizan para cambios urgentes que perjudiquen la operacion del aplicativo y estas nacen de la rama principal.
# ¿QUE ES LA TERMINAL?

<!--italic -->
 Es una interfaz *italic* <span style="font-family:'Bebas Neue'">gráfica</span> que simula una línea de comandos.Cuando hablamos de una línea de comandos nos referimos a una "shell".
<!-- UL -->
* Terminal: Una venta que nos muestra el PROMPT. Esta aloja en la shell.
* Linea de comandos (shell):Un programa que toma comandos y los pasa al sistema operativo para hacer algo.

     # Algunos tipos de shellls
Bourne shell, Bash shell, Z shell, C shell, Korn shell, Fish shell, Power shell.

![terminal](https://blogthinkbig.com/wp-content/uploads/sites/4/2020/04/Ubuntu-Terminal-Desktop.jpg?resize=450%2C220)

   # Aprendiendo a caminar en la Terminal

1. LS= Lista de archivos para ver su peso de una manera legible .

2. LS-LH= Lista de archivos ocultos. 

3. LS-A= Identificar la ruta en la que estamos en el Sistema .

4. PWD= Movernos entre directorios.

5. CD= Crear un directorio CD solo lo de vuelve al HOME.

6. MKDIR= Copiar un archivo. 

7. CP= Mover un archivo.

8. RM= Borrar un archivo.

9. MV= Mover un archivo a un directorio anterior .

10. RMDIR= Limpiar laa terminal.

11. CLEAR= Limpiar terminal.

12. FILE= Las propiedades del archivo o carpeta.

### operaciones de ls
* -a = muestra todo .
* -R = lista de manera recursiva.  
* -r = lista inversa .
* -t = ultimas modificaciones. 
* -s = orden por tamaño.
* -l = formato largo.


>MANIPULACION  ARCHIVOS Y DIRECTORIOS.
---
ls- la:archivos ocultos/.
ls- ls o lsh: tamaño de documento/.
ls- lr: archivos inverso/.
tree- l2: despliega todo el directorio/.
touch: crea un archivo/.
cp file 1: copia un archivo/.
cp file -bk: nombra un archivo.
____

---
* rm"nombre del archivo" : BORRA el archivo nombrado.
* rm -i o rm -ri "nombre del archivo": permite que aprueves que borre el archivo.
---
>EXPLORAR EL CONTENIDO DE NUESTROS ARCHIVOS.
* HEAD"el nombre del archivo de texto"
    * permite ver las primeras 10 lineas de texto.
* HEAD"nombre del archivo" -n "?"
    * numero de lineas que desees.
* TAIL"nombre del archivo" -n
    * ultimas lineas.
* LESS"nombre de archivos"
    * muestra todo el archivo de manera muy interactiva y con "/" puedes buscar la palabra deseada.
* XDG-OPEN"nombre del archivo"
    * habre el archivo en el editor de texto predeterminado . desactivas el proseso con  ctrl + c.
* NAUTILUS DOCUMENTOS/ "nombre de la carpeta"
    * permite habrir la carpeta de archivos mas rapido o la carpeta que deseamos. 

## Su majestad: Grep
![imagenGrep](https://geekland.eu/wp-content/uploads/2022/06/uso-del-comando-grep-en-linux.webp)

* Grep towers movies.csv= Grep es una herrramienta bastante util para buscar las lineas que deseas.

* Grep the movies.csv= Todas las coincidecia que tenga "grep -i the movies.cvs" con mayuscula tambien.

* Grep -c the movies.csv o Grep -ci movies.cvs.

* wc movies.cvs= indica cuantas lineas tiene o palabras.

* Grep -v tower movies.cvs o Grep -vi towers movies.cvs > sintower.txt= lo guarda en un archivo.

## Utilidades de red

1. ifconfig: Da informacion de la red de la cpu.

2. ping www.google.com: Nos manda una respuesta continua de la pagina se para la ejecucion con ctrl-c.

3. curl www.google.com: trae la estructura HTML de la pagina que elejimos.

4. wget www.google.com: Descarga el archivo directo a la cpu lo guarda en un archivo HTML.

5. traceroute www.google.com: Muestra por donde nos emos movido todas las computadoras que intervienen para llegar a la pagina.

6. netstat -i: Muestra los dispositivos de red.

# Procesos en Foreground y Background

Cuando un proceso esta en ejecucuion sin que sea mostrado en la terminal se dice que esta ejecutando en el BACKGROUND. si se muestra la ejecucion del comando dentro de la terminal se dice que esta en el FORGROUND.

> jobs: Permite saber si el archivo o texto esta en el BACKGROUD.

> Fg1 o Fg%1: Permite sustraer el archivo del Background y devolver al FORGROUND.

Para moverlo al BACKGROUD usamos ctrlZ enves de ctrlD que es para guardarlo y mandarlo al INPUT otra manera de enviar al BACKGROUD. Es usando el operador & al final del comando, otra forma es usado el bg1.

# Editor de texto en la terminal

>VIM: Para salir de vim usamos [: y q] para escribir en el editor vim preciona la tecla "i" se usa ESC para navegar en el. 
Con la tecla "/" nos permite escribir la palabra que deseamos buscar.
Para guardar se usa :W para guardar y salir :WQ para salir sin guardar se usa :WQ! de manera forzada.
--------------------------------------------


#     GIT  Y  GITHUD 
![gitimagesgithud](https://blog.facialix.com/wp-content/uploads/2021/04/git-github-cero-facialix.jpg)
>GIT:Es un sistema de control de versiones, pensando para la eficiencia y la confiabilidad del mantenimiento de versiones en un proyecto. Git funciona como una lina de tiempo que nos permite regresar a momentos especificos del codigo.

#### Su proposito es:
* llevar un registro de 
los cambios | Coordinar el trabajo de varias personas
---
Es un sistema de control de versiones,guarda solamente los cambios realizados en algun archivo o proyecto

* $git init: Inicia el repositorio de git.
* $git add (nombre del archivo): Git comienza a hacerle un seguimiento de archivo en cuenstion. 
* $git commit-m(mensaje): Envia los ultimos cambios del archivo a la base de datos del sistema de control de versiones, para controlar los cambios que se le hayan hecho.
Es tan simple este comando que nos permite hacer ua captura o guardar en el tiempo los cambios realizados que estabn en el esenario.
* $git add: Es otra forma de agregar archivos.Este comando agrega todos los archivos que hayan cambiado en el esenario
* $git show: Mostrara todos los cambios que hemos hecho, esto incluye las lineas que hemos cambiado, cuando y quien hizo dichos cambios.
* git status: Me permite saber que archivos y caules no fueron agregados al esenario.
* git log: Para ver la  historia completa de un archivo.

>DIRECTORIO EN GIT:Es el lugar donde se almacenan los metadatos y las bases de datos para nuestros proyectos, y es justamente lo que se copia cuando clonamos de un ordenador a otros archivos.
![imagesgit](https://vabadus.es/images/cache/imagen_nodo/images/articulos/5c9deedea0c7e844300455.png)

### Caracteristicas de Git
1. Git alamacena la informacion como un conjunto de archivos.
2. No existen cambios, corrupcion en archivos o cualquier alteracion sin que git lo sepa.
3. Casi todo en git es local.Es dificil que se necesiten recursos o infomacion externos, basta con los recursos locales con los que cuenta.
4. Git cuenta con 3 estados en los que es posible localizar archivos: staged, modified, committed.

>GITHUD:Es una forja para alojar proyectos utilizando el sistema de control de versiones Git.Se utiliza principalmante para la creacion de codigo fuente de programas de ordenador.El sofware que opera Githud fue escrito en Ruby on Rails.
![imagesgihud](https://global-uploads.webflow.com/5f5a53e153805db840dae2db/6073fbf151fa4565d48572dc_GitHub_aprender-programaci%25C3%25B3n.jpeg)

### Caracteristicas de Githud
1. Githud permite alojar proyectos en repositorios de forma gratuita y publica, pero tiene una forma de pago para privados.
2. Puedes compatir facilmente tus proyectos.
3. Permite colaborar para mejorar los proyectos de otros y a otros mejorar o aportar a los tuyos.
4. Ayuda a reducir significativamente los errores humanos, a tener un mejor mantenimiento de distintos entornos y a detectar fallos de una forma mas rapida y eficiente.
5. Es la opcion perfecta para poder trabajar en equipo en un mismo proyecto.
6. Ofrece todas las entajas del sistema de control de versiones Git, pero tambien tiene otas herramientas que ayudan a tener un mejor control de los proycetos.

### Que es el sistema de control de versiones 
Es SCV o VCS es un sistema que registra los cambios realizados sobre un archivo o conjunto de archivos a lo largo del tiempo, de modo que puedas llevar el historial del ciclo de vida de un proyecto, comparar cambios a lo largo del tiempo, ver quien los realizo o revertir el proyecto entero a un estado anterior.

### Analizar cambios en los archivos de tu proyecto con Git
El comando git show nos muestra los cambios que han existido sobre un archivo y es muy util para detectar cuando se produjeron ciertos cambios, que se rompio y como lo podemos solucionar.

### ¿ QUE ES BRANCH(RAMA) Y COMO FUNCIONA UN MERGE EN GIT ?
![gitimagenbrach](https://res.cloudinary.com/snyk/images/f_auto,q_auto/w_1240,h_384,c_scale/v1/wordpress-sync/image1-11/image1-11-1240x384.png)

La rama o brach es una version del codigo del proyecto sobre el que estas trabajando.Estas ramas ayudan a mantener el orden en el control de versiones y manipular el codigo de forma segura.

* RAMA MAIN(MASTER)
  * Por defecto, el proyecto se crea en una rama llamada Main cada vez que añade codigo y guardas los cambios, estas haciendo un commit, que es añadir el nuevo codigo a una rama.Esto genera nuevas versiones de esta rama o branch, hasta llegar a la version actual de la rama MAIN.
* RAMA DEVELOPMENT
  * Cuando decides hacer experimentos, puedes generar ramas experimentales (usualmente llamadas development), que estan basadas en alguna rama main, pero sobre las uales puedes hacer cambios a tu gusto sin necesidad de afectar directamente al codigo principal.
* RAMA HOTFIX
  * En otros casos, si encuentras un bug o error de codigo en la rama main (que afecta al proyecto en produccion) tendras que crear una nueva rama que usualmente se llama (bug fixing o hot fix) para hacer los arreglos necesarios.Cuando los cambios esten listos, los tendras que fusionar con la rama main para que los cambios sean aplicados. Para esto, se usa un comando llamado [Merge] que mezcla los cambios que originaste a la rama Main.

  ##  GIT reset Vs GIT rm
  ![imagensreset](https://static.platzi.com/media/user_upload/Git%20rm%20Git%20Reset-91d9ece5-b894-48ca-8102-f3bc9e91c5f1.jpg)

  * Git rm:
  Este comando nos ayuda a eliminar archivos de git sin eliminar su historia del sistema de versiones.Esto quiere decir que si necesitamos recuperar el archivo solo debemos "viajar en el tiempo" y recuperar el ultimo commit antes de borrar el archivo en cuestion.
   1. git rm --cached:
  Elimina los archivos de nuestros repositorio local y del area de stoging, pero los mantiene en nuestros disco duro.Basicamente le dicea git que deje de tracker el historial de cambios de estos archivos, por lo que pasaron a un estado untracked.
   2. git rm --force:Elimina loos archivos de git del discoduro.Git siempre guarda todo, por lo que podemos acceder al registro de la existencia de los archivos, de modo que podemos recuperar si es nesesario.
   * git reset:Este comando nos ayuda a volver en el tiempo.Pero no como git checkout que nos deja ir, mirar pasar o volver.Con git reset volvemos al pasado sin la posibilidad de volver al futuro.Hay dos formas de usarlo
   1. git reset--soft:Borramos todo el historial y los registros de git pero guardamos lo cambios que tengamos en staging, asi podemos plicar las ultimas actualizaciones a un nuevo commit.
   2. git reset --hard:Borra todo.Todo todito, absolutamente todo.Toda la informacion de los commints y del area de staging se borra del historia.

   >git reset HEAD:Este es el comando para sacar archivos del area de staging.No paraa borrarlos ni nada de eso, solo para que los ultimos cambios de estos archivos no se envien al ultimo commit, a menos que cambiemos de opinion y los incluyamos de nuevo en staging con git add. 
### Utlizando PULL Requests en Giyhud
![imagenpull](https://www.simplilearn.com/ice9/free_resources_article_thumb/pull_request_vs_merge_request.jpg)
* pull request:Es una funcionalidad de githud (en githud llamda merge request y en bitbuckt push request) en la que un colaborador pide que revisen sus cambios antes de hacer merge a una rama, normalmente master.
Al hacer un pull request se genera una conversacion que pueden seguir los demas usuarios del repositorio, asi como autorizar y rechazar los cambios.
### Readme.md una execelente practica
![imagenreadme](https://media.geeksforgeeks.org/wp-content/uploads/20210915020701/Readme1.png)
1. README.md:Es el lugar donde se explica se explica de que trata el proyecto como ultilizarlo y demas informacion que se considere que se deba conocer  antes de utilizar un proyecto.
2. Los archivos README son escritos en lenguaje llamao MARKDON, por eso la entension. MD, mismo que es un estandar de escritura en diversos sitios.
 

## BASE DE DATOS
![imajendatos](https://i.ytimg.com/vi/knVwokXITGI/maxresdefault.jpg)
* ¿Que es una entidad?
   1. Es algo similar a un objeto y representa algo en el mundo real incluso algo abstrato.Tiene atributos que son las cosas que los hacen ser una entidad.
* ¿Que es un aributo?
    1. Son las caracteristicas o propiedades que describen a la entidad.Los atributos se compen de:
    2. Atributos compuestos son aquellos que tiene atributos de ellos mismos.
    3. Atributos llave sona aquellos que identifican a  la entidad y no pueden ser repitidos.

### SQL
![imagensql](https://www.datocms-assets.com/14946/1627286560-sql-databases.png?auto=format&fit=max&w=1200) 
SQL significa STRUTURED QUERY LANGUAGE y tiene una estrutura clara y fija. Su onjetivo es hacer un solo lenguaje para consultar cualquier manejador de bases de datos volviendose un gran estadar.
### DDL CREATE
![imagenddl](https://i.ytimg.com/vi/zUNfiVql5CQ/maxresdefault.jpg)
DDL o DATA Definition Languaje que nos  ayuda a crear la estrutura de una base de datos
* create:Nos ayuda a crear bases de datos, tablas, vistas, indices, etc.
* alter:Ayuda a alterar o modificar entidades.
* Drop:Nos ayuda a borrar.Hay que tener cuidado al utilizarlo.
### DML
![imagendml](https://basededatosutp22.files.wordpress.com/2016/04/dmlsentencias.png)
Trata

 del conteido de la base de datos.Son las siglas de Data Manipulation Languaje y sus comandos son:
 1. Inset:Inserta o agrega nuevos registos a la tabla
 2. Update:Acrualiza o modifica los datos que ya existen
 3. Delete:Esta sentencia es riesgosa porque puede borrar el contenido de una tabla.
 4. Select:Trae informacion de la base de datos.
 ## ESTRUTURA BASICA DE UN QUERY
 Los query son la forma en la que estruturamos la preguntas que se haran a la que estructuramos las preguntas que haran a la base de datos.
 1. SELECT:Que datos queremos obtener que columnas/campos de la tabla.
 2. FROM:De donde los queremos obtener, de que tabla exatamente.
 3. WHERE:Condicion que deben cumplir o filtar que deben pasar los datos a obtener.Es opcional, pero se suele utilizar ya que sino se obtiene todos los datos sin filtar ninguno.
 4. GROUP BY:De que manera agrupamos los datos (agrupaddos en ciudades)
 5. ORDER BY:De que manera ordenamos los datos(en este caso por poblacion)
 ## FROM
 ![fromimajes](https://upload.wikimedia.org/wikipedia/commons/2/29/Base_de_datos_de_particulares.jpg)
 * Indica de done se deben traer los datos y puede ayudar a hacer sentencias y filtros complejos cuando se quieren unir tablas.La sentencia compañera que nos ayuda con este proceso es JOIN
 * Los diagramas de Venn son circulos que se tocan en algun punto para ver donde esta la interseccion de conjuntos.Ayudan mucho para poder formular la sentencia JOIN de la manera adecuada dependiendo del query que se quiere hacer.
# JOIN-Teoria de conjuntos.
![joinimajes](https://i.blogs.es/9d18f9/visual_join_cheatsheet/450_1000.jpg)
## Nulo o no NULO
NULL no corresponde a ningun valor en particular, sino a una "ausencia" de valor, por lo tanto un NOT NULL corresponderia a que no hay una aparente ausencia, es decir, existe un valor asi sea un o.NULL no es igual a nada por lo que en SQL no se le atribuye a un WHERE con un IS NULL.Para valores NOT NULL, tambien se aplica la misma sintaxis.Para agregar un criterio adicioanl con WHERE, se usa AND.
## Nested queries
![imagesqueries](https://www.w3resource.com/w3r_images/nested-subqueries-2nd-step.gif)
Significa que dentro de un query podemos hacer otro query.Esto sirve para hacer join de tablas,estando una en memoria.Tambien teniendo un query como condicional del otro.
Este proceso puede ser tan profundo como quieras, teniendo infinitos query anidados.
# Base de datos no relacionales
Contiene una amplia gama de DBMSS que difieren del modelo de bases de datos relacionales y como caracteristicas destacable no usa SQL.
![imajesnorelacion](https://miro.medium.com/max/811/1*UP3aK7hbAqYU6j8szceWpg.png)
Tipos de base dato no relacionales.
* CLAVE - VALOR:Son ideales para almacenar y extraer datos con una clave unica.Manejan los diccionaios de manera excecional.Dy namoDB Cassandra.
* Basedas en documentos:Son una implementacion de clave valor que varia en la froma semiestructurada en que se trat la infomacion.Ideal para almacenar datos ISON y XML, MongoDB Firestore.
* Basadas en grafos:Basadas en teoria de grafos, sirven pra entidades que se encuentran interconectadas por multiplees realciones.Ideales para almacenar realciones complejas. neo4, TITAN.
* En memorias:Pueden ser de estructura variada pero su ventaja radica en la velocidad, ya qie el vivir en memorias la extracion de datos casi Inmediata.Mencached, redies






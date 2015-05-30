# Plataforma de cursos

### Tabla de contenidos
* [Proyecto](#proyecto)
  * [Visión General](#vision-general)
  * [Funcionalidades](#funcionalidades)
    * [Principales](#principales)
    * [Secundarias](#secundarias)
* [Entregas](#entregas)
    * [Entrega 1](#entrega-1)
    * [Entrega 2](#entrega-2)
    * [Entrega 3](#entrega-3)

# Proyecto

## Vision General
> Idea original de: Grupo 2
  
La aplicación consiste en una herramienta educativa para la administración de cursos y la difusión del conocimiento. Es posible en ella crear cursos privados, los que servirán por ejemplo, para que profesores de instituciones académicas lleven una sencilla administración de su curso. También se pueden crear cursos públicos, los que servirán para que alumnos de distintos lugares e instituciones puedan aprender lo que se ensena en otros lugares, y a su vez, compartir el conocimiento mediante foros y chat uno a uno. Los cursos pueden ser administrados por una o más personas con distintos niveles de privilegio (Profesor, asistente, etc.), pero estos solamente pueden ser creados por gente que tenga los permisos necesarios. Finalmente, la aplicación contara con un sistema de visualización de estadísticas para enterarnos de los cursos más vistos, los materiales más utilizados, los usuarios destacados, el avance personal, etc.

## Funcionalidades

A grandes razgos, el proyecto debe cumplir con los siguientes requerimientos.

### Principales
* **Administradores**:
 * Asignar a usuarios la capacidad de crear cursos y asignar colaboradores.
 * Moderar curso en caso de ser necesario.
* **Profesores**:
 * Crear curso.
 * Asignar colaboradores (ayudantes, por ejemplo).
 * Asignar módulos al curso (Foro, sistema de cuestionarios, calificaciones, asistencia, repositorio de material).
* **Alumno**:
 * Si un usuario fue inscrito a un curso privado, este puede ingresar a él y tener acceso a toda la información.
 * Un usuario puede acceder a cualquier curso público y hacer uso del contenido que este publicado.
* **Página principal**:
 * Capacidad de registrarse en la aplicación
 * Login, conocer la aplicación etc.
* **Página principal (una vez logeado)**:
 * Sistema de buscador de cursos.
 * Recomendación de cursos.
 * Acceso a visualización de tareas por hacer en cursos inscritos, estadísticas del rendimiento individual, notificaciones de los diversos cursos (privados y no privados), etc.
 *Acceso a visualización de estadísticas de cursos interesantes, cursos nuevos, contenido m as visto, etc.
* **Curso Privado**:
 * Este curso tiene la capacidad de llevar registro de información que una entidad académica desearía tener, como vincular a los usuarios con su número de alumno en una institución, tener sistema de calificaciones, tener un foro con notificaciones al mail asociado, entre otros.
* **Curso Público**:
 * Al ser este curso un público, no tendrá un registro importante de la información de un alumno, pero si tendrá un sistema de foro que permita interactuar a alumnos de diversas instituciones, una sección de material de estudio, otra sección en el que se propongan problemas para que los alumnos pongan a prueba sus capacidades y habilidades adquiridas, etc.

### Secundarias
* **Opcional**:
 * Sistema de login sincronizado con el de las instituciones o cuentas en redes sociales o Gmail.
 * Sistema de escritura látex para publicar preguntas o material directo en la web y no mediante pdf.
 * Sistema de videos, que permitan subir material audiovisual o incluso clases en línea.


# Entregas

Se evaluará el **último commit antes del plazo límite** en la branch `master`. 

## Entrega 1
> Plazo hasta: Domingo 19 de abril a las 23:59

Para esta entrega se necesita que al menos estén las entidades **creadas** y **bien relacionadas**. También deben estar al menos las vistas `index.html`, `show.hml`, `edit.html` y `new.html` de los modelos (que las necesiten), para esto necesitan tener lo básico de los ``controllers`` y las ``routes``.

#### Requerimientos:
* Modelos de las clases que satisfagan los requerimientos de su aplicación.
    * Migraciones bien hechas
    * Clases relacionadas
    * Desde un punto de vista OOP, los métodos/funciones
        * Por ejemplo, *que los usuarios tengan un método para agregar a otro usuario como amigo.* 
* Controllers, vistas y rutas
    * Al menos `index.html` y `show.hml`. Con sus métodos respectivos en los controllers y las rutas para poder acceder a estos.
    * Las vistas para poder crear y modificar entidades del modelo. 
* Se deben crear `seeds` suficientes para poder apreciar a estas vistas con contenido. 
* **Se busca el esqueleto de la aplicación.**
    * Se recomienda usar los generadores de Rails.

#### No es necesario
* No es necesario que los métodos de los modelos se reflejen en las vistas ni controladores (por ahora).
* No es necesario que las `forms` sean complejas o con elementos *nested*. Esto se pedirá en detalle cuando se manejen mejor los permisos y se pidan vistas más completas. 
* No es necesario que queden perfectas las relaciones, puede que después las tengan que mejorar. Asegúrense de hacer bien las migraciones para no tener problemas en un futuro.
* No es necesario un diseño. Basta solo el esqueleto en HTML.
* No es necesario el manejo de permisos (administradores, profesores o alumnos); ni sistemas de login. 


-------------

## Entrega 2
> Plazo hasta: Martes 19 de mayo a las 23:59

#### Requerimientos comunes

Para esta entrega se necesita que todos los proyectos tengan:

* Validaciones en los modelos.

* Frontend:
    * Una página de inicio que sea navegable y que permita acceder a los recursos.
    * Flujo de navegación. Es decir, poder recorrer la página a través de *links*.
    * Estilo:
        * Respetar **buenas prácticas** de CSS.
        * Separar el estilo de la estructura de la página.
        * Intentar que se vea lo *"menos scaffold posible"*.
        * No se espera un diseño espectacular. 
            * Sin embargo, los entusiastas serán bien recibidos.
        
* Sesiones de usuario:
    * Tener la capacidad de poder registrar usuarios. 
        * Usar gema: [bcrypt-ruby](https://github.com/codahale/bcrypt-ruby).
    * El usuario debe poder modificar sus datos.
    * El usuario debe poder cerrar sesión.
    * El usuario debe poder borrar su cuenta.
    * Contar con las vistas necesarias para estos puntos.

        > **Claramente** un usuario no debe poder modificar los datos de otros usuarios o recursos que no le correspondan. **Esto se debe cuidar a nivel interno de la aplicación como en las vistas.**

* Testing:
    * Usar **[RSpec](https://github.com/rspec/rspec-rails)** para realizar al menos 5 tests para funcionalidades relevantes y delicadas para la aplicación. Se deberá dejar una explicación de por qué se eligió testear 

        > **Por ejemplo**: validaciones, dependencias, manejo de excepciones, etc.
    * Documentación: [RSpec Rails 3.2](https://relishapp.com/rspec/rspec-rails/docs)

Es importante recordar que **están prohibidas** las gemas y frameworks como [Devise](https://github.com/plataformatec/devise) para el manejo de sesiones o [Bootstrap](http://getbootstrap.com/) (o similares) para el estilo. 

Se recomienda usar la capacidad de *anidar recursos* de Rails. Pueden leer más de esto en la documentación oficial: http://guides.rubyonrails.org/routing.html#nested-resources. También pueden revisar los [ejemplos subidos a Github](https://github.com/IIC2513-2015-1).

#### Requerimientos particulares

Para la **Plaraforma de cursos** se necesita que lo siguiente:

Deben estar creados los distintos roles de usuarios, recordar que hay administradores, profesores y alumnos. (se debe crear este administrador en el archivo "seed").

Los administradores deben tener la capacidad de crear cursos y asignar colaboradores. También deben tener la capacidad de moderar cursos.

Los profesores tienen que poder crear un curso con información relevante asociada al mismo, debe poder asignar colaboradores (ayudantes, por ejemplo). y finalmente asignar módulos al curso (Foro, sistema de cuestionarios, calificaciones, asistencia, repositorio de material).

Un alumno debe poder ingresar a ingresar a un curso privado y tener acceso a toda la información, si es que el alumno fue inscrito en el curso. Ademas un alumno debe poder acceder a cualquier curso público y hacer uso del contenido que este publicado.

##### En términos generales

Cualquier progreso adicional o funcionalidad extra que *agregue valor* a su aplicación es bienvenida. 

No duden en hacer preguntas al mail meiordac@uc.cl

#### No es necesario
* No es necesario que el *frontend* sea [responsivo](http://es.wikipedia.org/wiki/Dise%C3%B1o_web_adaptable).
* No es necesario que la aplicación esté montada en [Heroku](https://www.heroku.com/).
* No es necesario el uso de Javascript, pero pueden usarlo si lo necesitan.


-------------

## Entrega 3
> Plazo hasta: Domingo 14 de junio a las 23:59

#### Requerimientos comunes

Para esta entrega se necesita que todos los proyectos cumplan como mínimo:

* Su aplicación debe estar **montada** y **funcional** en **[Heroku](https://www.heroku.com/)**. 
    * Es necesario que se especifique la URL en el `README.md` de su proyecto.
* Implementar *Mailers* para enviarle *notificaciones* al usuario cuando suceda algo de importancia. Deben existir **al menos 5** acciones distintas que gatillen el envío de correo(s).
    * El correo enviado debe entregar detalles de la interacción. Por ejemplo, si es sobre algún comentario recibido, se debe informar quién fue el autor y el contenido. 
* Consumir alguna **API** externa gratuita pero que requiera registro por parte de los desarrolladores y que provea información de valor a su aplicación.
    * Al momento de montar la aplicación en Heroku se debe procurar que **en ningún momento el ayudante tenga acceso a su `API KEY`** cuando revise su repositorio. Es decir, no debe estar guardada como un *string* en su repositorio.
    * Es trabajo del grupo investigar cómo lograr esto y **debe indicar en el `README.md` cómo lo realizó.**
* Realizar *[scrapping](http://es.wikipedia.org/wiki/Web_scraping)* en algún sitio que provea otra información de valor para su aplicación.
    * Esto se debe hacer en alguna `rake task`,  durante alguna *request* o en el archivo `seed.rb`.
    * Una gema recomendada para esto es [Nokogiri](https://github.com/sparklemotion/nokogiri).
* Mediante el uso de **Javascript** y **AJAX** mejorar la experiencia del usuario (puede usar [JQuery](https://github.com/jquery/jquery)). Se pide **al menos** implementar:
    1.  Validar los formularios de creación de usuarios (por ejemplo, no permitir una *primary key* repetida).
    1. Realizar alguna acción entre usuarios, como *"seguir"*, *"agregar a amigos"* o algo equivalente en su aplicación.
    1. Realizar alguna acción con algún recurso, como *"like"*, *"comentar"* o algo equivalente en su aplicación.
* Permitir que los usuarios puedan subir imágenes a la aplicación.
    * **Al menos** dar la posibilidad de subir imagen de perfil y alguna imagen para algún recurso que ellos creen/administren, etc.
    * Se recomienda usar la gema [paperclip](https://github.com/thoughtbot/paperclip).


#### Requerimientos particulares

* Se debe implementar en el *frontend* de la aplicación al menos una vista con un mapa interactivo. Queda a criterio suyo qué servicio usar, cómo usarlo y si va usar alguna gema para eso o no. El mapa no satisface el [requerimiento común](#requerimientos-comunes) de *Consumir alguna API externa*.

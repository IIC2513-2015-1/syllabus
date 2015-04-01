# Plataforma de cursos

### Tabla de contenidos
* [Proyecto](#proyecto)
  * [Visión General](#vision-general)
  * [Funcionalidades](#funcionalidades)
    * [Principales](#principales)
    * [Secundarias](#secundarias)

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
> Plazo hasta: 15 de abril a las 23:59

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




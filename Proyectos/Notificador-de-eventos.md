# Notificador de Eventos

### Tabla de contenidos
* [Proyecto](#proyecto)
  * [Visión General](#vision-general)
  * [Funcionalidades](#funcionalidades)
    * [Principales](#principales)
    * [Secundarias](#secundarias)
* [Entregas](#entregas)
	* [Entrega 1](#entrega-1)
	* [Entrega 2](#entrega-2)
    
# Proyecto

## Vision General
> Idea original de: Grupo 5
  
El principal objetivo de aplicación será informar sobre los eventos culturales de manera geográfica en Santiago. 
La idea es poder ser notificado de actividades como:
* Conferencias
* Seminarios
* Trekkings
* Corridas

La meta es obtener de manera automática o manual las fechas y características relevantes de eventos desde las páginas
web organizadoras. También existirá un sistema de moderadores que anuncien los eventos y de esta forma, mantener la información
disponible para el usuario, lo más actualizada posible. La cultura y educación son importantes en la sociedad y muchas veces hay personas que
no están informados de eventos que son incluso gratuitos donde todos pueden ser capaces de aprender algo
nuevo o disfrutar un concierto.

Cabe destacar que las funcionalidades descritas a continuación funcionan como una guía pero de ninguna forma se quiere truncar la creatividad del alumno.
Si este quiere cambiar alguna funcionalidad o feature de la aplicación, puede hacerlo, la única condición es que sea aceptado por su tutor.

## Funcionalidades

A grandes razgos, el proyecto debe cumplir con los siguientes requerimientos.

### Principales
* **Navegación**
  * **Página de Inicio**: Deberá contar con un display de eventos personalizado (o aleatorio en caso de ser un usuario no loggeado)
  * **Barra de Navegación**: Las funcionalidades de esta quedan a criterio del alumno pero se aconseja basarse en página populares.
  * **Ranking de acontecimientos importantes**: Este deberá mostrar los eventos que estén ganando popularidad (dentro y fuera de las preferencias del usuario)
  * **Vistas por roles**: Se deberá marcar la diferencia visualmente entre usuarios que cumplan distintos roles.

* **Los usuarios podrán**:
	* **Crear cuentas**:
		* Administrar su información pública y la privada (lo que quieren o no mostrar)
		* Tener una imagen de perfil
		* Los campos de la cuenta de cada usuario deberán ser flexibles:
		  * Nombre
		  * Email
		  * Guardar preferencias (i.e las categorías de eventos sobre las que le gustaría recibir información)
		  * Otros (cualquiera que quiera agregar)
	  * Adquirir un rol dentro de la plataforma, estos podrán ser:
		  * Usuario normal
		  * Usuario moderador (este debe incluir permiso de otro moderador)
		  * Administrador general
		  * (Puede incluir otros roles si considera necesario)
	* **Crear y subscribirse a eventos**:
		* Buscar y filtrar eventos
		* Enviar emails y notificaciones sociales (Facebook, Twitter, etc) a usuarios subscritos a los eventos.
		* Crear sección de discusión (administrable por el creador del evento) aquí el usuario podrá:
	    *Calificar comentarios como relevantes
	    *Notificar comportamientos incorrectos a usuarios moderadores
		* Los eventos deben poder ser actualizados (esto incluye crear administradores nuevos o restricciones como: sólo para mayores de edad)
	* **Alertas grupales**
		* Crear alertas para grupos que cumplan con pertenecer a sus preferencias
		* Los usuarios podrán desligarse de las alertas en cualquier momento
		* Los usuarios deberán ver sus alertas cuando ingresen a la plataforma inmediatamente
	* **Mensajería**
		* Los usuarios deberán poder comunicarse con otros usuarios
		* Se deberán definir distintos permisos para los distintos roles de la aplicación
		* Se deberá poder bloquear la comunicación con ciertos usuarios
		* Los administradores recibirán por este medio si hay acusaciones de mal comportamiento
		
* Es importante que los **Eventos** tengan:
	* Nombre
	* Dirección
	* Dirección o coordenadas
	* Geolocalización
* Es importante que las **Alertas grupales** tengan:
	* Título
	* Descripción
	* Un lugar donde ocurrirán
	* Organizador(es)
	
### Secundarias
* Se deberá contar con interacción entre redes sociales (Facebook ,Youtube, etc).
* Se deberá poder subir videos y fotos por evento.
* Se podrá resumir experiencias de los usuarios que hayan asistido a eventos, combinando fotos que compartan o archivos en general.


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

Para la **Notificador de Eventos** se necesita que lo siguiente:

Los usuarios deben poder adquirir roles dentro de aplicación. Estos roles deberán ser validados por un administrador y por creadores de eventos (se debe crear este administrador en el archivo "seed"). 

Los usuarios deben poder crear y subscribirse a **eventos** quí deberán poder comentarios, calificar, marcar asistencia, etc. Deben estar presentes, funcionales y visibles los privilegios de organizadores.

Los usuarios deben poder crear **alertas**. Estas deberán incluir el email de los usuarios (esto para el desarrollo futuro) y los usuarios deberán ser capaces de salirse de estas alertas. También se requiere que hayan relaciones por interes entre los usuarios (eso implica ciertos privilegios como poder contactar gente de tu mismo interpes).

##### En términos generales

Cualquier progreso adicional o funcionalidad extra que *agregue valor* a su aplicación es bienvenida.

No duden en preguntarme cosas al mail: dnpena@uc.cl

#### No es necesario
* No es necesario que el *frontend* sea [responsivo](http://es.wikipedia.org/wiki/Dise%C3%B1o_web_adaptable).
* No es necesario que se puedan subir imágenes. Por ejemplo: de perfil.
* No es necesario que la aplicación esté montada en [Heroku](https://www.heroku.com/).
* No es necesario el uso de Javascript, pero pueden usarlo si lo necesitan.

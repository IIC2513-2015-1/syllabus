# Central de eventos

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
> Idea original de: Grupo 7

Consiste en hacer una aplicación para **difundir eventos culturales** tales como:
* Obras de teatro
* Tocatas
* Ferias
* Exposiciones

La idea es facilitar la labor de las productoras en cuanto a difundir sus eventos, y también centralizar la búsqueda de este tipo de actividades para los usuarios.

## Funcionalidades

A grandes razgos, el proyecto debe cumplir con los siguientes requerimientos.

### Principales
* **Los usuarios podrán**:
	* **Cuentas**:
		* Crear una cuenta con un perfil público
		* Tener una imagen de perfil
		* Poder modificar sus datos
			* Nombre
			* Imagen de perfil
			* Contacto (sea email o teléfono... o fax)
			* Otros datos que considere importantes
		* Borrar su cuenta
		* Seguir a otros usarios
	* **Eventos**:
		* Inscribirse a un evento
		* Buscar y filtrar eventos
		* Anotar las fechas donde pretenden salir
		* Anotar las categorías de los eventos que les interesen. 
		* Notificar por medio de email al usuario cuando un evento cumple su criterio
		* Calificar a los eventos actuales y pasados como:
			* Genuinos / Fraudulentos
			* Buen o mal evento
		* Comentar eventos actuales y pasados
		* Notificar al usuario si un evento que ha calificado positivamente se repite
		* Ser notificado cuando un usuario al que sigue cree un evento
		* Crear eventos, en tal caso se convierte en "organizador"
		* Los organizadores del evento deben:
			* Poder modificar los datos del evento
			* Poder asignar o remover organizadores
			* Poder configurar si los organizadores pagan o no
	* **Lugares**
		* Crear lugares y quedar como dueño.
		* Hacerse fan de un lugar
		* Poder ver los eventos que han ocurrido y ocurrirán en el lugar
		* Calificar al lugar como:
			* Genuino / Fraudulento
			* Buen o mal lugar 
		* Los dueños del lugar deben:
			* Poder modificar los datos del lugar
			* Poder asignar o remover dueños
	* **Grupos**
		* Crear grupos
		* Unirse a grupos
		* Dejar grupos
		* Tener o no permisos de administrador, en caso de ser administrador:
			* Dar o no permisos de administrador a otros usuarios
			* Crear eventos donde el grupo será el organizador
			* Crear lugares donde el grupo será el dueño
* Es importante que los **lugares al menos tengan**:
	* Nombre
	* Dirección
	* Dirección o coordenadas
	* Dueño(s)
* Es importante que los **eventos al menos tengan**:
	* Título
	* Descripción
	* Precio (si es que son pagados)
	* Hora de inicio y término
	* Un lugar donde ocurrirán
	* Organizador(es)
* Se debe poder acceder a eventos a través de los perfiles de los lugares y grupos.
* **Es importante que haya al menos una vista con un mapa para poder ver los eventos.**

### Secundarias
* Se puede tener un sistema para difundir en las distintas **redes sociales** existentes.
* Se pueden incluir **cupones** de descuento en la misma aplicación. Estos podrán ser limitados o no.
* Se puede tener un sistema de **achievements** que otorgue premios a los usuarios que:
	* Ayuden a difundir una cierta cantidad de eventos.
	* Asistan a una determinada cantidad de eventos
		* Adicionalmente, si tomó **la mejor ruta** (la más corta) para llegar a todos esos eventos, se gana un **perfil Gold**. 


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

Para la **Central de Eventos** se necesita que lo siguiente:

Los usuarios deben poder seguir a otros usuarios. También debe estar la opción *dejar de seguir*. Que requiera confirmación del otro usuario queda a criterio de ustedes.

Los usuarios deben poder crear **eventos** e interactuar con ellos con comentarios, calificaciones, marcar asistencia, etc. Deben estar presentes, funcionales y visibles los privilegios de organizados en los eventos donde sean organizadores.

Los usuarios deben poder crear **lugares**. También se requiere que ellos puedan ver en los lugares los eventos que ocurrirán o han ocurrido allí. Recordar que los usuarios pueden ser dueños de un local y eso implica ciertos privilegios. Además recordar que los usuarios pueden calificar estos lugares. 

Deben estar presentes las funcionalidades correspondiente a los **grupos** y las interacciones de los usuarios a estos.

##### En términos generales

Cualquier progreso adicional o funcionalidad extra que *agregue valor* a su aplicación es bienvenida. 

#### No es necesario
* No es necesario que el *frontend* sea [responsivo](http://es.wikipedia.org/wiki/Dise%C3%B1o_web_adaptable).
* No es necesario que se puedan subir imágenes. Por ejemplo: de perfil.
* No es necesario que la aplicación esté montada en [Heroku](https://www.heroku.com/).
* No es necesario el uso de Javascript, pero pueden usarlo si lo necesitan. 


-------------

## Entrega 3
> Plazo hasta: Miércoles 17 de junio a las 23:59

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

* Se debe implementar en el *frontend* de la aplicación al menos una vista con un mapa interactivo. Queda a criterio suyo qué servicio usar, cómo usarlo y si va usar alguna gema para eso o no. Esta vista no satisface el [requerimiento común](#requerimientos-comunes) de *Consumir alguna API externa*.

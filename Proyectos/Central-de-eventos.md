# Central de eventos

### Tabla de contenidos
* [Proyecto](#proyecto)
  * [Visión General](#vision-general)
  * [Funcionalidades](#funcionalidades)
    * [Principales](#principales)
    * [Secundarias](#secundarias)
* [Entregas](#entregas)
	* [Entrega 1](#entrega-1)

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


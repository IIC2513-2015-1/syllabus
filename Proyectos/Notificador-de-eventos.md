# Notificador de Eventos

### Tabla de contenidos
* [Proyecto](#proyecto)
  * [Visión General](#vision-general)
  * [Funcionalidades](#funcionalidades)
    * [Principales](#principales)
    * [Secundarias](#secundarias)
    
# Proyecto

## Vision General
> Idea original de: Grupo 7
  
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

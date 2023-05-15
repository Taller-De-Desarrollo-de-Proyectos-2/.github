# Qatabum: Álbum Qatar 2022 - Taller de Desarrollo de Proyectos 2 - Grupo 03

## https://qatabum.herokuapp.com

Conjunto de repositorios para Qatabum - Trabajo práctico de Taller De Desarrollo de Proyectos II - 2C 2022 - Facultad de Ingeniería - Universidad de Buenos Aires (UBA)

<img src="https://github.com/Taller-De-Desarrollo-de-Proyectos-2/.github/assets/6344343/c1435b3a-c93c-4686-9a6a-00204295202c" width="800"></img>

## Descripción

Qatabum es una aplicación web responsive para escritorio y dispositivos móviles con fines académicos, cuya función principal es la de servir como álbum digital de figuritas para el mundial de fútbol Qatar 2022. Consta de una app web responsive principal y otra de backoffice, ambas desarrolladas con Flutter en frontend.

## Funcionalidades principales
- 4 países disponibles (grupo de Argentina)
- Biblioteca de figuritas del usuario para pegar en álbum y para intercambiar
- Apertura de nuevos paquetes de figuritas
- Obtención de paquetes diarios de regalo
- Visualización y edición de perfil
- OAuth login con Google Sign-in 
- Comunidades de usuarios para intercambio de figuritas y chat
- Creación y aceptación de solicitudes de intercambio de figuritas entre usuarios
- Pegado de figuritas en álbum y navegación realista por el mismo
- Vista mobile con diseño para orientación horizontal.

### Administrador (backoffice)
- Reportes varios de la plataforma (usuarios, completitud de álbumes, top figuritas más frecuentes, etc.)
- Listado y gestión de comunidades (bloqueos, filtros, etc.)

## Características técnicas y tecnologías principales

- Python / FastAPI (servicios de backend)
- Flutter (app Android & frontend backoffice web)
- PostgreSQL (bases de datos no-multimedia)
- Firebase Authentication OAuth (google login)
- Firebase Storage (multimedia -imágenes y audio-)
- Firebase Database (chat de comunidades)
- CI/CD mediante Github Actions
- Heroku cloud

### Arquitectura de alto nivel

<img src="https://github.com/Taller-De-Desarrollo-de-Proyectos-2/.github/assets/6344343/e1572f3f-3703-466d-8282-d1c583ffea45" width="600"></img>

## Showcase

<details>
  <summary>Qatabum web app</summary>
  <img src="https://github.com/Taller-De-Desarrollo-de-Proyectos-2/.github/assets/6344343/2cfa70d7-c4f6-4d32-a991-fa68d000877f" width="900"></img>
  <img src="https://github.com/Taller-De-Desarrollo-de-Proyectos-2/.github/assets/6344343/cf6140a1-7a69-4dff-a790-a2a6b5bf9577" width="900"></img>
  <img src="https://github.com/Taller-De-Desarrollo-de-Proyectos-2/.github/assets/6344343/2523b3ca-7950-4895-8ffd-2804c119809c" width="900"></img>
  <img src="https://github.com/Taller-De-Desarrollo-de-Proyectos-2/.github/assets/6344343/c6959f47-5981-4a43-a05e-93492b3ff649" width="900"></img>
  <img src="https://github.com/Taller-De-Desarrollo-de-Proyectos-2/.github/assets/6344343/25996442-95fe-46fd-9255-8a637be57648" width="900"></img>
  <img src="https://github.com/Taller-De-Desarrollo-de-Proyectos-2/.github/assets/6344343/46c4ecf1-fe10-4b81-9bdb-4abc26191895" width="900"></img>

</details>

<details>
  <summary>Backoffice web app</summary>
</details>

## Enunciado/idea preliminar original del TP

<details>
  <summary>Preliminar de proyecto del cliente. TP 2C 2022</summary>

> ## Trabajo Práctico 75.47 – Taller de desarrollo de proyectos 2 - FIUBA – 2do cuat. 2022

> ### Álbum de figuritas Qatar 2022

> El grupo de inversores digitales MAMOAL contrató a nuestra empresa para desarrollar y entregar al fin de este cuatrimestre la versión MVP del álbum de figuritas digitales para el mundial de Qatar 2022. A futuro se espera poder expandir el mismo a diferentes campeonatos de diversos países con versiones más completas. 

> El equipo de producto detectó que los siguientes puntos deberían formar parte de ese entregable:

> Para ingresar se requerirá un acceso con Facebook/Twitter/Google válido. Luego ingresará en la home donde se puede acceder a secciones principales como: Ver el álbum, Mis figus, Paquetes, Perfil, Comunidad, etc.

> La sección Perfil permite establecer: nombre, email, fecha de nacimiento, país e idioma además del alias y países favoritos. Tener el perfil completo da como beneficio la recepción de 3 paquetes de figuritas gratis. Además en el perfil se deberá visualizar el porcentaje de álbum completo,  la cantidad de figuritas coleccionadas y la cantidad de intercambios realizados.

> Hasta no tener completado el perfil no se podrá intercambiar figuritas ni pertenecer a una comunidad. La cantidad de intercambios una vez habilitados es de un máximo de 3 por día.

> Con respecto a los Paquetes, por día se puede solicitar dos gratis. Si no se ingresa a la plataforma ese día, se pierden. Adicionalmente cada día se podrán comprar hasta 5 paquetes adicionales.

> Al abrir el paquete se mostrarán las 5 figuritas que contiene el paquete. Se destacarán las figuritas que el usuario no posee y se puede ir al álbum para proceder a pegarlas. 
> Al terminarse los sobres y la posibilidad de comprar más deberá mostrar una cuenta regresiva hasta la hora en que pueda quedar habilitado para solicitar nuevos paquetes.

> En la sección Mis figus, el usuario almacena las figuritas que posee y puede seleccionarlas para pegarlas en el álbum.  Se pega haciendo click en la figurita, se abre el álbum en la posición donde hay que pegarlo y haciendo click en dicha posición se pega la misma con una animación. Las otras figuritas se pueden poner en la fila de repetidas.
> Las figuritas repetidas se pueden intercambiar en alguna de las comunidades a las que pertenece el usuario

> El usuario se puede unir a una comunidad de hasta 10 amigos, o crear una nueva. Para unirse a una comunidad existente debe contar con la clave de acceso. Para crear una comunidad nueva lo debe hacer con nombre único, una clave y una descripción. 
> El usuario podrá pertenecer hasta en 10 comunidades.

> Para la primera versión se espera que el álbum esté en condiciones de salir a producción con los países de la zona de Argentina. 
> Se deberá alentar a los usuarios a compartir su álbum en las redes sociales con una invitación a jugar. Cada usuario referido tendrá un paquete de premios.

> ### Backoffice administrativo:

> Deberá existir un backoffice administrativo que permita a un operador disponer de:

> #### Un administrador de figuritas:

> Se podrá administrar número, imagen y ponderación para ver con qué frecuencia aparecerá. 
> - Ponderación: de 1 más fácil a 5 la más difícil.

> #### Armar paquetes:

> Cada 10 paquetes que se arman debe aparecer:
> - 1 → ponderación 5
> - 2 → ponderación 1
> - 2 → ponderación entre 2 y 4
> Entre los 10 otros paquetes deben aparecer:
> - 5 → entre ponderación 1 y 3

> #### Gestión de comunidades:

> Se podrán observar las comunidades existentes y podrán bloquear/activar las mismas. Si se bloquea deberá aparecer un mensaje a los integrantes del mismo.

> #### Reportes:

> Reporte de usuarios registrados.
> Reportes de paquetes entregados y vendidos
> Otros reportes

</details>

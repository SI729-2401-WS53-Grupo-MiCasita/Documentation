
# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management
En este apartado se resume todo el contenido recopilado, examinando los procedimientos a seguir y evaluando el estado emocional.
### 5.1.1. Software Development Environment Configuration
En la siguiente sección se detalla la ruta de acceso de cada uno de los productos de software, facilitando a cualquier miembro del equipo el desarrollo de cada aspecto del trabajo:
* **Visual Studio Code:** Entorno de desarrollo.\
![image](https://hackmd.io/_uploads/Hy8d2y7lR.png)
* **HTML5:** Lenguaje de marcado para la elaboración de páginas web.\
![image](https://hackmd.io/_uploads/BJYDn17l0.png)
* **CSS3:** Tecnología para dar estilo a nuestras páginas web.\
![image](https://hackmd.io/_uploads/B1gDhkXgC.png)
* **JavaScript:** Lenguaje de programación orientado a objetos utilizado para implementar funcionalidades en nuestra Landing Page.\
![image](https://hackmd.io/_uploads/SJLU317xC.png)
* **GitHub:** Repositorio colaborativo en la nube.\
![image](https://hackmd.io/_uploads/ryiVhJXxC.png)
* **GitHub Pages:** Plataforma que facilita implementar despliegues sencillos para nuestras páginas web.\
![image](https://hackmd.io/_uploads/HyIQnyXgR.png)
* **LucidChart:** Aplicación web dedicada a la elaboración de Wireflows, User Flows y diagramas de clases.\
![image](https://hackmd.io/_uploads/H1QG2JXeC.png)

* **Vertabelo:** Plataforma colaborativa para la creación de diagramas de base de datos.\
![image](https://hackmd.io/_uploads/r1BjjyQgC.png)
* **Figma:** Herramienta colaborativa que permite elaborar wireframes y mockups.\
![image](https://hackmd.io/_uploads/BJ99okXeR.png)
### 5.1.2. Source Code Management
**Repositorio de la Landing Page:** 
**Implementación de GitFlow:**
Para nuestra estrategia de gestión de versiones con Git, nos hemos inspirado en el artículo "A successful Git branching model" de Vincent Driessen, adoptando el modelo de ramificación GitFlow. Este enfoque nos permite establecer claramente las convenciones de ramificación que aplicamos en nuestro proyecto.
![image](https://hackmd.io/_uploads/rJt95BobA.png)
* **Rama Principal (Main branch):** Contiene el código en producción y se conoce como la Master branch o Main branch.
    * Notación: main
* **Rama de Desarrollo (Develop branch):** Acumula las últimas actualizaciones y cambios para la próxima versión. Funciona como un entorno de integración y prueba continua.
    * Notación: develop
* **Rama de Lanzamiento (Release branch):** Facilita la preparación de una nueva versión del producto, permitiendo correcciones de errores y recibiendo más actualizaciones de Develop.
    * Debe derivarse de: develop
    * Debe fusionarse con: develop y master/main
    * Notación: release
* **Rama de Características (Feature branch):** Se utiliza para desarrollar nuevas funcionalidades para la siguiente versión o futuras iteraciones.
    * Debe derivarse de: develop
    * Debe fusionarse de vuelta a: develop
    * Notación: feature
* **Rama de Corrección Rápida (Hotfix branch):** Aborda errores críticos en producción, permitiendo la implementación rápida de soluciones.
    * Debe derivarse de: master/main
    * Debe fusionarse con: develop y master/main
    * Notación: hotfix

**Conventional Commits:** 
Adoptamos esta metodología para estructurar los mensajes de confirmación de cambios de manera estándar y semántica, lo que facilita la comunicación y la automatización de registros de cambios.
**Tipos de Commits Convencionales:**
* feat: Nuevas características o funcionalidades.
* fix: Correcciones de errores.
* docs: Cambios o mejoras en la documentación.
* style: Cambios de formato que no afectan la funcionalidad.
* refactor: Mejoras en la estructura o legibilidad del código.
* test: Adición o modificación de pruebas.
* chore: Cambios en el proceso de construcción o tareas de mantenimiento.
* perf: Mejoras de rendimiento en el código.
### 5.1.3. Source Code Style Guide & Conventions
En la redacción de nuestro código, hemos adoptado el uso exclusivo de la nomenclatura en inglés para todos los lenguajes mencionados.
**HTML**
* **Uso de minúsculas en elementos HTML:**
```html

<header>
  <nav>Navigation Menu</nav>
</header>
<!-- Cierre correcto de elementos HTML -->
<section>
  <article>This is an article</article>
  <article>This is another article</article>
</section>
```
* **Atributos en minúsculas:**
```html
<input type="text" placeholder="Enter your name">
```
* **Especificación de atributos para imágenes:**
```html
<img src="landscape.jpg" alt="A beautiful landscape" width="300" height="200">
```
**CSS**
* **Nombres significativos para ID y clases:**
```css
#main {}
#accessForm {}
.mainButton {}
```
* **Nombres cortos y descriptivos para ID y clases:**
```css
#menu {}
.userProfile {}
Uso de propiedades abreviadas en CSS:
margin: 10px 5px;
background: url('background.jpg') no-repeat center center;
```
* **Omisión de unidades después de cero:**
```css
margin: 0;
padding: 0;
Orden alfabético en las declaraciones CSS:
.content {
  align-items: center;
  display: flex;
  justify-content: space-between;
  padding: 20px;
}
```
**JavaScript**
* **Funciones con sintaxis expandida:**
```javascript
function updateCounter() {
  // Code to update the counter
}
```
* **Nombres de variables en lowercamelCase:**
```javascript
let visitCounter = 0;
let remainingTime = 120;
```
* **Uso de let y const en lugar de var:**
```javascript
const API_URL = 'https://api.example.com';
let operationResult = sum(5, 3);
function sum(a, b) {
  return a + b;
}
```
### 5.1.4. Software Deployment Configuration
En esta sección, detallamos el proceso de implementación de nuestra landing page en la plataforma de GitHub.

1. Se crea un repositorio en GitHub para alojar el código de nuestra landing page.

![image](https://hackmd.io/_uploads/SyNyy8obC.png)

2. Agregamos a los participantes:

![image](https://hackmd.io/_uploads/Bk4gJUoWR.png)

3. Habilitamos Github Pages en la rama principal “main” y ruta “/(root)”:

![image](https://hackmd.io/_uploads/S1vbJIoZC.png)

4. Finalmente, se confirma el despliegue de nuestra página web después de completar todo el procedimiento.


Este proceso garantiza el despliegue satisfactorio de nuestra landing page en la plataforma de GitHub, siguiendo las especificaciones y requisitos de nuestro proyecto.
**Enlace de la Landing Page: https://homeheavenly.github.io/MiCasita/**
## 5.2. Landing Page, Services & Applications Implementation

### 5.2.1. Sprint 1 
En este informe, se documenta el progreso realizado durante la fase de definición de requisitos del proyecto, que incluye entrevistas con los stakeholders y la creación de artefactos antes y durante la implementación de la aplicación web estática. El objetivo principal es proporcionar una visión clara del avance y garantizar una comunicación efectiva entre el equipo de desarrollo y los stakeholders.

Durante esta fase, se llevaron a cabo entrevistas exhaustivas con los stakeholders para comprender sus necesidades, expectativas y requisitos específicos para la aplicación. Estas entrevistas proporcionaron información valiosa que sirvió como base para la definición de los requisitos del proyecto.

Además de las entrevistas, se realizaron actividades de creación de artefactos antes y durante la implementación de la aplicación web estática. Estos artefactos incluyeron documentos de requisitos, prototipos de diseño y especificaciones técnicas, los cuales fueron iterados y refinados en función de la retroalimentación recibida durante el proceso.

La creación de la aplicación web estática se llevó a cabo con el objetivo de proporcionar a los stakeholders una vista preliminar del producto final y recopilar sus comentarios y sugerencias para su mejora. Esta versión inicial permitió a los visitantes tener una idea clara de la dirección del proyecto y proporcionó una plataforma para la retroalimentación temprana.

#### 5.2.1.1 Sprint Planning 1

| Sprint # | Sprint 1  | 
|--------------------|------------|
| Sprint Planning Background | 
| Date | 2024-04-04 | 
| Time |  10:00 AM |
| Location |  UPC - Campus San Miguel |
| Preparate by| Maycol Jhordan Rojas Velasquez | 
|  Attendees (to planning meeting) | -Abanto Vicente, Edery Renzo -Calderón Huamán, Jose Daniel Mario -Antonio Fretle, Jeremi Jose -Manco Cuellar, Anthony Ramon | 
| Sprint n-1 Review Summary | Se implementó correctamente el landing page estático. | 
| Sprint Planning Background | Durante esta etapa, se llevó a cabo una exhaustiva verificación de la funcionalidad de la landing page diseñada para el proyecto. El objetivo principal fue asegurar que la landing page cumpla con los estándares de calidad y proporcionar una experiencia ópptima para los visitantes. |
| Sprint Goal & User Stories | 
| Sprint 1 Goal | Desarrolar la funcionalidad de la página web con inicio de sesión. Se considerará que el objetivo del sprint se ha cumplido si todas las historias de usuario relacionadas con el registro de usuarios están implementadas y hecho con las entrevistas de segmentos objetivos.|  
| Sprint Velocity | Se establece un Velocity de 20 Story Points para este Sprint. | 
| Sum of Story Points | 20 Story Points | 

#### 5.2.1.2 Sprint  Backlog 1
| Epic / Story ID | Título | Descripción | 
|-----------------|--------|-------------|
| US001 | Página "Sobre" | Como visitante, quiero poder acceder a la página "Sobre" para obtener más información sobre la aplicación. |
| US002 | Página de Contacto | Como visitante, quiero poder acceder a la página de contacto para ponerme en contacto con el equipo de la aplicación. |
| US003 | Centro de Ayuda | Como visitante, quiero poder acceder al centro de ayuda para obtener asistencia con el uso de la aplicación. | 
| US004 | Registro de Nuevos Usuarios | Como visitante, quiero poder registrarme como usuario para acceder a todas las funcionalidades de la aplicación. |  
| US005 | Iniciar Sesión en la Aplicación | Como visitante, quiero poder acceder a mi cuenta de usuario existente para utilizar las funcionalidades de la aplicación. |  

<table align="center" border="1" width="90%" style="text-align:center">
 <tr>
    <td colspan="2"><b>User Story</b></td>
    <td colspan="6"><b>Work-Item / Task</b></td>
  </tr>
  <tr>
    <td><b>Id</b></td>
    <td><b>Title</b></td>
    <td><b>Id</b></td>
    <td><b>Title</b></td>
    <td><b>Estimation</b></td>
    <td><b>Assigned To</b></td>
    <td><b>Status(To-do/ In-Process/ To-Review/ Done)</b></td>
  </tr>
  <tr>
    <td>US001</td>
    <td>Página "Sobre"</td>
    <td>T01</td>
    <td>Registro de la página</td>
    <td>2</td>
    <td>Abanto Vicente, Edery Renzo</td>
    <td>To - do</td>
 </tr>
 <tr>
    <td>US002</td>
    <td>Página de Contacto</td>
    <td>T02</td>
    <td>Creación de la página</td>
    <td>3</td>
    <td>Rojas Velasquez, Maycol Jhordan</td>
    <td>To - do</td>
<tr>
    <td>US003</td>
    <td>Centro de Ayuda</td>
    <td>T04</td>
    <td>Visualizar el Centro de Ayuda</td>
    <td>3</td>
    <td>Rojas Velasquez, Maycol Jhordan</td>
    <td>To - do</td>
 </tr>
<tr>
    <td>US004</td>
    <td>Registro de Nuevos Usuarios</td>
    <td>T05</td>
    <td>Registro de Visitas</td>
    <td>5</td>
    <td>Calderón Huamán, Jose Daniel Mario</td>
    <td>To - do</td>
 </tr>
<tr>
    <td>US005</td>
    <td>Iniciar Sesión en la Aplicación</td>
    <td>T06</td>
    <td>Inicio de sesión en la aplicación</td>
    <td>3</td>
    <td>Manco Cuellar, Anthony Ramon</td>
    <td>To - do</td>
 </tr>
</table>

### 5.2.2. Sprint 2
En este informe, se detallan las correcciones realizadas en el informe completo, así como los puntos a trabajar para la elaboración de la primera versión de la aplicación web front-end "Mi Casita".

Durante la revisión del informe completo, se identificaron áreas que requerían correcciones y mejoras para garantizar la calidad y coherencia del documento. Estas correcciones abarcan aspectos como la claridad en la presentación de la información, la precisión de los datos y la cohesión del contenido.

Además de las correcciones realizadas, se han designado puntos específicos para trabajar en la elaboración de la primera versión de la aplicación web front-end "Mi Casita". Estos puntos incluyen aspectos como el diseño de la interfaz de usuario, la implementación de funcionalidades clave y la optimización del rendimiento del sitio web.

#### 5.2.2.1. Sprint Planning 2.

| Sprint # | Sprint 2  | 
|--------------------|------------|
| Sprint Planning Background | 
| Date | 2024-04-08 | 
| Time |  10:00 AM |
| Location |  UPC - Campus San Miguel |
| Preparate by| Maycol Jhordan Rojas Velasquez | 
|  Attendees (to planning meeting) | -Abanto Vicente, Edery Renzo -Calderón Huamán, Jose Daniel Mario -Antonio Fretle, Jeremi Jose -Manco Cuellar, Anthony Ramon | 
| Sprint n-1 Review Summary | Se realizó las correcciones de la landing page correctamente | 
| Sprint Planning Background | Durante la etapa anterior se desarrolló con complicaciones e ideas de los integrantes de manera coherente, y responsive. |
| Sprint Goal & User Stories | 
| Sprint 1 Goal | Desarrolar la funcionalidad de la página web con angular para poder desarrollar correctamente lo aprendido en clase.|  
| Sprint Velocity | Se establece un Velocity de 25 Story Points para este Sprint. | 
| Sum of Story Points | 25 Story Points | 

#### 5.2.2.2. Sprint Backlog 2
| Epic / Story ID | Título | Descripción | 
|-----------------|--------|-------------|
| US006        | Crear Usuario     | Como administrador, quiero poder agregar nuevos usuarios al sistema para permitirles acceder a las funcionalidades de la plataforma. 
| US 010        | Agregar Propiedad   | Como administrador, quiero poder agregar nuevas propiedades al sistema para ampliar el catálogo de opciones para los usuarios.                                               | **Escenario 1:** Agregar propiedad exitosamente <br> **Given** el administrador completa el formulario de propiedades con información válida <br> **When** hace clic en el botón de agregar propiedad <br> **Then** la propiedad se agrega al sistema y se muestra un mensaje de éxito. <br><br> **Escenario 2:** Error al agregar propiedad <br> **Given** el administrador completa el formulario con información inválida <br> **When** hace clic en el botón de agregar propiedad <br> **Then** el sistema muestra un mensaje de error y no agrega la propiedad. | EPIC003                     |
| US014        | Búsqueda por Filtros  | Como usuario, quiero poder filtrar propiedades según diferentes criterios (precio, ubicación, tamaño, etc.) para refinar mi búsqueda.                                             | **Escenario 1:** Búsqueda exitosa con filtros <br> **Given** el usuario está en la página de búsqueda <br> **When** aplica filtros de búsqueda <br> **Then** se muestran las propiedades que coinciden con los criterios seleccionados. <br><br> **Escenario 2:** Sin resultados con filtros <br> **Given** el usuario está en la página de búsqueda <br> **When** aplica filtros de búsqueda que no tienen resultados <br> **Then** se muestra un mensaje indicando que no hay propiedades que coincidan con los criterios seleccionados. | EPIC004                    |                    |
| US018        | Reservar Cita para Ver Propiedad          | Como usuario, quiero poder reservar una cita para ver una propiedad seleccionando una fecha y hora disponibles, para confirmar mi interés en la propiedad. | **Escenario 1:** Reserva exitosa de cita <br> **Given** el usuario está en la página de detalles de la propiedad <br> **When** selecciona una fecha y hora disponibles <br> **Then** se guarda la cita en el sistema y se muestra un mensaje de confirmación. <br><br> **Escenario 2:** Error al reservar cita <br> **Given** el usuario está en la página de detalles de la propiedad <br> **When** intenta reservar una cita en una fecha y hora no disponibles <br> **Then** se muestra un mensaje de error y no se guarda la cita. | EPIC005                    |
| US006        | Crear Usuario     | Como administrador, quiero poder agregar nuevos usuarios al sistema para permitirles acceder a las funcionalidades de la plataforma.                                                  | **Escenario 1:** Creación exitosa de usuario <br> **Given** el administrador completa el formulario con datos válidos <br> **When** hace clic en el botón de crear usuario <br> **Then** el sistema crea el usuario y muestra un mensaje de éxito. <br><br> **Escenario 2:** Error en la creación de usuario <br> **Given** el administrador completa el formulario con datos inválidos <br> **When** hace clic en el botón de crear usuario <br> **Then** el sistema muestra un mensaje de error y no crea el usuario. | EPIC002                     |
| US007        | Ver Usuarios      | Como administrador, quiero poder ver una lista de todos los usuarios registrados en el sistema para supervisar la base de usuarios.                                                   | **Escenario 1:** Visualización de la lista de usuarios <br> **Given** el administrador está en la página de administración de usuarios <br> **When** accede a la lista de usuarios <br> **Then** el sistema muestra una lista de todos los usuarios registrados. <br><br> **Escenario 2:** No hay usuarios registrados <br> **Given** el administrador está en la página de administración de usuarios <br> **When** no hay usuarios registrados <br> **Then** el sistema muestra un mensaje indicando que no hay usuarios registrados. | EPIC002                    |
| US008        | Actualizar Usuario | Como administrador, quiero poder actualizar la información de un usuario existente en el sistema para corregir datos incorrectos o desactualizados.                                 | **Escenario 1:** Actualización exitosa de la información del usuario <br> **Given** el administrador está en la página de detalles del usuario <br> **When** modifica la información del usuario <br> **Then** el sistema guarda los cambios y muestra un mensaje de éxito. <br><br> **Escenario 2:** Error en la actualización de la información del usuario <br> **Given** el administrador está en la página de detalles del usuario <br> **When** intenta modificar la información del usuario con datos inválidos <br> **Then** el sistema muestra un mensaje de error y no guarda los cambios. | EPIC002                    |
| US009        | Eliminar Usuario  | Como administrador, quiero poder eliminar un usuario del sistema si ya no es necesario o si incumple las políticas de la plataforma.                                                   | **Escenario 1:** Eliminación exitosa de usuario <br> **Given** el administrador está en la página de detalles del usuario <br> **When** confirma la eliminación del usuario <br> **Then** el sistema elimina al usuario y muestra un mensaje de confirmación. <br><br> **Escenario 2:** Cancelar eliminación de usuario <br> **Given** el administrador está en la página de detalles del usuario <br> **When** cancela la eliminación del usuario <br> **Then** el sistema no elimina al usuario y vuelve a la página de detalles del usuario. | EPIC002

<table align="center" border="1" width="90%" style="text-align:center">
 <tr>
    <td colspan="2"><b>User Story</b></td>
    <td colspan="6"><b>Work-Item / Task</b></td>
  </tr>
  <tr>
    <td><b>Id</b></td>
    <td><b>Title</b></td>
    <td><b>Id</b></td>
    <td><b>Title</b></td>
    <td><b>Estimation</b></td>
    <td><b>Assigned To</b></td>
    <td><b>Status(To-do/ In-Process/ To-Review/ Done)</b></td>
  </tr>
  <tr>
    <td>US001</td>
    <td>Crear Usuario</td>
    <td>T01</td>
    <td>Creación de Usuario</td>
    <td>5</td>
    <td>Abanto Vicente, Edery Renzo</td>
    <td>in Process</td>
 </tr>
 <tr>
    <td>US002</td>
    <td>Agregar Propiedad</td>
    <td>T02</td>
    <td>Agregación de propiedad</td>
    <td>5</td>
    <td>Rojas Velasquez, Maycol Jhordan</td>
    <td>in Process</td>
<tr>
    <td>US003</td>
    <td>Búsqueda por filtros</td>
    <td>T04</td>
    <td>Búsqueda por filtros</td>
    <td>5</td>
    <td>Antonio Fretle, Jeremi Jose</td>
    <td>in Process</td>
 </tr>
<tr>
    <td>US004</td>
    <td>Reservar Cita para ver propiedad</td>
    <td>T05</td>
    <td>Reserva de citas</td>
    <td>4</td>
    <td>Calderón Huamán, Jose Daniel Mario</td>
    <td>in Process</td>
 </tr>
<tr>
    <td>US005</td>
    <td>Ver mis citas reservadas</td>
    <td>T06</td>
    <td>Citas guardadas</td>
    <td>4</td>
    <td>Manco Cuellar, Anthony Ramon</td>
    <td>in Process</td>
 </tr>
</table>

#### 5.2.2.3 Development Evidence for Sprint Review
<table>
    <thead>
        <tr>
            <th>Repository</th>
            <th>Branch</th>
            <th>Commit ID</th>
            <th>Commited on (Date)</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>HomeHeavenly/MiCasita</td>
            <td>dev</td>
            <td>feat: Add user task matrix to report</td>
            <td>Apr 28, 2024</td>
        </tr>
        <tr>
            <td>HomeHeavenly/MiCasita</td>
            <td>dev</td>
            <td>feat: Add user person to images</td>
            <td>Apr 27, 2024</td>
        </tr>
        <tr>
            <td>HomeHeavenly/MiCasita</td>
            <td>dev</td>
            <td>feat: Añadir información de entrevista sobre búsqueda de alojamiento</td>
            <td>Apr 28, 2024</td>
        </tr>
        <tr>
            <td>HomeHeavenly/MiCasita</td>
            <td>dev</td>
            <td>feat: add Impact Mapping</td>
            <td>Apr 27, 2024
</td>
        </tr>
    </tbody>
</table>

#### 5.2.2.4 Testing Suite Evidence for Sprint Review
Durante este primer sprint, hemos implementado todas las funcionalidades definidas en nuestro Sprint Backlog, asegurándonos de cumplir con sus criterios de aceptación correspondientes.\
#### 5.2.2.5 Execution Evidence for Sprint Review
Durante el primer sprint, el equipo de desarrollo de HomeHeavenly completó la creación de la Landing Page para nuestro proyecto MiCasita. En nuestro sitio web, los usuarios pueden acceder a información sobre las casas en alquiler, conocernos mejor, contactarnos, comentarios y encontrar respuestas a las preguntas más frecuentes.\
<img src="../assets/im1.png"/>
<img src="../assets/im2.png"/>
<img src="../assets/im3.png"/>
<img src="../assets/im4.png"/>
<img src="../assets/im5.png"/>

#### 5.2.2.6 Services Documentation Evidence for Sprint Review
Hasta ahora, no disponemos de documentación de nuestros servicios, ya que este primer sprint se ha centrado en el desarrollo de la Landing Page.
#### 5.2.2.7 Software Deployment Evidence for Sprint Review
Para empezar a trabajar en la implementación de la Landing Page, primero configuramos el repositorio en Github, creando las ramas principales necesarias: main, developer y features.\
![image](https://hackmd.io/_uploads/ByJqBFYxC.png)
Una vez establecido, cada miembro del equipo cargó su parte del proyecto al repositorio, colaborando de manera eficiente en el desarrollo.
![image](https://hackmd.io/_uploads/BJ5sSKKxA.png)
Por último, para mostrar nuestro progreso, desplegamos el proyecto en la rama main utilizando la herramienta GitHub Pages.
![image](https://hackmd.io/_uploads/H1uf8ttgR.png)

#### 5.2.2.8 Team Collaboration Insights during Sprint
A lo largo del primer sprint, todos los integrantes del equipo de HomeHeavenly estuvimos comprometidos y colaboramos de manera continua en la realización de las tareas asignadas. Cada uno de nosotros demostró el avance de sus respectivas labores mediante la presentación de sus avances individuales.
![image](https://hackmd.io/_uploads/H14cUtFe0.png)

### 5.2.3 Sprint 3
#### 5.2.3.1. Sprint Planning 3
En esta sección, se detalla el desarrollo de una nueva versión de nuestra aplicación web, incluyendo una reestructuración significativa del equipo de trabajo del proyecto. Este proceso implicó una reevaluación de roles y responsabilidades dentro del equipo, asegurando una distribución equilibrada de tareas y habilidades para maximizar la eficacia del proyecto. Además, se inició el desarrollo del backend del sistema, introduciendo nuevas funcionalidades y mejorando la infraestructura técnica subyacente. La participación activa de todos los miembros del equipo fue crucial, desde la realización de commits hasta la colaboración en la creación de ambas partes de la aplicación, front-end y back-end. Esta reestructuración no solo mejoró la dinámica interna del equipo sino que también permitió una mayor flexibilidad y adaptabilidad frente a los desafíos técnicos y de proyecto.

| Sprint # | Sprint 3  | 
|--------------------|------------|
| Sprint Planning Background | 
| Date | 2024-05-30 | 
| Time |  10:00 AM |
| Location |  UPC - Campus San Miguel |
| Preparate by| Maycol Jhordan Rojas Velasquez | 
|  Attendees (to planning meeting) | -Cantoral Sedamano, Alexander ALberto -Calderón Huamán, Jose Daniel Mario -Antonio Fretle, Jeremi Jose -Manco Cuellar, Anthony Ramon | 
| Sprint n-1 Review Summary | Se realizó las correcciones necesarios para el front-end de la aplicación web | 
| Sprint Planning Background | Luego de la reestructuración del equipo se repartiaron las tareas apropiadas para cada miembro relacionado con el backend |
| Sprint Goal & User Stories | 
| Sprint 1 Goal | Desarrolar la funcionalidad de la página web con relacionada con el back-end utilizando Spring realizando el código con ayuda del diagrama de Base de datos.|  
| Sprint Velocity | Se establece un Velocity de 40 Story Points para este Sprint. | 
| Sum of Story Points | 40 Story Points | 

#### 5.2.3.2. Sprint Backlog 3

Este Sprint se centra en la implementación de una nueva vista para nuestra página web y apliaciones web, diseñada para mejorar la experiencia del usuario mediante una interfaz más visual y moderna. El objetivo principal es proporcionar a nuestros usuarios una forma más intuitiva y atractiva de interactuar con nuestra plataforma, haciendo que la navegación y el acceso a las funcionalidades sean más fluidos y menos complicados.Además de la nueva vista, el Sprint también incluirá la incorporación de funciones básicas esenciales que faciliten el uso de la plataforma para los usuarios nuevos y existentes. Estas funciones estarán diseñadas para ser simples y directas, permitiendo a los usuarios realizar tareas comunes de manera rápida y eficiente.La implementación de esta nueva vista y funcionalidades básicas es un paso crucial para mejorar la usabilidad y la retención de usuarios, asegurando que nuestra plataforma permanezca competitiva y relevante en el mercado. Este Sprint representará un hito importante en el camino hacia la mejora continua de nuestra oferta digital, buscando siempre ofrecer la mejor experiencia posible a nuestros usuarios.


<table align="center" border="1" width="90%" style="text-align:center">
 <tr>
    <td colspan="2"><b>User Story</b></td>
    <td colspan="6"><b>Work-Item / Task</b></td>
  </tr>
  <tr>
    <td><b>Id</b></td>
    <td><b>Title</b></td>
    <td><b>Id</b></td>
    <td><b>Title</b></td>
    <td><b>Estimation</b></td>
    <td><b>Assigned To</b></td>
    <td><b>Status(To-do/ In-Process/ To-Review/ Done)</b></td>
  </tr>
  <tr>
    <td>US006</td>
    <td>Iniciar Sesión en la aplicación</td>
    <td>T01</td>
    <td>Inicio de la sesión en la aplicación</td>
    <td>4</td>
    <td>Rojas Velasquez, Maycol Jhordan</td>
    <td>Done</td>
 </tr>
 <tr>
    <td>US011</td>
    <td>Agregar Propiedad</td>
    <td>T02</td>
    <td>Agregación de propiedad</td>
    <td>5</td>
    <td>Calderón Huamán, Jose Daniel Mario</td>
    <td>Done</td>
<tr>
    <td>US018</td>
    <td>Ver Disponibilidad de Citas</td>
    <td>T03</td>
    <td>Citas disponibles</td>
    <td>4</td>
    <td>Rojas Velasquez, Maycol Jhordan</td>
    <td>Done</td>
 </tr>
<tr>
    <td>US019</td>
    <td>Reservar Cita para ver propiedad</td>
    <td>T04</td>
    <td>Reserva de citas</td>
    <td>4</td>
    <td>Rojas Velasquez, Maycol Jhordan</td>
    <td>Done</td>
 </tr>
<tr>
    <td>US020</td>
    <td>Ver mis citas reservadas</td>
    <td>T05</td>
    <td>Ver citas reservadas</td>
    <td>5</td>
    <td>Rojas Velasquez, Maycol Jhordan</td>
    <td>Done</td>
 </tr>
   <tr>
    <td>US023</td>
    <td>Gestión de Métodos de Pago</td>
    <td>T06</td>
    <td>Métodos de pago</td>
    <td>5</td>
    <td>Antonio Fretle, Jeremi Jose</td>
    <td>Done</td>
 </tr>
   <tr>
    <td>US024</td>
    <td>Página no encontrada 404</td>
    <td>T07</td>
    <td>Página no encontrada</td>
    <td>3</td>
    <td>Rojas Velasquez, Maycol Jhordan</td>
    <td>Done</td>
 </tr>
</table>

![image](https://hackmd.io/_uploads/SJZfYn8XC.png)


#### 5.2.3.3. Development Evidence for Sprint Review

| Repository | Branch | Commit Id | Commit Message | Commit Message Body | Commited on (Date) |
|:----------:|:------:|:---------:|:--------------:|:-------------------:|:------------------:|
| Landing-page | dev | 7079360ade051c90fe9258d654ae73a4f9f582fa | Merge pull request #36 | from SI729-2401-WS53-Grupo-MiCasita/dev | Jun 4, 2024 |
| Grupo02-Micasita-Angular-front | feat/calendar-appointment | ef714be93b8df19d0c079fa1841fe5548da6ac77 | fix | fixed publishing properties in create-estates | Jun 4, 2024 | 
| Grupo02-Micasita-Angular-front |feat/page-not-found| 14a742463d6e002214c0578b1a067bc63d4c6e80 | feat: |updated db.json with new attributes and improved visuals for create-estates form and estate-details | Jun 2, 2024 | 
| Grupo02-Micasita-SpringBoot-backend | feature-communication | 1e093268f1f68c0d84d0ce49b326207c3d0bb025 | add | Seller, Property and Appointment entities | Commits on Jun 2, 2024 |
| Grupo02-Micasita-SpringBoot-backend | feature-estates | 039ab53585fa595e411460acc8ddd534b621f25b | Merge pull request #11  | from SI729-2401-WS53-Grupo-MiCasita/feature-estates | Jun 6, 2024 | 
| Grupo02-Micasita-SpringBoot-backend | feature-estates | bb9e0946c11d2ab712cf7e52386467df81dd2102 | update feature | transaction | Jun 2, 2024 |
| Grupo02-Micasita-SpringBoot-backend | feature-user | 3570b6cdd346a0b94efec4b2005e9b264f9186a0 | feat | add resources, transforms, and PropertyController | Jun 6, 2024 |
| Grupo02-Micasita-SpringBoot-backend | feature-user | 1f63201c5c16a3ed1e68b0e15e6564399d1ea55c | feat | update attributes in CreatePropertyResource, PropertyResource, UpdatePropertyResource and transforms | Jun 8, 2024 |

Link del repositorio Landing page: https://github.com/SI729-2401-WS53-Grupo-MiCasita/Landing-page

Link del repositorio Front-end: https://github.com/SI729-2401-WS53-Grupo-MiCasita/Grupo02-Micasita-Angular-front

Link del repositorio Back-end: https://github.com/SI729-2401-WS53-Grupo-MiCasita/Grupo02-Micasita-SpringBoot-backend

#### 5.2.3.4. Testing Suite Evidence for Sprint Review

| Repository/Branch | Commit Id | Commit Message | Commit Message Body | Commited on (Date) |
|:-----------------:|:---------:|:--------------:|:-------------------:|:------------------:|
| Grupo02-MiCasita-testing / HU01 | 196b29e | Add | files via upload | May 14, 2024 |
| Grupo02-MiCasita-testing / HU02 | 3c46002 | Add |files via upload | May 14, 2024 |
| Grupo02-MiCasita-testing / HU03 | 3c46002 | Add |files via upload | May 14, 2024 |
| Grupo02-MiCasita-testing / HU05 | c1eaf91 | Create |HU05 - TP.feature | Jun 9, 2024 |
| Grupo02-MiCasita-testing / HU11 | 1e0ff69 | Update and rename HU11 | TP.feature to HU11 - TB2.feature | Jun 9, 2024 |
| Grupo02-MiCasita-testing / HU18 | 3c46002 | Add |files via upload | May 14, 2024 |

Link del repositorio del testing: https://github.com/SI729-2401-WS53-Grupo-MiCasita/Grupo02-MiCasita-testing 

#### 5.2.3.5. Execution Evidence for Sprint Review

Para este sprint se consolido el avance del frontend, LandingPage y la primera versión del backend de la aplicación web.

Video explicativo del avance del backend

![image](https://github.com/SI729-2401-WS53-Grupo-MiCasita/Documentation/assets/66744988/c84cad2d-1856-497f-9d1c-04e38d64052e)

Link del repositorio de los webservices: https://github.com/SI729-2401-WS53-Grupo-MiCasita/Grupo02-Micasita-SpringBoot-backend

Link de vídeo explicativo del backend:"https://acortar.link/5FCTLg"


#### 5.2.3.6. Services Documentation Evidence for Sprint Review

Evidencia del Back-end
![image](https://raw.githubusercontent.com/AlexlmL/ImagesforOpenSource/main/back1.png)
![image](https://raw.githubusercontent.com/AlexlmL/ImagesforOpenSource/main/back2.png)
![image](https://raw.githubusercontent.com/AlexlmL/ImagesforOpenSource/main/back-3.png)

#### 5.2.3.7. Software Deployment Evidence for Sprint Review

Landing Page evidence:
![image](https://raw.githubusercontent.com/AlexlmL/ImagesforOpenSource/main/Landingpageopen.PNG)
Link de la Landing Page desplegada: https://micasita-landingpage.netlify.app/ 
Frontend Evidence:
![image](https://raw.githubusercontent.com/AlexlmL/ImagesforOpenSource/main/aplicaci%C3%B3n%20webopen.PNG)
Link del Frontend desplegado: https://micasita-frontend.web.app


#### 5.2.3.8. Team Collaboration Insights during Sprint

En este apartado se adjuntarán las evidencias de la colaboración durante el sprint

LandinPage Insights:
![image](https://raw.githubusercontent.com/AlexlmL/ImagesforOpenSource/main/Insights%20lp.PNG)
Frontend Insights:
![image](https://raw.githubusercontent.com/AlexlmL/ImagesforOpenSource/main/Insights%20front.PNG)
Backend Insights:
![image](https://raw.githubusercontent.com/AlexlmL/ImagesforOpenSource/main/Insights%20back.PNG)


### 5.2.4 Sprint 4

#### 5.2.4.1. Sprint Planning 4
En esta sección se verán los detalles faltantes pospuestos del anterior sprint junto con el deploy del backend, unión del frontend con el backend y adición de tipos de administración.

| Sprint # | Sprint 4  | 
|--------------------|------------|
| Sprint Planning Background | 
| Date | 2024-03-24 | 
| Time |  10:00 AM |
| Location |  UPC - Campus San Miguel |
| Prepared by | Maycol Jhordan Rojas Velasquez | 
| Attendees (to planning meeting) | -Cantoral Sedamano, Alexander Alberto <br> -Calderón Huamán, Jose Daniel Mario <br> -Antonio Fretle, Jeremi Jose <br> -Manco Cuellar, Anthony Ramon | 
| Sprint n-1 Review Summary | Se completaron las funcionalidades del back-end incluyendo la gestión de métodos de pago, citas reservadas y la adición de nuevas propiedades. |
| Sprint Planning Background | En este sprint, se enfoca en finalizar las funcionalidades pendientes del back-end y asegurarse de que las interacciones entre el front-end y el back-end funcionen correctamente. |
| Sprint Goal & User Stories | 
| Sprint 4 Goal | Completar las funcionalidades de la página web relacionadas con el back-end, y asegurar la integración y el correcto funcionamiento de las mismas. |  
| Sprint Velocity | Se establece un Velocity de 45 Story Points para este Sprint. | 
| Sum of Story Points | 45 Story Points | 

#### 5.2.4.2. Sprint Backlog 4

En este Sprint nos enfocaremos en la optimización de la carga y rendimiento de la nueva vista implementada en el Sprint anterior, así como en la corrección de posibles errores o ajustes derivados de la retroalimentación inicial de los usuarios. Además, exploraremos la integración de características avanzadas que enriquezcan la experiencia del usuario, tales como notificaciones en tiempo real y personalización de contenido según preferencias.

El objetivo principal es la conexión entre el backend y frontend.

| Epic / Story ID | Título | Descripción | 
|-----------------|--------|-------------|
| US021 | Cancelar Cita Reservada | Como usuario, quiero poder cancelar una cita que he reservado para ver una propiedad si ya no puedo asistir, para liberar ese horario para otros usuarios.|
| TS14 | Cancelar Cita Reservada | Como developer, voy a desarrollar una Api que permita que se puedan cancelar las reservas de la aplicación web |
|TS15 | Inicio de sesión como administrador | Como developer, quiero poder iniciar sesión en la aplicación para gestionar las funcionalidades de administración | 

<table align="center" border="1" width="90%" style="text-align:center">
 <tr>
    <td colspan="2"><b>User Story</b></td>
    <td colspan="6"><b>Work-Item / Task</b></td>
  </tr>
  <tr>
    <td><b>Id</b></td>
    <td><b>Title</b></td>
    <td><b>Estimation</b></td>
    <td><b>Assigned To</b></td>
    <td><b>Status(To-do/ In-Process/ To-Review/ Done)</b></td>
  </tr>
  <tr>
    <td>US21</td>
    <td>Cancelar Cita Reservada</td>
    <td>5</td>
    <td>Cantoral Sedamano, Alexander Alberto</td>
    <td>Done</td>
 </tr>
 <tr>
    <td>TS14</td>
    <td>Cancelar Cita Reservada</td>
    <td>5</td>
    <td>Cantoral Sedamano, Alexander Alberto</td>
    <td>Done</td>
<tr>
    <td>TS15</td>
    <td>Inicio de sesión como administrador</td>
    <td>5</td>
    <td>Rojas Velasquez, Maycol Jhordan</td>
    <td>Done</td>
 </tr>
 </table>

![image](https://raw.githubusercontent.com/AlexlmL/ImagesforOpenSource/main/sprint4.PNG)

#### 5.2.4.3. Development Evidence for Sprint Review

| Repository | Branch | Commit Id | Commit Message | Commit Message Body | Commited on (Date) |
|:----------:|:------:|:---------:|:--------------:|:-------------------:|:------------------:|
| SpringBoot-backend | dev|c419e0b| Merge pull request #17 | from SI729-2401-WS53-Grupo-MiCasita/feature-transaction |23/06/2024|
| SpringBoot-backend | dev|c28340a| Merge pull request #18 | from SI729-2401-WS53-Grupo-MiCasita/feature-interaction |23/06/2024|

Link de repositorio Front-end: https://github.com/SI729-2401-WS53-Grupo-MiCasita/Grupo02-Micasita-Angular-front

Link de repositorio Back-end: https://github.com/SI729-2401-WS53-Grupo-MiCasita/Grupo02-Micasita-SpringBoot-backend

#### 5.2.4.4. Testing Suite Evidence for Sprint Review

| Repository/Branch | Commit Id | Commit Message | Commit Message Body | Commited on (Date) |
|:-----------------:|:---------:|:--------------:|:-------------------:|:------------------:|
| feature/tf-Alexander-Cantoral| b0e90b3 | Sprint 4| |24/06/2024 |

Link de repositorio testing: https://github.com/SI729-2401-WS53-Grupo-MiCasita/Grupo02-MiCasita-testing

#### 5.2.4.5. Execution Evidence for Sprint Review

En esta sección se adjuntará evidencia de la ejecución de lo desarrollado para este sprint:

Link del vídeo: " "

#### 5.2.4.6. Services Documentation Evidence for Sprint Review

En esta sección se adjuntará evidencia del desarrollo para este sprint:

Link de la Documentación web: http://localhost:8080/swagger-ui/index.html#/

Evidencia de los endpoints realizados:

![image](https://raw.githubusercontent.com/AlexlmL/ImagesforOpenSource/main/endpoints.PNG)
![image](https://raw.githubusercontent.com/AlexlmL/ImagesforOpenSource/main/endpoints2.PNG)

Se realizaron los endpoints Reservation, Buy, Rent, User, Properties, PropertiesImages y  Voucher.
Se hizo uso de enums para los endpoints de Reservation, Properties. 
Para reservation en el atributo de "status": 'PENDING' o 'CONFIRMED' o 'CANCELLED'.
Para Properties en el atributo de "status": 'Sale' o 'Rent'y "type": 'House' o 'Apartment'
Además se debe tener en cuenta esto para los atributos de Buy o Rent: dni: MAX 8 y MIN 8 , phoneNumber: MAX 9 y MIN 9
Y para User:  email: debe tener un arroba , dni: max 8 , phone number 9.

Para que esto funcione en local se debe de crear una base de datos en pgadmin4 con el nombre de "micasita".

Id de los commits relacionados: b233b67, 3aa0a4e, 5b752a0, da28ee4, a05c533, c28340a

#### 5.2.4.7. Software Deployment Evidence for Sprint Review
En esta sección se dará evidencia del deploy de la aplicación web completa:

Landing Page evidence:
![image](https://raw.githubusercontent.com/AlexlmL/ImagesforOpenSource/main/Landingpageopen.PNG)
Link de la Landing Page desplegada: https://micasita-landingpage.netlify.app/ 
Frontend Evidence:
![image](https://raw.githubusercontent.com/AlexlmL/ImagesforOpenSource/main/aplicaci%C3%B3n%20webopen.PNG)
Link del Frontend desplegado: https://micasita-frontend.web.app
Backend Evidence:
![image]()


#### 5.2.4.8. Team Collaboration Insights during Sprint

En esta sección se presentará los insights de los repositorios donde se avanzó el proyecto.

![image]()
![image]()
![image]()


## 5.3. Validation Interviews

### 5.3.1. Design of Interviews

Esta parte del informe presentará la parte objetiva de las entrevistas junto con el análisis relevante de cada una de ellas. Al ser preguntas generales de uso, no se distinguirá de segmento objetivo.

Preguntas principales:
¿Qué te parece la Landing Page?
¿Siente que es facil de usar?
¿Podrías hacerme el favor de registrarte y mandar un mensaje?
¿Qué te parece la aplicación web?
¿Siente que la aplicación web satisfacerá tus necesidades como futur@ usuario?


### 5.3.2. Recording of Interviews

Link de entrevistas: https://acortar.link/nK1qDF 

### Entrevista 1

![Entrevista 1](https://raw.githubusercontent.com/AlexlmL/ImagesforOpenSource/main/Entrevista%201%20Maycol.PNG)

| Nombres | Apellidos | Edad | Distrito | Inicio | Duración |
|---------|-----------|------|--------------|----------|--------|
| Maria Delia | Martinez Meza | 20 | Lima, Lima |  0:00| 8:59 |

Descripción: María, estudiante de tecnología médica, comenta que la página es muy llamativa visualmente, con colores e imágenes de buena calidad. Aprecia la segmentación clara de las propiedades por cuartos, tamaño, distrito, y número de pisos. María destaca la inclusión de propiedades de distintos departamentos de Perú, no solo Lima, lo que es beneficioso para estudiantes de provincia. Valora la seguridad ofrecida por los comentarios de otros usuarios y pregunta sobre el motivo del proyecto, que le explican está dirigido a estudiantes y familias jóvenes. Finalmente, María encuentra la página fácil de usar y bien estructurada para universitarios con poco tiempo y experiencia.

![Entrevista 2](https://raw.githubusercontent.com/AlexlmL/ImagesforOpenSource/main/Entrevista%202.PNG)

| Nombres | Apellidos | Edad | Distrito | Inicio | Duración |
|---------|-----------|------|--------------|----------|--------|
| Diego Sebastián | Valdivia Colque | 19 | Lima, Lima |  8:59|  |

Descripción: Diego, quien representa al segmento objetivo del cliente, explora la landing page y encuentra que se enfoca en alquilar casas cerca de universidades, lo cual es útil para estudiantes que viven lejos. Diego navega por los diferentes apartados, como el inicio, sobre nosotros, contacto, y centro de ayuda. También crea una cuenta y prueba funcionalidades como la compra y renta de propiedades, la descripción detallada de propiedades, y el proceso de pago. Sugiere mejorar con botones de confirmación y agrega que la página cumple su objetivo de ser intuitiva y fácil de usar.

![Entrevista 3](https://raw.githubusercontent.com/AlexlmL/ImagesforOpenSource/main/Entrevista%203%20anthony.PNG)

| Nombres | Apellidos | Edad | Distrito | Inicio | Duración |
|---------|-----------|------|--------------|----------|--------|
| Samantha Allison | Balazar Saavedra | 23 | Lima, Lima |  08:38 |

Descripción: Samantha, estudiante de enfermería, navega por la página y encuentra que es accesible y llamativa, con buena distribución de colores y secciones específicas. Registra una cuenta y explora las propiedades disponibles para compra y renta, notando que las descripciones detalladas son útiles. También prueba funcionalidades como el proceso de simulación de renta, añadir una propiedad, y reservar citas para ver propiedades. Samantha sugiere añadir más imágenes y la posibilidad de conversar directamente con el arrendatario, y concluye que recomendaría la página por su facilidad de uso y buena distribución.

![Entrevista 4](https://raw.githubusercontent.com/AlexlmL/ImagesforOpenSource/main/Entrevista%204.PNG)

| Nombres | Apellidos | Edad | Distrito | Inicio | Duración |
|---------|-----------|------|--------------|----------|--------|
| Alfredo | Medina | 23 | Lima, Lima |  26:24| 07:08 |

Descripción: Alfredo revisa la página comenzando por la portada y opciones de casas disponibles. Navega por las opciones de registro, contacto, y exploración de propiedades en diferentes distritos. Realiza una simulación de registro y reserva de una propiedad. También prueba la funcionalidad de añadir una propiedad, ingresando detalles como el nombre, ubicación, características, y precio. El proceso finaliza con la carga de una imagen de la propiedad. El usuario concluye cerrando sesión y agradece por la oportunidad de interactuar con la aplicación.

### 5.3.3. Evaluations according to Heuristics

UX Heuristics & Principles Evaluation  

Usability – Inclusive Design – Information Architecture  

CARRERA: Ingeniería de Software  

CURSO: Desarrollo de Aplicaciones Open Source  

SECCIÓN: WS53  

PROFESORES: *Juan Antonio Flores Moroco, Jimmy Alexander Armas Aguirre y Angel Augusto Velasquez Nuñez*

AUDITOR :  Grupo 2 

CLIENTE(S): *Maria Delia Martinez Meza, Diego Sebastián Valdivia Colque, Samantha Allison, Balazar Saavedra y Alfredo Medina.*

 

SITE o APP A EVALUAR: 

Nombre de App: *Mi Casita*

 

TAREAS A EVALUAR: 

 

**Registro de Usuario:**

Descripción: El usuario debe poder registrarse en la plataforma usando su correo electrónico y una contraseña. 

Objetivo: Evaluar la facilidad y eficiencia del proceso de registro. 


**Inicio de Sesión:**

Descripción: El usuario debe poder iniciar sesión utilizando su correo electrónico y contraseña. 

Objetivo: Verificar la usabilidad y rapidez del inicio de sesión. 


**Exploración de Propiedades:**

Descripción: El usuario debe poder navegar y explorar las propiedades disponibles para alquiler o compra. 

Objetivo: Evaluar la navegación y organización de la información. 

**Visualización de Detalles de Propiedad:**

Descripción: El usuario debe poder ver los detalles completos de una propiedad seleccionada. 

Objetivo: Comprobar la claridad y exhaustividad de la información proporcionada. 

**Agregar una Propiedad:**

Descripción: El usuario debe poder agregar una nueva propiedad para alquiler o venta. 

Objetivo: Verificar la usabilidad del proceso de adición de propiedades. 


**Reservar una Visita:**

Descripción: El usuario debe poder reservar una cita para visitar una propiedad. 

Objetivo: Evaluar la facilidad y funcionalidad del sistema de reservas. 

**Simulación de Compra/Alquiler:**

Descripción: El usuario debe poder simular el proceso de compra o alquiler de una propiedad. 

Objetivo: Verificar la usabilidad y claridad del proceso de simulación de transacción. 


**Cerrar Sesión:**

Descripción: El usuario debe poder cerrar sesión de la plataforma. 

Objetivo: Evaluar la facilidad y seguridad del proceso de cierre de sesión. 

 

**Escala de severidad:**  

| Nivel  | Descripción |
|---------|-----------|
| 1 | Problema superficial: puede ser fácilmente superado por el usuario o con muy poca frecuencia. No necesita ser arreglado a no ser que exista disponibilidad de tiempo. |
| 2 | Problema menor: puede ocurrir un poco más frecuentemente o es poco más difícil de superar para el usuario. Se le debería asignar una prioridad baja, resolverlo de cara a la siguiente reléase. |
| 3 | Problema mayor: ocurre frecuentemente o los usuarios no son capaces de resolverlos. Es importante que sean corregidos y se debe asignar una prioridad alta. |
| 4 | Problema muy grave: un error de gran impacto que impide al usuario continuar con el uso de la herramienta. Es imperativo que sea corregido antes del lanzamiento. |

**Tabla resumen:**
| # | Problema | Escala de severidad | Heurística/Principio violada(o) |
|---------|-----------|------|---------|
| 1 | No se tiene un control del pop up en la Landing Page | 2 | Usability: Libertad y control de usuario |
| 2 | El botón de signup te hace iniciar sesión de forma repentina | 1 | Usability: Consistencia y estándares |
| 3 | Falta unión de con backend para poder ver las propiedades añadidas | 1 | Feedback y visibilidad del sistema (en relación con la usabilidad) |

**Descripción de problemas:**

Problema #1:  No se tiene un control del pop up en la Landing Page 

Severidad: 2 

Heurística/Principio violado: Usabilidad: Libertad y control de usuario 

Descripción: Los usuarios no pueden controlar la aparición o el cierre de los pop-ups en la página de inicio. Esto puede causar frustración y una sensación de pérdida de control sobre la navegación. 

Recomendación: Permitir que los usuarios cierren los pop-ups fácilmente y evitar que aparezcan de manera intrusiva o repetitiva sin una acción del usuario. 

Problema #2: El botón de signup te hace iniciar sesión de forma repentina 

Severidad: 1 

Heurística/Principio violado: Usabilidad: Consistencia y estándares 

Descripción: Un botón de "signup" (registrarse) debería llevar a un formulario de registro, pero si en lugar de eso inicia sesión de manera inesperada, se rompe con la expectativa del usuario y la consistencia del diseño. 

Recomendación: Asegurarse de que el botón de "signup" lleve a la página de login o verificación de correo y que cualquier redirección sea clara y predecible. 

Problema #3: Falta unión con backend para poder ver las propiedades añadidas 

Severidad: 1 

Heurística/Principio violado: Feedback y visibilidad del sistema (en relación con la usabilidad) 

Descripción: Si los usuarios no pueden ver las propiedades que han añadido porque no hay conexión con el backend, falta el feedback necesario que informe al usuario de que sus acciones han sido exitosas. 

Recomendación: Implementar la conexión con el backend para que el usuario pueda ver su propiedad agregada a la sección que corresponda. 

## 5.4. Video About-the-Product

Video about the product: "https://upcedupe-my.sharepoint.com/:v:/g/personal/u20181b152_upc_edu_pe/EduhzE3v9AtHhmaa_crqWTcBpIxM06ta11vHziGI2O2SIw?e=zgPDtq&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D"

## Conclusiones 

En el proyecto, la ejecución fue exitosa gracias a la coordinación eficiente entre los tres miembros del equipo. Todos contribuyeron de manera colaborativa, codificando dentro de los límites del contexto de manera satisfactoria.

Video about the team: "https://upcedupe-my.sharepoint.com/:v:/g/personal/u20181b152_upc_edu_pe/EZIeY6jngL1AgY_RrBMWGO0BY9tXiCc5jbRLmZhA7b9GQA?e=aZkwQT&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D"

## Bibliografía

1. The C4 model for visualising software architecture (2024) Recuperado de: https://c4model.com
2. Naming Conventions for java (2024) Recuperado de: https://www.oracle.com/java/technologies/javase/codeconventions-namingconventions.html#:~:text=Except%20for%20variables%2C%20all%20instance,should%20be%20short%20yet%20meaningful.

## Anexos

**Enlaces**

</center>

 |Segmento del trabajo|Link de repositorio|
|---------|---------|
| LandingPage (Anexo A)    | https://github.com/SI729-2401-WS53-Grupo-MiCasita/Documentation |
| Diagramas de clases (Anexo B)   | https://lucid.app/documents/view/c7d290c1-6d5f-4e26-b73e-cfdbba38c57a     |
| Diagramas de base de datos (Anexo C)   | https://my.vertabelo.com/doc/wrl6YNg5OsGyeUKD2zrofTFNGwBj0sOF   |
| Proyecto Anagular   |  https://github.com/SI729-2401-WS53-Grupo-MiCasita/Grupo02-Micasita-Angular-front  |



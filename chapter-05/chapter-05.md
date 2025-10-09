# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management

En esta sección, nuestro equipo establece las decisiones y convenciones para mantener una consistencia durante todo el desarrollo del proyecto. Estas convenciones son cruciales para asegurar que todos los miembros del equipo estén alineados en términos de uso de herramientas, buenas prácticas y procesos de despliegue.

### 5.1.1. Software Development Environment Configuration

En este apartado se mencionan los distintos productos de software empleados por el equipo para llevar a cabo las actividades relacionadas con la elaboración del proyecto.

**Product UX/UI Desing**

1. **UXPressia:** https://uxpressia.com/Se utilizó para la creación de User Personas, Empathy Maps, Journey Maps e Impact Maps, proporcionando una visión centrada en el usuario.

2. **Figma**: https://www.figma.com/Herramienta de diseño colaborativo utilizada para la creación de wireframes, mock-ups y prototipos de aplicaciones móviles y de escritorio.

**Software Development**

3. **Visual Studio Code**: https://code.visualstudio.com/Entorno de desarrollo ligero empleado para la creación del landing page y las aplicaciones web, utilizando HTML5, CSS3, JavaScript y TypeScript.

4. **WebStorm**: Entorno de desarrollo utilizado para trabajar con HTML, CSS, JavaScript y frameworks como Vue y Angular.

5. **Spring Boot Framework**:Framework utilizado para desarrollar servicios web RESTful en Java, proporcionando una base escalable y robusta.

6. **GitHub**: https://github.com/Plataforma de control de versiones utilizada para la gestión del código fuente, aplicando el flujo de trabajo GitFlow para garantizar un desarrollo ordenado.

**Project Management and Collaboration**

7. **WhatsApp**: https://web.whatsapp.com/Aplicación de mensajería utilizada para la coordinación y discusión de temas relacionados con el proyecto en tiempo real.

8. **Discord**: https://discord.com/ Aplicación de mensajería utilizada para la coordinación y discusión de temas relacionados con el proyecto en tiempo real

**Software Documentation**

9. **LucidChart**: https://lucid.app/Plataforma utilizada para la creación de diagramas UML, wireflows y user flows, facilitando la visualización y planificación del sistema.

10. **Structurizr**: https://www.structurizr.com/ Herramienta utilizada para modelar la arquitectura de software mediante diagramas C4, permitiendo un modelado claro de la estructura del proyecto.

**Software Testiong**

11. **Markdown**: Lenguaje de marcado ligero utilizado para documentar el proyecto y en los archivos README del repositorio de la organización.

### 5.1.2. Source Code Management

La gestión del código fuente es parte fundamental del desarrollo de cualquier proyecto de software, ya que nos permitirá rastrear cambios, revertir versionas y coordinar a los diferentes integrantes del equipo a la misma vez. En ENERGIX, utilizaremos **GitHub** como plataforma para alojar nuestros repositorios.

**URL de los Repositorios**

- **Organization:** https://github.com/Upc-pre-1ASI0729-2520-7401-Energix
- **Reporte:** https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Energix-Proyect-Report
- **Landing Page:** https://energixlp.netlify.app

**Commits Convencionales**

Para los mensajes de commit en el proyecto ENERGIX, se sigue la convención **Coventional Commits**. Estos mensajes deben seguir el formato estándar para facilitar la lectura y entendimiento del historial del proyecto:

``` githubexpressionlanguage
<type>[optional scope]:<decription>

[optional body]

[optional footer(s)]
```

- **Type**
-  -  ```feat```: Se usa cuando se añade una nueva catacterística.
-  -  ```fix```: Para la correción de errores.
-  -  ```docs```: Modificaciones en la documentación.
-  -  ```style```: Cambios que no afectan la lógica del código, como los formatos o estilos.
-  -  ```refactor```: Modificaciones que no añaden características ni corrigen errores.
-  -  ```test```: Addicón o modificación de pruebas.

- **Scope:** Proporciona información adicional sobre el área del código afectada.

**Ejemplos de commits**

- ```feat(login): add user authentication module```
- ```fix(payment): resolve payment gateway issue```
- ```docs(README): update setup instructions```

Con estas estructuras, ENERGIX se puede gestionar eficientemente el flujo de trabajo del desarrollo, asegurándonos una integración continua y una organización clara del código.

### 5.1.3. Source Code Style Guide & Conventions
En el proyecto ENERGIX, hemos implementaado una serie de guías de estilo y convenciones para asegurar que todo el equipo de desarrollo siga una estructura consistente y clara en todo el desarrollo del proyecto. Facilitando la legibidad del código, mejorando la colaboración entre los integrantes asegurando que el código sea mantenible a largo plazo.

**Nomenclatura General**

Para asegurar la coherencia en todo el código, seguiremos las siguientes directrices:

- Los nombres de variables, funciones y métodos deben utilizar **camelCase**.
- Los nombres de clases y componentes seguirán la convención **PascalCase**.
- Para los archivos y carpetas, se empleará la convención **kebab-Case**.

El uso de **ingles** para todos los nombres es obligatorio, con el fin de asegurar la comprensión entre los miembros del equipo y seguir las buenas prácticas.

**Ejemplo**

- **Variables:** ``` home```,```userLocation```
- **Clases:** ``` HomeOwner```,```user```
- **Archivos:** ```home-owner.service.js```,```user.controller.js```

**Espacios y Sangrías**

La sangría de código en ENERGIX seguirá las siguientes reglas para asegurar la claridad y el orden del código:

- Se utilizarán **2 espacios** para la sangría en archivos HTML, CSS, JavaScript, y TypeScript.
- En archivos **Java**, se utilizarán **4 espacios** para la sangría.

Esta convención ayuda a mantener la consistencia en todos los lenguajes empleados en el proyecto, facilitando la colaboración entre los diferentes miembros del equipo.

``` html
<!DOCTYPE html>
<html>
  <head>
    <title>Energix</title>
  </head>
  <body>
    <h1>Registros Disponible</h1>
    <p>Registra tus dispositivos fácilmente</p>
  </body>
</html>
```

**Convenciones por Lenguaje**

1. HTML/CSS/JavaScript:

- - Se utilizará la Google HTML/CSS Style Guide (https://google.github.io/styleguide/htmlcssguide.html) para asegurar la consistencia en la estructura y la presentación de los archivos HTML y CSS.
- - Para JavaScript, adoptamos la Airbnb JavaScript Style Guide (https://google.github.io/styleguide/htmlcssguide.html), ampliamente conocida y utilizada en la industria.

2. TypeScript:

- - Angular es el framework elegido para el frontend de PARKINGNOW, por lo que seguimos la Angular Style Guide (https://v17.angular.io/guide/styleguide), que dicta cómo deben estructurarse los módulos, servicios y componentes.
- - También seguimos la Google TypeScript Style Guide (https://google.github.io/styleguide/tsguide.html) para garantizar la correcta tipificación y legibilidad del código.

3. Java:

- - En el backend, utilizamos Spring Boot para crear APIs y servicios web. Seguimos la Google Java Style Guide (https://google.github.io/styleguide/javaguide.html) para mantener consistencia en la estructura de las clases y los métodos.
- - Los nombres de clases serán descriptivos, utilizando sustantivos para clases y verbos para métodos.

**Ejemplo de una clase Java**

``` javascript 
public class HomeOwner {
  private int totalDevices;

  public HomeOwner(int spaces) {
    this.availableSpaces = spaces;
  }

  public void devicesRegistered() {
    if (availableSpaces > 0) {
      availableSpaces--;
    }
  }
}
```

4. **Gherkin**
- - Para escribir los tests automatizados, seguimos la convención de Gherkin Syntax. (https://cucumber.io/docs/gherkin/) Esto permite una descripción clara y precisa de los escenarios de prueba en los archivos .feature.
- - Utilizamos Given-When-Then para describir el comportamiento esperado en cada escenario.

**Ejemplo de Gherkin**

``` gherkin
Feature: Registro de dispositivo 

  Scenario: Registro exitosa
    Given el usuario ha iniciado sesión
    When selecciona la opción de dispositivos
    Then el usuario debe configurar el dispositivo a registrar
    Then el sistema debe confirmar el registro
    
```

**Espacios y Comillas**

- **Espacios:** Siempre se debe colocar un espacio alrededor de los operadores y entre los parámetros en las funciones.

**Ejemplo:**

``` typescript

let totalDevices = 50;
let devicesRegistered = 10;
let availableSpace = totalDevices - devicesRegistered;
 
```
- **Commillas:** En **JavaScript** y **TypeScript**, se utilizan comillas simples ```(')``` para cadenas, mientras que en **HTML** se prefieren las comillas dobles ```(")```.

**Limite de Longitud de Línea**

El código no debe exceder las 80 columnas por líneas. En caso de necesitar más espacios, se recomienda dividir la línea de código para mejorar la legibilidad.
### 5.1.4. Software Deployment Configuration
- En esta sección se detalla la configuración necesaria para el despliegue de la solución ENERGIX, incluyendo los pasos claves para lograr la publicación satisfactoria de la Landing Page, Servicios Web y Aplicaciones Web Frontend utilizando Netlify para visualizar cada commit del Landing Page.

- A continuación, se describen los pasos para realizar el despliegue de la Landing Page del proyecto ENERGIX.- 1- **Actualización de Ramas**: Asegúrate de que todas las ramas del repositorio estén actualizadas. Luego, ingresa a Github y dirígete al repositorio del proyecto ENERGIX.
1. **Actualización de Ramas**: Asegúrate de que todas las ramas del repositorio estén actualizadas. Luego, ingresa a Netlify y dirígete al repositorio del proyecto ENERGIX.
2. **Acceso a las configuraciones**: Una vez dentro de Netifly, haz click en la pestaña Get Started en el centro de la pantalla, te loqueas con Git Hub, buscas la organización y el repositorio de tu landign page y la selecciones.
3. **Selección de la Configuración**: Selecciona la configuración y carga los archivos del repositorio. Esta opción permite generar el link de la landing page, con el nombre Energix.
4. **Acceso a la página**: Finalmente, podrás acceder a la Landing Page desde el enlace que se generó al finalizar el deploy. Aquí está el enlace para el proyecto ENERGIX: https://energixlp.netlify.app

### 5.2.1. Sprint 1

#### 5.2.1.1. Sprint Planning 1

Para este primer sprint nos enfocaremos en los tasks para la
elaboración de la Landing Page. Nos dividiremos entre nosotros cada
una de las tareas identificadas para el sprint.

<table>
<tr>
    <th colspan="5">Sprint 1</th>
    <th colspan="9">Sprint 1</th>
  </tr>
      <tr>
    <td colspan="13">Sprint Planning Background</td>
  </tr>
  <tr>
    <td colspan="5">Date</td>
    <td colspan="8">2025-09-15</td>
</tr>
  <tr>
    <td colspan="5">Time</td>
    <td colspan="8">4:30 PM</td>
  </tr>
  <tr>
    <td colspan="5">Location</td>
    <td colspan="8">Via Discord</td>
<tr>
    <td colspan="5">Prepared By</td>
    <td colspan="8">Iker Gabriel Barturen Panez</td>
</tr>
<tr>
    <td colspan="5">Attendees (to planning meeting)</td>
    <td colspan="8">Alexis Encalada Salazar, Yeira Shari Huaman Olivos, Andrés Rodrigo Torres Lavandera, Iker Gabriel Barturen Panez, Mateo Italo Loechle Arias</td>
</tr>
<tr>
    <td colspan="5">Sprint  1 Review Summary</td>
    <td colspan="8">En esta primera sección se planteo el desarrollo de la Landing Page y planeación de aplicación para el proyecto de Energix.</td>
</tr>
<tr>
    <td colspan="5">Sprint 1 Retrospective Summary</td>
    <td colspan="8">En esta sección todos los integrantes mencionaron tener aciertos en partes del codigo y en otras partes poder mejorar sus habilidades realizando la Landing Page</td>
</tr>
<tr>
    <td colspan="13">Sprint Goal & User Stories</td>
</tr>
<tr>
    <td colspan="5">Sprint 1 Goal</td>
    <td colspan="8">Desarrollar y desplegar una landing page que presente información a los usuarios a través de imágenes y texto. La página debe ser completamente adaptable a cualquier tipo de dispositivo que utilicen los usuarios, garantizando una experiencia de usuario fluida y responsiva.</td>
</tr>
<tr>
    <td colspan="5">Sprint 1 Velocity</td>
    <td colspan="8">5 story points</td>
</tr>
<tr>
    <td colspan="5">Sum of Story Points</td>
    <td colspan="8">5 Story Points</td>
</tr>
</table>

#### 5.2.1.2. Aspect Leaders and Collaborators

Con la finalidad de mejorar la colaboración en equipo a cada integrante se asignó un rol de líder por cada aspecto. Los aspectos están relacionados con los entregables.

| Team member (LastName, First Name) | GitHub UserName       | Aspect 1: Landing Page Leader (L) / Collaborator (C) | Aspect 2: Diseños Figma: Leader (L) / Collaborator (C) | Aspect 3: Reporte (L) / Collaborator (C) |
|------------------------------------|-----------------------|------------------------------------------------------|--------------------------------------------------------|------------------------------------------|
| Alexis Encalada                    | Alexiz248             | C                                                    | C                                                      | L                                        |
| Yeira Sharia                       | YeiShari              | L                                                    | L                                                      | L                                        |
| Andrés Torres                      | AndresTorres202312557 | C                                                    | L                                                      | L                                        |
| Iker Barturen                      | krxxg04               | L                                                    | L                                                      | L                                        |
| Mateo Loechle                      | LowMathzzz            | C                                                    | C                                                      | L                                        |

#### 5.2.1.3. Sprint Backlog 1

<table border="1">
  <tr>
    <th colspan="3">Sprint 1</th>
    <th colspan="10">Sprint 1</th>
  </tr>
  <tr>
    <td colspan="3">User Story</td>
    <td colspan="10">Work-Item/Task</td>
  </tr>
  <tr>
    <td>ID</td>
    <td colspan="2">Title</td>
    <td>ID</td>
    <td colspan="2">Title</td>
    <td colspan="3">Description</td>
    <td>Estimation</td>
    <td colspan="2">Assigned to</td>
    <td>Status</td>
  </tr>
  <tr>
    <td>US31</td>
    <td colspan="2">Consultar la propuesta de valor</td>
    <td>UT01</td>
    <td colspan="2">Redactar contenido de propuesta de valor</td>
    <td colspan="3">Crear el texto que explique los beneficios y el valor de la plataforma.</td>
    <td>2h</td>
    <td colspan="2">Iker Barturen</td>
    <td>Done</td>
  </tr>
  <tr>
    <td></td>
    <td colspan="2"></td>
    <td>UT02</td>
    <td colspan="2">Diseñar sección de propuesta de valor</td>
    <td colspan="3">Implementar la sección en la landing page con diseño atractivo y responsivo.</td>
    <td>2h</td>
    <td colspan="2">Iker Barturen</td>
    <td>Done</td>
  </tr>
  <tr>
    <td>US32</td>
    <td colspan="2">Acceder a preguntas frecuentes (FAQ)</td>
    <td>UT03</td>
    <td colspan="2">Redactar preguntas y respuestas frecuentes</td>
    <td colspan="3">Crear listado de dudas comunes y sus respuestas.</td>
    <td>2h</td>
    <td colspan="2">Yeira Huaman</td>
    <td>Done</td>
  </tr>
  <tr>
    <td></td>
    <td colspan="2"></td>
    <td>UT04</td>
    <td colspan="2">Implementar sección FAQ</td>
    <td colspan="3">Desarrollar componente visual (acordeón/collapsible) para mostrar las preguntas frecuentes.</td>
    <td>2h</td>
    <td colspan="2">Yeira Huaman</td>
    <td>Done</td>
  </tr>
  <tr>
    <td>US33</td>
    <td colspan="2">Revisar planes de suscripción</td>
    <td>UT05</td>
    <td colspan="2">Redactar información de planes</td>
    <td colspan="3">Crear contenido sobre los distintos planes, precios y beneficios.</td>
    <td>3h</td>
    <td colspan="2">Andrés Torres</td>
    <td>Done</td>
  </tr>
  <tr>
    <td></td>
    <td colspan="2"></td>
    <td>UT06</td>
    <td colspan="2">Implementar sección de comparación de planes</td>
    <td colspan="3">Diseñar tabla o cards para comparar los planes en la landing page.</td>
    <td>3h</td>
    <td colspan="2">Andrés Torres</td>
    <td>Done</td>
  </tr>
  <tr>
    <td>US34</td>
    <td colspan="2">Consultar información del equipo</td>
    <td>UT07</td>
    <td colspan="2">Redactar información del equipo</td>
    <td colspan="3">Crear contenido sobre la misión, visión y miembros del equipo.</td>
    <td>2h</td>
    <td colspan="2">Alexis Encalada</td>
    <td>Done</td>
  </tr>
  <tr>
    <td></td>
    <td colspan="2"></td>
    <td>UT08</td>
    <td colspan="2">Implementar sección del equipo</td>
    <td colspan="3">Diseñar e integrar la sección del equipo en la landing page.</td>
    <td>2h</td>
    <td colspan="2">Alexis Encalada</td>
    <td>Done</td>
  </tr>
  <tr>
    <td>US35</td>
    <td colspan="2">Cambiar idioma</td>
    <td>UT09</td>
    <td colspan="2">Implementar selector de idioma</td>
    <td colspan="3">Desarrollar funcionalidad para cambiar entre español e inglés en la landing page.</td>
    <td>4h</td>
    <td colspan="2">Mateo Italo</td>
    <td>Done</td>
  </tr>
</table>

#### 5.2.1.4. Development Evidence for Sprint Review

En esta sección se demuestran los commits relacionados con los principales avances en la implementación.
Estos commits provienen del repositorio del Landing Page de la organización de GitHub.

Enlace al repositorio de la Landing Page: https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page# 

| Repository                                              | Branch                | Commit Id                                  | Commit Message            | Commit Message Body | Commited on (Date) |
|---------------------------------------------------------|-----------------------|--------------------------------------------|---------------------------|---------------------|--------------------|
| Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page | feature/start         | 692024b93d68e539d1cc5cbb6de3cd176d562b7c   | feat: add start.          |                     | 19/09/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page | feature/products      | 1eeb09c177966f93ac491cbd9b80a6e4ba81bc90   | feat: add products.       |                     | 19/09/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page | feature/subscriptions | 45f25028afb713b93cb8673a1ee5abdc9fe53594   | feat: add subscriptions.  |                     | 19/09/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page | feature/our-team      | d29df95ef29cdf224c966d07c8e8a15704647854   | feat: add our-team.       |                     | 19/09/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page | feature/Faqs          | 37f3b8c28d521878663c72a6ae046432deea790e   | feat: add Faqs.           |                     | 19/09/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page | feature/footer        | d09da40ecc996d11a3d84e31c003e4fa9d7bcf75   | feat: add footer.         |                     | 19/09/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page | feature/payment       | ff27629a30c625d174ef98b16b47b0a8ce97370a   | feat: add payment.        |                     | 19/09/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page | feature/js            | f83045d6a61811aab992b009689c67e2a3ed24e6   | feat: add files js.       |                     | 19/09/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page | feature/image         | f6cf2c1f36b63ab62729127683830a22fa1be8ba   | feat: add image.          |                     | 19/09/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page | feature/responsive    | 5d38b6997ae8e5326d8a96f618a460612610a6af   | feat: add responsive.     |                     | 20/09/2025         |

#### 5.2.1.5. Execution Evidence for Sprint Review

Durante el desarrollo del sprint se lograron completar todos los puntos planteados. A continuación se muestran evidencias del landing page logrado.



#### 5.2.1.6. Services Documentation Evidence for Sprint Review

Como se mencionó previamente, Este sprint solo tuvo como objetivo el desarrollo de Landing Page. Aún no se han implementado ni documentado Endpoints con OpenAPI, ya que el desarrollo de los servicios web está planificado para los siguientes Sprints, conforme al roadmap del proyecto.

#### 5.2.1.7. Software Deployment Evidence for Sprint Review

Durante este Sprint, se completó el desarrollo de la Landing Page y se realizó su despliegue utilizando GitHub Pages como plataforma de publicación gratuita. El objetivo fue contar con una primera versión accesible en línea del producto digital para revisión y retroalimentación.

Actividades realizadas: Se creó el repositorio en GitHub: https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page#

Se subió el código fuente de la Landing Page, incluyendo los archivos HTML, CSS necesarios.

Se configuró GitHub Pages desde la pestaña Settings > Pages, seleccionando la rama principal y la carpeta raíz.

Se verificó la correcta publicación de la Landing Page en la siguiente URL: https://energixlp.netlify.app

#### 5.2.1.8. Team Collaboration Insights during Sprint

En esta sección se evidencia la colaboración de cada integrante en el repositorio de la Landing Page.

Repositorio de Landing Page: https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page#

| **Integrante**                       | **Actividad**                                                                                          |  
|--------------------------------------|--------------------------------------------------------------------------------------------------------|
| **Huaman Olivos, Yeira Shari**       | Implementación de secciones de la **landing page** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |
| **Loechle Arias, Mateo Ítalo**       | Implementación de secciones de la **landing page** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |
| **Barturen Panez, Iker Gabriel**     | Implementación de secciones de la **landing page** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |
| **Encalada Salazar, Alexis**         | Implementación de secciones de la **landing page** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |
| **Torres Lavandera, Andrés Rodrigo** | Implementación de secciones de la **landing page** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |

**chapter 1, 2, 3, 4, 5.md**



**Landing Page**

### 5.2.2. Sprint 2

#### 5.2.2.1. Sprint Planning 2

Durante el Sprint 2 se estableció el desarrollo de la aplicación web de la plataforma Energix, enfocándose en la implementación de las principales vistas y funcionalidades orientadas a los perfiles propietarios de viviendas y universitarios que alquilan. El trabajo incluyó la integración de la interfaz con la base de datos, la gestión dinámica de la información de usuario y la mejora de la experiencia visual y de navegación. Asimismo, se priorizó la internacionalización (i18n) y la coherencia del diseño, consolidando una versión funcional y estable del sistema.

<table>
<tr>
    <th colspan="5">Sprint 2</th>
    <th colspan="9">Sprint 2</th>
  </tr>
      <tr>
    <td colspan="13">Sprint Planning Background</td>
  </tr>
  <tr>
    <td colspan="5">Date</td>
    <td colspan="8">2025-09-29</td>
</tr>
  <tr>
    <td colspan="5">Time</td>
    <td colspan="8">6:30 PM</td>
  </tr>
  <tr>
    <td colspan="5">Location</td>
    <td colspan="8">Via Discord</td>
<tr>
    <td colspan="5">Prepared By</td>
    <td colspan="8">Iker Gabriel Barturen Panez</td>
</tr>
<tr>
    <td colspan="5">Attendees (to planning meeting)</td>
    <td colspan="8">Alexis Encalada Salazar, Yeira Shari Huaman Olivos, Andrés Rodrigo Torres Lavandera, Iker Gabriel Barturen Panez, Mateo Italo Loechle Arias</td>
</tr>

<tr>
    <td colspan="13">Sprint Goal & User Stories</td>
</tr>
<tr>
    <td colspan="5">Sprint 2 Goal</td>
    <td colspan="8">Implementar y estabilizar la arquitectura fundamental de la aplicación web Energix, entregando la capa de presentación funcionalmente integrada a la base de datos para las vistas centrales y la gestión de datos de los perfiles de usuario (propietarios de viviendas y universitarios que alquilan), con soporte inicial para internacionalización (i18n).</td>
</tr>
<tr>
    <td colspan="5">Sprint 2 Velocity</td>
    <td colspan="8"></td>
</tr>
<tr>
    <td colspan="5">Sum of Story Points</td>
    <td colspan="8"></td>
</tr>
</table>

#### 5.2.2.2. Aspect Leaders and Collaborators

Con la finalidad de mejorar la colaboración en equipo a cada integrante se asignó un rol de líder por cada aspecto. Los aspectos están relacionados con los entregables.

| Team member (LastName, First Name) | GitHub UserName       | Aspect 1: Dashboard & Devices View | Aspect 2: Profile View and UI Design | Aspect 3: Reports View | Aspect 4: Notifications View | Aspect 5: Settings View |
|------------------------------------|-----------------------|------------------------------------|--------------------------------------------------------------------|------------------------|------------------------------|-------------------------|
| Alexis Encalada                    | Alexiz248             | C                                  | C                                                                  | C                      | C                            | L                       |
| Yeira Sharia                       | YeiShari              | C                                  | L                                                                  | C                      | C                            | C                       |
| Andrés Torres                      | AndresTorres202312557 | C                                  | C                                                                  | L                      | C                            | C                       |
| Iker Barturen                      | krxxg04               | L                                  | C                                                                  | C                      | C                            | C                       |
| Mateo Loechle                      | LowMathzzz            | C                                  | C                                                                  | C                      | L                            | C                       |

#### 5.2.2.3. Sprint Backlog 2

<table border="1">
  <tr>
    <th colspan="3">Sprint 1</th>
    <th colspan="10">Sprint 1</th>
  </tr>
  <tr>
    <td colspan="3">User Story</td>
    <td colspan="10">Work-Item/Task</td>
  </tr>
  <tr>
    <td>ID</td>
    <td colspan="2">Title</td>
    <td>ID</td>
    <td colspan="2">Title</td>
    <td colspan="3">Description</td>
    <td>Estimation</td>
    <td colspan="2">Assigned to</td>
    <td>Status</td>
  </tr>
  <tr>
    <td>US31</td>
    <td colspan="2">Consultar la propuesta de valor</td>
    <td>UT01</td>
    <td colspan="2">Redactar contenido de propuesta de valor</td>
    <td colspan="3">Crear el texto que explique los beneficios y el valor de la plataforma.</td>
    <td>2h</td>
    <td colspan="2">Iker Barturen</td>
    <td>Done</td>
  </tr>
  <tr>
    <td></td>
    <td colspan="2"></td>
    <td>UT02</td>
    <td colspan="2">Diseñar sección de propuesta de valor</td>
    <td colspan="3">Implementar la sección en la landing page con diseño atractivo y responsivo.</td>
    <td>2h</td>
    <td colspan="2">Iker Barturen</td>
    <td>Done</td>
  </tr>
  <tr>
    <td>US32</td>
    <td colspan="2">Acceder a preguntas frecuentes (FAQ)</td>
    <td>UT03</td>
    <td colspan="2">Redactar preguntas y respuestas frecuentes</td>
    <td colspan="3">Crear listado de dudas comunes y sus respuestas.</td>
    <td>2h</td>
    <td colspan="2">Yeira Huaman</td>
    <td>Done</td>
  </tr>
  <tr>
    <td></td>
    <td colspan="2"></td>
    <td>UT04</td>
    <td colspan="2">Implementar sección FAQ</td>
    <td colspan="3">Desarrollar componente visual (acordeón/collapsible) para mostrar las preguntas frecuentes.</td>
    <td>2h</td>
    <td colspan="2">Yeira Huaman</td>
    <td>Done</td>
  </tr>
  <tr>
    <td>US33</td>
    <td colspan="2">Revisar planes de suscripción</td>
    <td>UT05</td>
    <td colspan="2">Redactar información de planes</td>
    <td colspan="3">Crear contenido sobre los distintos planes, precios y beneficios.</td>
    <td>3h</td>
    <td colspan="2">Andrés Torres</td>
    <td>Done</td>
  </tr>
  <tr>
    <td></td>
    <td colspan="2"></td>
    <td>UT06</td>
    <td colspan="2">Implementar sección de comparación de planes</td>
    <td colspan="3">Diseñar tabla o cards para comparar los planes en la landing page.</td>
    <td>3h</td>
    <td colspan="2">Andrés Torres</td>
    <td>Done</td>
  </tr>
  <tr>
    <td>US34</td>
    <td colspan="2">Consultar información del equipo</td>
    <td>UT07</td>
    <td colspan="2">Redactar información del equipo</td>
    <td colspan="3">Crear contenido sobre la misión, visión y miembros del equipo.</td>
    <td>2h</td>
    <td colspan="2">Alexis Encalada</td>
    <td>Done</td>
  </tr>
  <tr>
    <td></td>
    <td colspan="2"></td>
    <td>UT08</td>
    <td colspan="2">Implementar sección del equipo</td>
    <td colspan="3">Diseñar e integrar la sección del equipo en la landing page.</td>
    <td>2h</td>
    <td colspan="2">Alexis Encalada</td>
    <td>Done</td>
  </tr>
  <tr>
    <td>US35</td>
    <td colspan="2">Cambiar idioma</td>
    <td>UT09</td>
    <td colspan="2">Implementar selector de idioma</td>
    <td colspan="3">Desarrollar funcionalidad para cambiar entre español e inglés en la landing page.</td>
    <td>4h</td>
    <td colspan="2">Mateo Italo</td>
    <td>Done</td>
  </tr>
</table>

#### 5.2.2.4. Development Evidence for Sprint Review

En esta sección se demuestran los commits relacionados con los principales avances en la implementación.
Estos commits provienen del repositorio del Landing Page de la organización de GitHub.

Enlace al repositorio de la Landing Page: https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page#

| Repository                                              | Branch                | Commit Id                                  | Commit Message            | Commit Message Body | Commited on (Date) |
|---------------------------------------------------------|-----------------------|--------------------------------------------|---------------------------|---------------------|--------------------|
| Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page | feature/start         | 692024b93d68e539d1cc5cbb6de3cd176d562b7c   | feat: add start.          |                     | 19/09/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page | feature/products      | 1eeb09c177966f93ac491cbd9b80a6e4ba81bc90   | feat: add products.       |                     | 19/09/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page | feature/subscriptions | 45f25028afb713b93cb8673a1ee5abdc9fe53594   | feat: add subscriptions.  |                     | 19/09/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page | feature/our-team      | d29df95ef29cdf224c966d07c8e8a15704647854   | feat: add our-team.       |                     | 19/09/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page | feature/Faqs          | 37f3b8c28d521878663c72a6ae046432deea790e   | feat: add Faqs.           |                     | 19/09/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page | feature/footer        | d09da40ecc996d11a3d84e31c003e4fa9d7bcf75   | feat: add footer.         |                     | 19/09/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page | feature/payment       | ff27629a30c625d174ef98b16b47b0a8ce97370a   | feat: add payment.        |                     | 19/09/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page | feature/js            | f83045d6a61811aab992b009689c67e2a3ed24e6   | feat: add files js.       |                     | 19/09/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page | feature/image         | f6cf2c1f36b63ab62729127683830a22fa1be8ba   | feat: add image.          |                     | 19/09/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page | feature/responsive    | 5d38b6997ae8e5326d8a96f618a460612610a6af   | feat: add responsive.     |                     | 20/09/2025         |

#### 5.2.2.5. Execution Evidence for Sprint Review

Durante el desarrollo del sprint se lograron completar todos los puntos planteados. A continuación se muestran evidencias del landing page logrado.



#### 5.2.2.6. Services Documentation Evidence for Sprint Review

El Sprint 2 de Energix se centró en la implementación funcional de la aplicación web, integrando la interfaz con una API desplegada que simula un backend mediante la estructura del archivo db.json para el consumo de información. Este avance permitió el desarrollo e integración de las vistas principales de la plataforma (Dashboard, Profile, Reports, etc.), garantizando coherencia visual y navegación fluida con el contenido dinámico simulado. Se habilitaron funcionalidades interactivas clave (como la edición de datos de usuario y la gestión por roles) y se reforzó la internacionalización (i18n). Aunque no se implementó una capa backend con lógica de negocio avanzada, la arquitectura utiliza endpoints REST que consumen db.json, sentando una base plenamente operativa y preparada para la posterior incorporación de la persistencia real y lógica de negocio.

#### 5.2.2.7. Software Deployment Evidence for Sprint Review

Durante este Sprint, se completó el desarrollo de la Landing Page y se realizó su despliegue utilizando GitHub Pages como plataforma de publicación gratuita. El objetivo fue contar con una primera versión accesible en línea del producto digital para revisión y retroalimentación.

Actividades realizadas: Se creó el repositorio en GitHub: https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page#

Se subió el código fuente de la Landing Page, incluyendo los archivos HTML, CSS necesarios.

Se configuró GitHub Pages desde la pestaña Settings > Pages, seleccionando la rama principal y la carpeta raíz.

Se verificó la correcta publicación de la Landing Page en la siguiente URL: https://energixlp.netlify.app

#### 5.2.2.8. Team Collaboration Insights during Sprint

En esta sección se evidencia la colaboración de cada integrante en el repositorio de la Landing Page.

Repositorio de Landing Page: https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page#

| **Integrante**                       | **Actividad**                                                                                          |  
|--------------------------------------|--------------------------------------------------------------------------------------------------------|
| **Huaman Olivos, Yeira Shari**       | Implementación de secciones de la **landing page** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |
| **Loechle Arias, Mateo Ítalo**       | Implementación de secciones de la **landing page** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |
| **Barturen Panez, Iker Gabriel**     | Implementación de secciones de la **landing page** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |
| **Encalada Salazar, Alexis**         | Implementación de secciones de la **landing page** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |
| **Torres Lavandera, Andrés Rodrigo** | Implementación de secciones de la **landing page** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |

**chapter 1, 2, 3, 4, 5.md**

# Conclusiones

### Conclusiones

El desarrollo del primer entregable del proyecto Energix ha permitido establecer una base metodológica, técnica y colaborativa sólida para la evolución del sistema SEMS. Se validaron hipótesis de diseño y se definió una visión clara de los objetivos, articulando un ecosistema funcional para la gestión inteligente de energía.

El enfoque Lean UX facilitó la identificación precisa de los principales retos de los usuarios propietarios de vivienda, estudiantes y soporte técnico, permitiendo comprender sus necesidades y expectativas mediante entrevistas, mapas de empatía, user personas y scenario mapping. Esto guió la propuesta de valor centrada en la experiencia del usuario.

La especificación y análisis de requisitos se realizó de forma rigurosa, aplicando técnicas modernas como To-Be Scenario Mapping, Impact Mapping, backlog grooming y user stories con criterios de aceptación. Esto permitió descomponer la solución en funcionalidades concretas y alineadas con los objetivos del negocio.

En cuanto al diseño visual y arquitectónico, se implementaron style guidelines, una arquitectura de información clara y una estructura modular basada en bounded contexts, siguiendo principios de Domain-Driven Design. Esto garantiza escalabilidad, mantenibilidad y separación de responsabilidades, reforzando la calidad técnica y la sostenibilidad del proyecto.

Durante el Sprint 1, se completaron las historias de usuario planificadas para la landing page, UI responsive, internacionalización y accesibilidad. El equipo demostró alta colaboración y cumplimiento de estándares técnicos, utilizando herramientas como GitHub, Figma, PlantUML y Netlify. La landing page fue desplegada y validada funcionalmente bajo criterios de usabilidad y accesibilidad.

Este primer sprint, centrado en la interfaz gráfica y experiencia inicial, sienta las bases para la futura implementación de servicios backend, APIs RESTful y microservicios modulares que conformarán el núcleo transaccional de la plataforma.

---

### Recomendaciones

- Mantener la sistematización en la gestión de requisitos y la validación continua con usuarios reales para asegurar la alineación con sus necesidades.
- Priorizar la escalabilidad y mantenibilidad en el diseño arquitectónico, reforzando la modularidad y separación de responsabilidades.
- Continuar aplicando principios de Lean UX y Domain-Driven Design en los siguientes sprints, especialmente en la integración de servicios backend y APIs.
- Fortalecer la colaboración y comunicación del equipo, promoviendo el uso de herramientas ágiles y buenas prácticas de desarrollo.
- Realizar pruebas de usabilidad y accesibilidad en cada iteración para garantizar una experiencia inclusiva y eficiente.
- Documentar exhaustivamente los avances y decisiones técnicas para facilitar la transferencia de conocimiento y el onboarding de nuevos miembros.

# Bibliografía



# Anexos

- Link de la Organización
  https://github.com/Upc-pre-1ASI0729-2520-7401-Energix
- Link del Figma
  https://www.figma.com/design/tmJAly092Cbckme5PFfA6Z/Energix?node-id=26-4210&t=4xEBZLNYgT1IM6IQ-1

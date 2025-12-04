# CapÃ­tulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management

En esta secciÃ³n, nuestro equipo establece las decisiones y convenciones para mantener una consistencia durante todo el desarrollo del proyecto. Estas convenciones son cruciales para asegurar que todos los miembros del equipo estÃ©n alineados en tÃ©rminos de uso de herramientas, buenas prÃ¡cticas y procesos de despliegue.

### 5.1.1. Software Development Environment Configuration

En este apartado se mencionan los distintos productos de software empleados por el equipo para llevar a cabo las actividades relacionadas con la elaboraciÃ³n del proyecto.

**Product UX/UI Desing**

1. **UXPressia:** https://uxpressia.com/Se utilizÃ³ para la creaciÃ³n de User Personas, Empathy Maps, Journey Maps e Impact Maps, proporcionando una visiÃ³n centrada en el usuario.

2. **Figma**: https://www.figma.com/Herramienta de diseÃ±o colaborativo utilizada para la creaciÃ³n de wireframes, mock-ups y prototipos de aplicaciones mÃ³viles y de escritorio.

**Software Development**

3. **Visual Studio Code**: https://code.visualstudio.com/Entorno de desarrollo ligero empleado para la creaciÃ³n del landing page y las aplicaciones web, utilizando HTML5, CSS3, JavaScript y TypeScript.

4. **WebStorm**: Entorno de desarrollo utilizado para trabajar con HTML, CSS, JavaScript y frameworks como Vue y Angular.

5. **Spring Boot Framework**:Framework utilizado para desarrollar servicios web RESTful en Java, proporcionando una base escalable y robusta.

6. **GitHub**: https://github.com/Plataforma de control de versiones utilizada para la gestiÃ³n del cÃ³digo fuente, aplicando el flujo de trabajo GitFlow para garantizar un desarrollo ordenado.

7. IntelliJ IDEA ultimate: https://www.jetbrains.com/es-es/idea/ Entorno de desarrollo utilizado para trabajar con Java, proporcionando una base escalable y robusta.
**Project Management and Collaboration**

8. **WhatsApp**: https://web.whatsapp.com/AplicaciÃ³n de mensajerÃ­a utilizada para la coordinaciÃ³n y discusiÃ³n de temas relacionados con el proyecto en tiempo real.

9. **Discord**: https://discord.com/ AplicaciÃ³n de mensajerÃ­a utilizada para la coordinaciÃ³n y discusiÃ³n de temas relacionados con el proyecto en tiempo real

**Software Documentation**

10. **LucidChart**: https://lucid.app/Plataforma utilizada para la creaciÃ³n de diagramas UML, wireflows y user flows, facilitando la visualizaciÃ³n y planificaciÃ³n del sistema.

11. **Structurizr**: https://www.structurizr.com/ Herramienta utilizada para modelar la arquitectura de software mediante diagramas C4, permitiendo un modelado claro de la estructura del proyecto.

**Software Testiong**

12. **Markdown**: Lenguaje de marcado ligero utilizado para documentar el proyecto y en los archivos README del repositorio de la organizaciÃ³n.

### 5.1.2. Source Code Management

La gestiÃ³n del cÃ³digo fuente es parte fundamental del desarrollo de cualquier proyecto de software, ya que nos permitirÃ¡ rastrear cambios, revertir versionas y coordinar a los diferentes integrantes del equipo a la misma vez. En ENERGIX, utilizaremos **GitHub** como plataforma para alojar nuestros repositorios.

**URL de los Repositorios**

- **Organization:** https://github.com/Upc-pre-1ASI0729-2520-7401-Energix
- **Reporte:** https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Energix-Proyect-Report
- **Landing Page:** https://energixlp.netlify.app
- **Frontend:** https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Frontend-SEMS 
- **Backend:** https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS 

**Commits Convencionales**

Para los mensajes de commit en el proyecto ENERGIX, se sigue la convenciÃ³n **Coventional Commits**. Estos mensajes deben seguir el formato estÃ¡ndar para facilitar la lectura y entendimiento del historial del proyecto:

``` githubexpressionlanguage
<type>[optional scope]:<decription>

[optional body]

[optional footer(s)]
```

- **Type**
-  -  ```feat```: Se usa cuando se aÃ±ade una nueva catacterÃ­stica.
-  -  ```fix```: Para la correciÃ³n de errores.
-  -  ```docs```: Modificaciones en la documentaciÃ³n.
-  -  ```style```: Cambios que no afectan la lÃ³gica del cÃ³digo, como los formatos o estilos.
-  -  ```refactor```: Modificaciones que no aÃ±aden caracterÃ­sticas ni corrigen errores.
-  -  ```test```: AddicÃ³n o modificaciÃ³n de pruebas.

- **Scope:** Proporciona informaciÃ³n adicional sobre el Ã¡rea del cÃ³digo afectada.

**Ejemplos de commits**

- ```feat(login): add user authentication module```
- ```fix(payment): resolve payment gateway issue```
- ```docs(README): update setup instructions```

Con estas estructuras, ENERGIX se puede gestionar eficientemente el flujo de trabajo del desarrollo, asegurÃ¡ndonos una integraciÃ³n continua y una organizaciÃ³n clara del cÃ³digo.

### 5.1.3. Source Code Style Guide & Conventions
En el proyecto ENERGIX, hemos implementaado una serie de guÃ­as de estilo y convenciones para asegurar que todo el equipo de desarrollo siga una estructura consistente y clara en todo el desarrollo del proyecto. Facilitando la legibidad del cÃ³digo, mejorando la colaboraciÃ³n entre los integrantes asegurando que el cÃ³digo sea mantenible a largo plazo.

**Nomenclatura General**

Para asegurar la coherencia en todo el cÃ³digo, seguiremos las siguientes directrices:

- Los nombres de variables, funciones y mÃ©todos deben utilizar **camelCase**.
- Los nombres de clases y componentes seguirÃ¡n la convenciÃ³n **PascalCase**.
- Para los archivos y carpetas, se emplearÃ¡ la convenciÃ³n **kebab-Case**.

El uso de **ingles** para todos los nombres es obligatorio, con el fin de asegurar la comprensiÃ³n entre los miembros del equipo y seguir las buenas prÃ¡cticas.

**Ejemplo**

- **Variables:** ``` home```,```userLocation```
- **Clases:** ``` HomeOwner```,```user```
- **Archivos:** ```home-owner.service.js```,```user.controller.js```

**Espacios y SangrÃ­as**

La sangrÃ­a de cÃ³digo en ENERGIX seguirÃ¡ las siguientes reglas para asegurar la claridad y el orden del cÃ³digo:

- Se utilizarÃ¡n **2 espacios** para la sangrÃ­a en archivos HTML, CSS, JavaScript, y TypeScript.
- En archivos **Java**, se utilizarÃ¡n **4 espacios** para la sangrÃ­a.

Esta convenciÃ³n ayuda a mantener la consistencia en todos los lenguajes empleados en el proyecto, facilitando la colaboraciÃ³n entre los diferentes miembros del equipo.

``` html
<!DOCTYPE html>
<html>
  <head>
    <title>Energix</title>
  </head>
  <body>
    <h1>Registros Disponible</h1>
    <p>Registra tus dispositivos fÃ¡cilmente</p>
  </body>
</html>
```

**Convenciones por Lenguaje**

1. HTML/CSS/JavaScript:

- - Se utilizarÃ¡ la Google HTML/CSS Style Guide (https://google.github.io/styleguide/htmlcssguide.html) para asegurar la consistencia en la estructura y la presentaciÃ³n de los archivos HTML y CSS.
- - Para JavaScript, adoptamos la Airbnb JavaScript Style Guide (https://google.github.io/styleguide/htmlcssguide.html), ampliamente conocida y utilizada en la industria.

2. TypeScript:

- - Angular es el framework elegido para el frontend de PARKINGNOW, por lo que seguimos la Angular Style Guide (https://v17.angular.io/guide/styleguide), que dicta cÃ³mo deben estructurarse los mÃ³dulos, servicios y componentes.
- - TambiÃ©n seguimos la Google TypeScript Style Guide (https://google.github.io/styleguide/tsguide.html) para garantizar la correcta tipificaciÃ³n y legibilidad del cÃ³digo.

3. Java:

- - En el backend, utilizamos Spring Boot para crear APIs y servicios web. Seguimos la Google Java Style Guide (https://google.github.io/styleguide/javaguide.html) para mantener consistencia en la estructura de las clases y los mÃ©todos.
- - Los nombres de clases serÃ¡n descriptivos, utilizando sustantivos para clases y verbos para mÃ©todos.

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
- - Para escribir los tests automatizados, seguimos la convenciÃ³n de Gherkin Syntax. (https://cucumber.io/docs/gherkin/) Esto permite una descripciÃ³n clara y precisa de los escenarios de prueba en los archivos .feature.
- - Utilizamos Given-When-Then para describir el comportamiento esperado en cada escenario.

**Ejemplo de Gherkin**

``` gherkin
Feature: Registro de dispositivo 

  Scenario: Registro exitosa
    Given el usuario ha iniciado sesiÃ³n
    When selecciona la opciÃ³n de dispositivos
    Then el usuario debe configurar el dispositivo a registrar
    Then el sistema debe confirmar el registro
    
```

**Espacios y Comillas**

- **Espacios:** Siempre se debe colocar un espacio alrededor de los operadores y entre los parÃ¡metros en las funciones.

**Ejemplo:**

``` typescript

let totalDevices = 50;
let devicesRegistered = 10;
let availableSpace = totalDevices - devicesRegistered;
 
```
- **Commillas:** En **JavaScript** y **TypeScript**, se utilizan comillas simples ```(')``` para cadenas, mientras que en **HTML** se prefieren las comillas dobles ```(")```.

**Limite de Longitud de LÃ­nea**

El cÃ³digo no debe exceder las 80 columnas por lÃ­neas. En caso de necesitar mÃ¡s espacios, se recomienda dividir la lÃ­nea de cÃ³digo para mejorar la legibilidad.
### 5.1.4. Software Deployment Configuration
- En esta secciÃ³n se detalla la configuraciÃ³n necesaria para el despliegue de la soluciÃ³n ENERGIX, incluyendo los pasos claves para lograr la publicaciÃ³n satisfactoria de la Landing Page, Servicios Web y Aplicaciones Web Frontend utilizando Netlify para visualizar cada commit del Landing Page.

- A continuaciÃ³n, se describen los pasos para realizar el despliegue de la Landing Page del proyecto ENERGIX.- 1- **ActualizaciÃ³n de Ramas**: AsegÃºrate de que todas las ramas del repositorio estÃ©n actualizadas. Luego, ingresa a Github y dirÃ­gete al repositorio del proyecto ENERGIX.
1. **ActualizaciÃ³n de Ramas**: AsegÃºrate de que todas las ramas del repositorio estÃ©n actualizadas. Luego, ingresa a Netlify y dirÃ­gete al repositorio del proyecto ENERGIX.
2. **Acceso a las configuraciones**: Una vez dentro de Netifly, haz click en la pestaÃ±a Get Started en el centro de la pantalla, te loqueas con Git Hub, buscas la organizaciÃ³n y el repositorio de tu landign page y la selecciones.
3. **SelecciÃ³n de la ConfiguraciÃ³n**: Selecciona la configuraciÃ³n y carga los archivos del repositorio. Esta opciÃ³n permite generar el link de la landing page, con el nombre Energix.
4. **Acceso a la pÃ¡gina**: Finalmente, podrÃ¡s acceder a la Landing Page desde el enlace que se generÃ³ al finalizar el deploy. AquÃ­ estÃ¡ el enlace para el proyecto ENERGIX: https://energixlp.netlify.app

### 5.2.1. Sprint 1

#### 5.2.1.1. Sprint Planning 1

Para este primer sprint nos enfocaremos en los tasks para la
elaboraciÃ³n de la Landing Page. Nos dividiremos entre nosotros cada
una de las tareas identificadas para el sprint.

| Sprint 1 | Sprint 1 |
| :--- | :--- |
| **Sprint Planning Background** | |
| **Date** | 2025-09-15 |
| **Time** | 4:30 PM |
| **Location** | Via Discord |
| **Prepared By** | Iker Gabriel Barturen Panez |
| **Attendees (to planning meeting)** | Alexis Encalada Salazar, Yeira Shari Huaman Olivos, AndrÃ©s Rodrigo Torres Lavandera, Iker Gabriel Barturen Panez, Mateo Italo Loechle Arias |
| **Sprint 1 Review Summary** | En esta primera secciÃ³n se planteo el desarrollo de la Landing Page y planeaciÃ³n de aplicaciÃ³n para el proyecto de Energix. |
| **Sprint 1 Retrospective Summary** | En esta secciÃ³n todos los integrantes mencionaron tener aciertos en partes del codigo y en otras partes poder mejorar sus habilidades realizando la Landing Page |
| **Sprint Goal & User Stories** | |
| **Sprint 1 Goal** | Desarrollar y desplegar una landing page que presente informaciÃ³n a los usuarios a travÃ©s de imÃ¡genes y texto. La pÃ¡gina debe ser completamente adaptable a cualquier tipo de dispositivo que utilicen los usuarios, garantizando una experiencia de usuario fluida y responsiva. |
| **Sprint 1 Velocity** | 5 story points |
| **Sum of Story Points** | 5 Story Points |

#### 5.2.1.2. Aspect Leaders and Collaborators

Con la finalidad de mejorar la colaboraciÃ³n en equipo a cada integrante se asignÃ³ un rol de lÃ­der por cada aspecto. Los aspectos estÃ¡n relacionados con los entregables.

| Team member (LastName, First Name) | GitHub UserName       | Aspect 1: Landing Page Leader (L) / Collaborator (C) | Aspect 2: DiseÃ±os Figma: Leader (L) / Collaborator (C) | Aspect 3: Reporte (L) / Collaborator (C) |
|------------------------------------|-----------------------|------------------------------------------------------|--------------------------------------------------------|------------------------------------------|
| Alexis Encalada                    | Alexiz248             | C                                                    | C                                                      | L                                        |
| Yeira Sharia                       | YeiShari              | L                                                    | L                                                      | L                                        |
| AndrÃ©s Torres                      | AndresTorres202312557 | C                                                    | L                                                      | L                                        |
| Iker Barturen                      | krxxg04               | L                                                    | L                                                      | L                                        |
| Mateo Loechle                      | LowMathzzz            | C                                                    | C                                                      | L                                        |
| Jafeth Ynga                        | Jafeth-MV             | C                                                    | C                                                      | C                                        |

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
    <td colspan="2">DiseÃ±ar secciÃ³n de propuesta de valor</td>
    <td colspan="3">Implementar la secciÃ³n en la landing page con diseÃ±o atractivo y responsivo.</td>
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
    <td colspan="2">Implementar secciÃ³n FAQ</td>
    <td colspan="3">Desarrollar componente visual (acordeÃ³n/collapsible) para mostrar las preguntas frecuentes.</td>
    <td>2h</td>
    <td colspan="2">Yeira Huaman</td>
    <td>Done</td>
  </tr>
  <tr>
    <td>US33</td>
    <td colspan="2">Revisar planes de suscripciÃ³n</td>
    <td>UT05</td>
    <td colspan="2">Redactar informaciÃ³n de planes</td>
    <td colspan="3">Crear contenido sobre los distintos planes, precios y beneficios.</td>
    <td>3h</td>
    <td colspan="2">AndrÃ©s Torres</td>
    <td>Done</td>
  </tr>
  <tr>
    <td></td>
    <td colspan="2"></td>
    <td>UT06</td>
    <td colspan="2">Implementar secciÃ³n de comparaciÃ³n de planes</td>
    <td colspan="3">DiseÃ±ar tabla o cards para comparar los planes en la landing page.</td>
    <td>3h</td>
    <td colspan="2">AndrÃ©s Torres</td>
    <td>Done</td>
  </tr>
  <tr>
    <td>US34</td>
    <td colspan="2">Consultar informaciÃ³n del equipo</td>
    <td>UT07</td>
    <td colspan="2">Redactar informaciÃ³n del equipo</td>
    <td colspan="3">Crear contenido sobre la misiÃ³n, visiÃ³n y miembros del equipo.</td>
    <td>2h</td>
    <td colspan="2">Alexis Encalada</td>
    <td>Done</td>
  </tr>
  <tr>
    <td></td>
    <td colspan="2"></td>
    <td>UT08</td>
    <td colspan="2">Implementar secciÃ³n del equipo</td>
    <td colspan="3">DiseÃ±ar e integrar la secciÃ³n del equipo en la landing page.</td>
    <td>2h</td>
    <td colspan="2">Alexis Encalada</td>
    <td>Done</td>
  </tr>
  <tr>
    <td>US35</td>
    <td colspan="2">Cambiar idioma</td>
    <td>UT09</td>
    <td colspan="2">Implementar selector de idioma</td>
    <td colspan="3">Desarrollar funcionalidad para cambiar entre espaÃ±ol e inglÃ©s en la landing page.</td>
    <td>4h</td>
    <td colspan="2">Mateo Italo</td>
    <td>Done</td>
  </tr>
</table>

#### 5.2.1.4. Development Evidence for Sprint Review

En esta secciÃ³n se demuestran los commits relacionados con los principales avances en la implementaciÃ³n.
Estos commits provienen del repositorio del Landing Page de la organizaciÃ³n de GitHub.

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

Durante el desarrollo del sprint se lograron completar todos los puntos planteados. A continuaciÃ³n se muestran evidencias del landing page logrado.

![Barra-de-Navegacion.png](../chapter-04/assets/Barra-de-Navegacion.png)
![Inicio.png](../chapter-04/assets/Inicio.png)
![Beneficios.png](../chapter-04/assets/Beneficios.png)
![Producto.png](../chapter-04/assets/Producto.png)
![Suscripciones.png](../chapter-04/assets/Suscripciones.png)
![About-the-Team.png](../chapter-04/assets/About-the-Team.png)
![Nuestro-Equipo.png](../chapter-04/assets/Nuestro-Equipo.png)
![Preguntas-Frecuentes.png](../chapter-04/assets/Preguntas-Frecuentes.png)
![Footer.png](../chapter-04/assets/Footer.png)


#### 5.2.1.6. Services Documentation Evidence for Sprint Review

Como se mencionÃ³ previamente, Este sprint solo tuvo como objetivo el desarrollo de Landing Page. AÃºn no se han implementado ni documentado Endpoints con OpenAPI, ya que el desarrollo de los servicios web estÃ¡ planificado para los siguientes Sprints, conforme al roadmap del proyecto.

#### 5.2.1.7. Software Deployment Evidence for Sprint Review

Durante este Sprint, se completÃ³ el desarrollo de la Landing Page y se realizÃ³ su despliegue utilizando GitHub Pages como plataforma de publicaciÃ³n gratuita. El objetivo fue contar con una primera versiÃ³n accesible en lÃ­nea del producto digital para revisiÃ³n y retroalimentaciÃ³n.

Actividades realizadas: Se creÃ³ el repositorio en GitHub: https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page#

Se subiÃ³ el cÃ³digo fuente de la Landing Page, incluyendo los archivos HTML, CSS necesarios.

Se configurÃ³ GitHub Pages desde la pestaÃ±a Settings > Pages, seleccionando la rama principal y la carpeta raÃ­z.

Se verificÃ³ la correcta publicaciÃ³n de la Landing Page en la siguiente URL: https://energixlp.netlify.app

#### 5.2.1.8. Team Collaboration Insights during Sprint

En esta secciÃ³n se evidencia la colaboraciÃ³n de cada integrante en el repositorio de la Landing Page.

Repositorio de Landing Page: https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page#

| **Integrante**                       | **Actividad**                                                                                          |  
|--------------------------------------|--------------------------------------------------------------------------------------------------------|
| **Huaman Olivos, Yeira Shari**       | ImplementaciÃ³n de secciones de la **landing page** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |
| **Loechle Arias, Mateo Ãtalo**       | ImplementaciÃ³n de secciones de la **landing page** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |
| **Barturen Panez, Iker Gabriel**     | ImplementaciÃ³n de secciones de la **landing page** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |
| **Encalada Salazar, Alexis**         | ImplementaciÃ³n de secciones de la **landing page** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |
| **Torres Lavandera, AndrÃ©s Rodrigo** | ImplementaciÃ³n de secciones de la **landing page** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |
| **Ynga Amado, Jafeth Worren**        | ImplementaciÃ³n de secciones de la **landing page** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |

![NetLP.png](assets/NetLP.png) 
### 5.2.2. Sprint 2

#### 5.2.2.1. Sprint Planning 2

Durante el Sprint 2 se estableciÃ³ el desarrollo de la aplicaciÃ³n web de la plataforma Energix, enfocÃ¡ndose en la implementaciÃ³n de las principales vistas y funcionalidades orientadas a los perfiles propietarios de viviendas y universitarios que alquilan. El trabajo incluyÃ³ la integraciÃ³n de la interfaz con la base de datos, la gestiÃ³n dinÃ¡mica de la informaciÃ³n de usuario y la mejora de la experiencia visual y de navegaciÃ³n. Asimismo, se priorizÃ³ la internacionalizaciÃ³n (i18n) y la coherencia del diseÃ±o, consolidando una versiÃ³n funcional y estable del sistema.

| Sprint 2 | Sprint 2 |
| :--- | :--- |
| **Sprint Planning Background** | |
| **Date** | 2025-09-29 |
| **Time** | 6:30 PM |
| **Location** | Via Discord |
| **Prepared By** | Iker Gabriel Barturen Panez |
| **Attendees (to a planning meeting)** | Alexis Encalada Salazar, Yeira Shari Huaman Olivos, Andrés Rodrigo Torres Lavandera, Iker Gabriel Barturen Panez, Mateo Italo Loechle Arias |
| **Sprint Goal & User Stories** | |
| **Sprint 2 Goal** | Implementar y estabilizar la arquitectura fundamental de la aplicación web Energix, entregando la capa de presentación funcionalmente integrada a la base de datos para las vistas centrales y la gestión de datos de los perfiles de usuario (propietarios de viviendas y universitarios que alquilan), con soporte inicial para internacionalización (i18n). |
| **Sprint 2 Velocity** | 10 |
| **Sum of Story Points** | 89 |

#### 5.2.2.2. Aspect Leaders and Collaborators

Con la finalidad de mejorar la colaboraciÃ³n en equipo a cada integrante se asignÃ³ un rol de lÃ­der por cada aspecto. Los aspectos estÃ¡n relacionados con los entregables.

| Team member (LastName, First Name) | GitHub UserName       | Aspect 1: Dashboard & Devices View | Aspect 2: Profile View and UI Design | Aspect 3: Reports View | Aspect 4: Notifications View | Aspect 5: Settings View |
|------------------------------------|-----------------------|------------------------------------|--------------------------------------------------------------------|------------------------|------------------------------|-------------------------|
| Alexis Encalada                    | Alexiz248             | C                                  | C                                                                  | C                      | C                            | L                       |
| Yeira Sharia                       | YeiShari              | C                                  | L                                                                  | C                      | C                            | C                       |
| AndrÃ©s Torres                      | AndresTorres202312557 | C                                  | C                                                                  | L                      | C                            | C                       |
| Iker Barturen                      | krxxg04               | L                                  | C                                                                  | C                      | C                            | C                       |
| Mateo Loechle                      | LowMathzzz            | C                                  | C                                                                  | C                      | L                            | C                       |
| Jafeth Ynga                        | Jafeth-MV             | C                                  | C                                                                  | C                      | C                            | C                       |

#### 5.2.2.3. Sprint Backlog 2
| Sprint 2 – Work Items / Tasks (Aplicación Web Energix) | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **User Story ID** | **Task ID** | **Title** | **Description** | **Estimation** | **Assigned To** | **Status** |
| **EP01 – Autenticación y Perfil de Usuario** | | | | | | |
| US01 | UT01 | Diseñar formulario de registro | Diseñar el formulario con campos de correo, contraseña y validación. | 3h | Yeira Huamán | Done |
| | UT02 | Implementar backend de registro | Crear endpoint de registro y validaciones de correo duplicado. | 4h | Mateo Loechle | Done |
| US02 | UT03 | Implementar inicio de sesión | Crear pantalla de login y autenticación JWT. | 3h | Iker Barturen | Done |
| | UT04 | Manejo de errores en login | Mostrar mensajes por credenciales inválidas o usuario inexistente. | 2h | Yeira Huamán | Done |
| US03 | UT05 | Configurar perfil inicial | Crear formulario de configuración inicial (tipo de vivienda, dispositivos). | 3h | Andrés Torres | Done |
| | UT06 | Validar configuración | Verificar información incompleta en perfil inicial. | 2h | Alexis Encalada | Done |
| US04 | UT07 | Flujo de recuperación de contraseña | Crear formulario para restablecer contraseña y envío de correo. | 3h | Yeira Huamán | Done |
| | UT08 | Actualizar contraseña desde enlace | Implementar vista para establecer nueva contraseña. | 2h | Mateo Loechle | Done |
| US05 | UT09 | Implementar cierre de sesión | Desarrollar logout seguro y cierre automático por inactividad. | 3h | Iker Barturen | Done |
| **EP02 – Conexión y Monitoreo de Dispositivos** | | | | | | |
| US06 | UT10 | Vincular dispositivos | Crear flujo para conectar dispositivos compatibles con la plataforma. | 4h | Alexis Encalada | Done |
| | UT11 | Validar compatibilidad | Mostrar error si el dispositivo no es compatible. | 2h | Mateo Loechle | Done |
| US07 | UT12 | Identificación automática | Implementar reconocimiento automático de dispositivos conectados. | 3h | Yeira Huamán | Done |
| | UT13 | Definición manual | Permitir al usuario definir dispositivo si no se identifica. | 2h | Alexis Encalada | Done |
| US08 | UT14 | Monitoreo en tiempo real | Mostrar consumo en tiempo real de dispositivos conectados. | 4h | Iker Barturen | Done |
| | UT15 | Manejo de desconexiones | Notificar al usuario cuando un dispositivo se desconecta. | 2h | Yeira Huamán | Done |
| **EP03 – Alertas y Recordatorios de Consumo** | | | | | | |
| US09 | UT16 | Alertas de consumo elevado | Configurar sistema de alertas automáticas por exceso de consumo. | 3h | Mateo Loechle | Done |
| | UT17 | Registrar alertas | Guardar las alertas generadas con fecha y hora. | 2h | Andrés Torres | Done |
| US10 | UT18 | Recordatorios por inactividad | Enviar notificaciones para desconectar dispositivos en reposo. | 3h | Alexis Encalada | Done |
| | UT19 | Configuración de recordatorios | Permitir ajustar frecuencia de avisos. | 2h | Yeira Huamán | Done |
| US11 | UT20 | Configurar umbrales personalizados | Definir límites de consumo por usuario y restablecimiento a valores predeterminados. | 4h | Iker Barturen | Done |
| **EP04 – Reportes y Facturación** | | | | | | |
| US12 | UT21 | Reporte semanal | Generar reporte semanal del consumo energético en PDF. | 4h | Mateo Loechle | Done |
| US13 | UT22 | Comparación entre periodos | Permitir comparar consumo entre semanas o meses con gráficos. | 3h | Yeira Huamán | Done |
| US14 | UT23 | Proyección de factura | Estimar factura mensual según consumo actual. | 3h | Andrés Torres | Done |
| US15 | UT24 | Historial de consumo mensual | Mostrar historial mensual de consumo y descarga en PDF. | 3h | Alexis Encalada | Done |
| **EP05 – Metas y Ahorro Energético** | | | | | | |
| US16 | UT25 | Recomendaciones personalizadas | Mostrar consejos adaptados al patrón de consumo del usuario. | 3h | Yeira Huamán | Done |
| US17 | UT26 | Metas de ahorro | Configurar metas mensuales y seguimiento de progreso. | 4h | Iker Barturen | Done |
| US18 | UT27 | Comparar consumo con otros usuarios | Mostrar comparación con hogares similares y ranking de eficiencia. | 3h | Mateo Loechle | Done |
| US19 | UT28 | Programar encendido automático | Permitir programación de horarios de encendido de dispositivos. | 3h | Alexis Encalada | Done |
| US20 | UT29 | Programar apagado automático | Implementar apagado programado para reducir consumo innecesario. | 3h | Andrés Torres | Done |
| **EP06 – Soporte y Asesoría** | | | | | | |
| US21 | UT30 | Solicitar asesoría | Permitir al usuario agendar sesiones con especialistas. | 3h | Yeira Huamán | Done |
| US22 | UT31 | Centro de ayuda | Implementar sección con guías y artículos de ayuda. | 3h | Mateo Loechle | Done |
| US23 | UT32 | Contactar soporte | Crear formulario de contacto y recepción de respuestas. | 3h | Iker Barturen | Done |
| **EP07 – Gestión de Categorías de Dispositivos** | | | | | | |
| US24 | UT33 | Agrupar dispositivos | Permitir al usuario crear categorías personalizadas de dispositivos. | 3h | Alexis Encalada | Done |
| US25 | UT34 | Consumo por categoría | Mostrar consumo agrupado y comparativo por categoría. | 4h | Yeira Huamán | Done |
| US26 | UT35 | Dispositivos de alto consumo | Identificar y alertar sobre los dispositivos con mayor gasto energético. | 3h | Andrés Torres | Done |
| **EP08 – Multiusuario y Roles** | | | | | | |
| US27 | UT36 | Administrar múltiples cuentas | Permitir agregar miembros al hogar y compartir gestión. | 3h | Mateo Loechle | Done |
| US28 | UT37 | Definir roles de acceso | Implementar control de permisos (administrador/invitado). | 3h | Iker Barturen | Done |
| **EP09 – Noticias e Internacionalización** | | | | | | |
| US29 | UT38 | Cambiar idioma de la aplicación | Implementar selector de idioma con persistencia de preferencia. | 3h | Yeira Huamán | Done |
| US30 | UT39 | Noticias y consejos | Agregar sección de noticias con artículos y recomendaciones. | 4h | Alexis Encalada | Done |



#### 5.2.2.4. Development Evidence for Sprint Review

En esta secciÃ³n se demuestran los commits relacionados con los principales avances en la implementaciÃ³n.
Estos commits provienen del repositorio de la aplicaciÃ³n web de la organizaciÃ³n de GitHub.

Enlace al repositorio de la aplicaciÃ³n web: https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Frontend-SEMS

| Repository                                        | Branch                      | Commit Id                                  | Commit Message                  | Commit Message Body | Commited on (Date) |
|---------------------------------------------------|-----------------------------|--------------------------------------------|---------------------------------|---------------------|--------------------|
| Upc-pre-1ASI0729-2520-7401-Energix/Fronten-SEMS   | feature/ddd                 | 069e2cb5286f9ad8d996f8924e67be96575b5b09   | feat: add domain driven desing. |                     | 02/10/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Fronten-SEMS   | feature/addAunthentication  | 5ea94a4d17e60a53db5830b42eb1a989d9d38e03   | feat: add aunthentication.      |                     | 03/10/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Fronten-SEMS   | feature/update-login        | 48d68c1ff07a03a224a3dd4b0f2603be367f48a6   | feat: add update login.         |                     | 03/10/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Fronten-SEMS   | feature/add-dashboard       | 3dc92d1346c082774d9853a2fffa1d8f483a24fd   | feat: add dashboard.            |                     | 04/10/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Fronten-SEMS   | feature/server              | a3bfb8dd3bf8e2192dacd74ae6eaa5e7be0d4dae   | feat: add server.               |                     | 04/10/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Fronten-SEMS   | feature/server              | 430f5da64e6b67c5fa64716becd212675678e94e   | feat: add config server.        |                     | 05/10/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Fronten-SEMS   | feature/reports             | 87102a704126e9ba3d7f0302ae489a3d5f3d1db1   | feat: add device chart.         |                     | 05/10/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Fronten-SEMS   | feature/config-app-routes   | c21124db6bc7563e1421f46e6f139a6f545d5e74   | feat: add config routes.        |                     | 05/10/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Fronten-SEMS   | feature/consumption         | d8ab0155901192167c0d100b4558ac43ff596b25   | Feature/consumption             |                     | 05/10/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Fronten-SEMS   | feature/notification        | 86fde845c4afdd0b68dd2887bc2a0d2ec55c2be8   | Feature/notification merging.   |                     | 05/10/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Fronten-SEMS   | feature/devices             | 38c0aea980d68cc380d86847fabf9f01d0325d97   | feat:add devices window.        |                     | 05/10/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Fronten-SEMS   | feature/devices-preferences | 375acbac860fa2204dd7db6f6c0f42959937ff6a   | feat: add devices preferences.  |                     | 06/10/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Fronten-SEMS   | feature/settings            | 07cb159ed1c5af5df5312a2ef30b9c950302ebe0   | Feature/settings                |                     | 06/10/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Fronten-SEMS   | feature/profile             | 64f6e18251d73801245b50c243d8dda88fb6e3e3   | Feature/profile                 |                     | 07/10/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Fronten-SEMS   | feature/export-report       | bbd27b1cd2ba3b987ecb1b3a3cb026053e9bb661   | feat: update export report      |                     | 07/10/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Fronten-SEMS   | feature/db.config           | d563c430f96bdc863fb30ef0742154c4de920735   | feat: config httpclient.        |                     | 08/10/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Fronten-SEMS   | feature/home-translation    | 15c6f68e4ced7c9c7519d43ee1074ab6b205a8b0   | feat: update home.              |                     | 08/10/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Fronten-SEMS   | feature/-deploy-api         | 09765b5d78094dba4715ad95fb7afab260b0e3c7   | feat: update json-server.       |                     | 09/10/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Fronten-SEMS   | feature/update-fakeapi      | 0c9d780777036f6c43edb15a8401b533fb31bf04   | feat: changed .env api url      |                     | 09/10/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Fronten-SEMS   | feature/realese-1.0         | d56c76e06c621c06de108b7db4c78dc89c4b490f   | feat: update api_url            |                     | 09/10/2025         |

#### 5.2.2.5. Execution Evidence for Sprint Review

Durante el desarrollo del sprint se lograron completar todos los puntos para la implementaciÃ³n de las funcionalidades esenciales para el sistema de gestiÃ³n Energix, estableciendo una base sÃ³lida para la administraciÃ³n de energÃ­a en los hogares. Las principales caracterÃ­sticas desarrolladas fueron:

1. Sistema de autenticaciÃ³n completo con diferentes campos para rellenar segÃºn el rol del usuario, si es dueÃ±o o estudiante.

2. PersonalizaciÃ³n de perfil, permitiendo al usaurio modificar a su preferencia su experiencia en la aplicaciÃ³n.    

3. VisualizaciÃ³n y descarga de reportes, con la posibilidad de filtrar por fecha y tipo de reporte y poder descargar los datos acumulados en diferentes formatos.

4. GestiÃ³n de dispositivos, facilitando el control entre los diferentes dispositivos registrados.

5. InternalizaciÃ³n (i18n) para soportar dos idiomas en la plataforma.

6. Cierre se sesiÃ³n seguro, permitiendo al usuario salir de la aplicaciÃ³n de manera segura y facil, dandole la optortunidad al usaurio de inicar sesiÃ³n con las mismas credenciales.   

7. Sistema de navegaciÃ³n robusto entre pÃ¡ginas con manejo de rutas protegidas y pÃ¡gina 4040 personalizada. 

**Capturas de pantalla de las principales vistas**


Login y AuntenticaciÃ³n

![login.png](assets/login.png)

Dashboard principal

![dashboard.png](assets/dashboard.png)

Mis dispositivos

![devices.png](assets/devices.png)

Reportes

![reports.png](assets/reports.png)

ConfiguraciÃ³n

![configuration.png](assets/configuration.png)


#### 5.2.2.6. Services Documentation Evidence for Sprint Review

IntroducciÃ³n

Durante el sprint 2, hemos implementado una estrategia de despliegue completa para el sistema de Energix, abarcando tanto el frontend como los servicios de backend que soportan la aplicaciÃ³n. Nuestro enfoque principal ha sido crear una infraestuctura robusta y unificada que facilite tanto el desarrollo como la experiencia del usuario final.

**ImplementaciÃ³n de API centralizada en render**

Decidimos migrar de una arquitectura distribuida con multiples enpoints a una soluciÃ³n mÃ¡s centralizada y mÃ¡s robusta utilizando Render. Esta desiciÃ³n nos permitiÃ³ superar las limitaciones al momento de llamar a la API y tener un mayor control sobre nuestra infraestructura.

La URL base para todos los recurso de nuestra API ahora es:

https://sems-fake-api.onrender.com/

Esta URL base sirve como punto de entrada principal para todos los recursos del sistema, simplificando considerablemente la configuraciÃ³n y mantenimiento de la aplicaciÃ³n.

**ConfiguraciÃ³n del servidor en Render**

El proceso de implementaciÃ³n en Render involucrÃ³ varias etapas para asegurar un despliegue exitoso. Comenzamos creando una nueva cuenta y proyecto en la plataforma, configurÃ¡ndolo especÃ­ficamente para trabajar con Node.js como entorno de ejecuciÃ³n.

Conectamos nuestro repositorio de GitHub para habilitar el despliegue automÃ¡tico, lo que nos permite mantener sincronizado el entorno de producciÃ³n con la rama principal del proyecto. Esto ha resultado en un flujo de trabajo mÃ¡s eficiente, donde cada merge a la rama principal actualiza automÃ¡ticamente nuestra API.

| MÃ©todo HTTP | Endpoint               | DescripciÃ³n                                            | Ejemplo de uso                             |
|-------------|------------------------|--------------------------------------------------------|--------------------------------------------|
| GET         | /users                 | Obtiene todos los usuarios                             | Listar supervisores o tÃ©cnicos registrados |
| GET         | /users/:id             | Obtiene un usuario especÃ­fico                          | Consultar datos de un usuario              |
| POST        | /users                 | Crea un nuevo usuario                                  | Registrar nuevo supervisor o tÃ©cnico       |
| PUT         | /users/:id             | Actualiza datos de un usuario                          | Modificar informaciÃ³n de contacto          |
| DELETE      | /users/:id             | Elimina un usuario existente                           | Dar de baja a un supervisor                |
| GET         | /dashboardStas         | Obtiene estadÃ­sticas del panel principal               | Visualizar mÃ©tricas generales del sistema  |
| GET         | /deilyConsumption      | Obtiene consumo diario de energÃ­a o recursos           | Mostrar grÃ¡fico de consumo del dÃ­a         |
| GET         | /consumptionByCategory | Obtiene consumo dividido por categorÃ­as                | Comparar consumo entre Ã¡reas o tipos       |
| GET         | /monthlyComparasion    | Obtiene comparaciÃ³n mensual de consumo                 | Ver evoluciÃ³n del consumo mes a mes        |
| GET         | /devices               | Obtiene lista de dispositivos registrados              | Listar sensores o equipos conectados       |
| POST        | /devices               | Agrega un nuevo dispositivo                            | Registrar sensor o medidor nuevo           |
| PUT         | /device/:id            | Actualiza un dispositivo existente                     | Editar nombre o estado de un dispositivo   |
| DELETE      | /device/:id            | Elimina un dispositivo                                 | Dar de baja un sensor fuera de servicio    |
| GET         | /alerts                | Obtiene lista de alertas activas                       | Mostrar alertas de consumo o fallos        |
| GET         | /notification          | Obtiene notificaciones generadas                       | Mostrar avisos al usuario                  |
| GET         | /devicePreferences     | Obtiene configuraciÃ³n de preferencias por dispositivo  | Mostrar ajustes personalizados             |


#### 5.2.2.7. Software Deployment Evidence for Sprint Review

Durante este Sprint, se completÃ³ el desarrollo de la aplicaciÃ³n web y se realizÃ³ su despliegue utilizando vercel app como plataforma de publicaciÃ³n gratuita. El objetivo fue contar con una primera versiÃ³n accesible en lÃ­nea del producto digital para revisiÃ³n y retroalimentaciÃ³n.

Actividades realizadas: Se creÃ³ el repositorio en Git hub: https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Frontend-SEMS

Se subiÃ³ el cÃ³digo fuente de la aplicaciÃ³n, incluyendo los archivos html, .Vue, CSS, ts, .json  necesarios.

Se configurÃ³ en vercel app para el deploy de la app web.

Se verificÃ³ la correcta publicaciÃ³n de la aplicaciÃ³n web en la siguiente URL: https://frontend-sems.vercel.app

#### 5.2.2.8. Team Collaboration Insights during Sprint

En esta secciÃ³n se evidencia la colaboraciÃ³n de cada integrante en el repositorio del Frontend de la AplicaciÃ³n Web.

Repositorio del Frontend de la AplicaciÃ³n Web: https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Frontend-SEMS

| **Integrante**                       | **Actividad**                                                                                                         |  
|--------------------------------------|-----------------------------------------------------------------------------------------------------------------------|
| **Huaman Olivos, Yeira Shari**       | ImplementaciÃ³n de secciones del **Frontend de la AplicaciÃ³n Web** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |
| **Loechle Arias, Mateo Ãtalo**       | ImplementaciÃ³n de secciones del **Frontend de la AplicaciÃ³n Web** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |
| **Barturen Panez, Iker Gabriel**     | ImplementaciÃ³n de secciones del **Frontend de la AplicaciÃ³n Web** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |
| **Encalada Salazar, Alexis**         | ImplementaciÃ³n de secciones del **Frontend de la AplicaciÃ³n Web** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |
| **Torres Lavandera, AndrÃ©s Rodrigo** | ImplementaciÃ³n de secciones del **Frontend de la AplicaciÃ³n Web** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |
| **Ynga Amado, Jafeth Worren**        | ImplementaciÃ³n de secciones del **Frontend de la AplicaciÃ³n Web** y contribuciones a los **chapter 1, 2, 3, 4, 5.md** |

![commits.png](assets/commits.png)

![contributors.png](assets/contributors.png)

![gitflow1.png](assets/gitflow1.png)

![gitflow2.png](assets/gitflow2.png)

![gitflow3.png](assets/gitflow3.png)

### 5.2.3. Sprint 3

#### 5.2.3.1. Sprint Planning 3

Durante el Sprint 3 se desarrollÃ³ el backend correspondiente al frontend implementado en el Sprint 2 de la plataforma SEMS, enfocÃ¡ndose en la implementaciÃ³n de las APIs principales y funcionalidades del servidor orientadas a los perfiles propietarios de viviendas y universitarios que alquilan. El trabajo incluyÃ³ la integraciÃ³n con la base de datos, la gestiÃ³n dinÃ¡mica de la informaciÃ³n de usuario a travÃ©s del backend y la consolidaciÃ³n de una versiÃ³n funcional y estable del sistema, desplegado en Render.

| Sprint 3 | Sprint 3 |
| :--- | :--- |
| **Sprint Planning Background** | |
| **Date** | 2025-11-07 |
| **Time** | 4:30 PM |
| **Location** | Via Discord |
| **Prepared By** | Iker Gabriel Barturen Panez |
| **Attendees (to a planning meeting)** | Alexis Encalada Salazar, Yeira Shari Huaman Olivos, Andrés Rodrigo Torres Lavandera, Iker Gabriel Barturen Panez, Mateo Italo Loechle Arias |
| **Sprint Goal & User Stories** | |
| **Sprint 3 Goal** | Implementar y estabilizar la arquitectura fundamental del backend de la aplicación web Energix, entregando la capa de servidor funcionalmente integrada a la base de datos para las APIs centrales y la gestión de datos de los perfiles de usuario (propietarios de viviendas y universitarios que alquilan), con soporte inicial. |
| **Sprint 3 Velocity** | 10 |
| **Sum of Story Points** | 89 |

#### 5.2.3.2. Aspect Leaders and Collaborators

Con la finalidad de mejorar la colaboraciÃ³n en equipo a cada integrante se asignÃ³ un rol de lÃ­der por cada aspecto. Los aspectos estÃ¡n relacionados con los entregables.

| Team member (LastName, First Name) | GitHub UserName       | Aspect 1: Backend for Dashboard, Devices & Authentication | Aspect 2: Profile View  | Aspect 3: Backend for Reports | Aspect 4: Backend for Notifications | Aspect 5: Backend for Settings |
|------------------------------------|-----------------------|-----------------------------------------------------------|-------------------------|-------------------------------|-------------------------------------|--------------------------------|
| Alexis Encalada                    | Alexiz248             | C                                                         | C                       | C                             | C                                   | L                              |
| Yeira Sharia                       | YeiShari              | C                                                         | L                       | C                             | C                                   | C                              |
| AndrÃ©s Torres                      | AndresTorres202312557 | C                                                         | C                       | L                             | C                                   | C                              |
| Iker Barturen                      | krxxg04               | L                                                         | C                       | C                             | C                                   | C                              |
| Mateo Loechle                      | LowMathzzz            | C                                                         | C                       | C                             | L                                   | C                              |

#### 5.2.3.3. Sprint Backlog 3
| Sprint 3 – Work Items / Tasks (Web Service SEMS) | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **User Story ID** | **Task ID** | **Title** | **Description** | **Estimation** | **Assigned To** | **Status** |
| **EP01 – Autenticación y Perfil de Usuario** | | | | | | |
| US01 | UT01 | Registro de usuario | Crear endpoint POST /api/v1/auth/register con validaciones de correo y contraseña. | 4h | Mateo Loechle | Done |
| | UT02 | Validar correo duplicado en registro | Implementar verificación de que el correo no esté registrado previamente. | 2h | Yeira Huamán | Done |
| US02 | UT03 | Inicio de sesión | Crear endpoint POST /api/v1/auth/login con autenticación JWT. | 3h | Iker Barturen | Done |
| | UT04 | Manejo de errores en autenticación | Retornar mensajes de error para credenciales inválidas o usuario inexistente. | 2h | Yeira Huamán | Done |
| US03 | UT05 | Gestión de perfil | Crear endpoints GET/PUT /api/profile/{userId} para obtener y actualizar perfil. | 3h | Andrés Torres | Done |
| | UT06 | Implementar subida de foto de perfil | Crear endpoint POST /api/profile/{userId}/photo para actualizar foto. | 2h | Alexis Encalada | Done |
| US04 | UT07 | Recuperación de contraseña | Crear endpoint POST /api/v1/settings/{userId}/reset para iniciar reset. | 3h | Yeira Huamán | Done |
| | UT08 | Implementar actualización de contraseña | Crear endpoint POST /api/v1/settings/{userId}/password para cambiar contraseña. | 2h | Mateo Loechle | Done |
| US05 | UT09 | Validación de sesión | Crear endpoint GET /api/v1/auth/validate para verificar sesión activa. | 3h | Iker Barturen | Done |
| **EP02 – Conexión y Monitoreo de Dispositivos** | | | | | | |
| US06 | UT10 | Gestión de dispositivos | Crear endpoints GET/POST /api/v1/devices y GET/PUT/DELETE /api/v1/devices/{deviceId}. | 4h | Alexis Encalada | Done |
| | UT11 | Validar compatibilidad de dispositivos | Implementar lógica para verificar si un dispositivo es compatible. | 2h | Mateo Loechle | Done |
| US07 | UT12 | Toggle de dispositivos | Crear endpoint POST /api/v1/devices/{deviceId}/toggle para encender/apagar. | 3h | Yeira Huamán | Done |
| | UT13 | Implementar preferencias de dispositivos | Crear endpoints GET/PUT /api/v1/preferences/devices. | 2h | Alexis Encalada | Done |
| US08 | UT14 | Monitoreo de dispositivos activos | Crear endpoint GET /api/v1/devices/active para listar dispositivos conectados. | 4h | Iker Barturen | Done |
| | UT15 | Manejo de desconexiones | Implementar notificaciones cuando un dispositivo se desconecta. | 2h | Yeira Huamán | Done |
| **EP03 – Alertas y Recordatorios de Consumo** | | | | | | |
| US09 | UT16 | Gestión de alertas | Crear endpoints GET/POST /api/v1/alerts y PUT /api/v1/alerts/{alertId}/read. | 3h | Mateo Loechle | Done |
| | UT17 | Implementar conteo de alertas no leídas | Crear endpoint GET /api/v1/alerts/count/unread. | 2h | Andrés Torres | Done |
| US10 | UT18 | Gestión de notificaciones | Crear endpoints GET/POST /api/v1/notifications y PUT /api/v1/notifications/{notificationId}/read. | 3h | Alexis Encalada | Done |
| | UT19 | Implementar conteo de notificaciones no leídas | Crear endpoint GET /api/v1/notifications/count/unread. | 2h | Yeira Huamán | Done |
| US11 | UT20 | Configuración de umbrales | Permitir definir límites de consumo y restablecer a predeterminados. | 4h | Iker Barturen | Done |
| **EP04 – Reportes y Facturación** | | | | | | |
| US12 | UT21 | Generación de reportes semanales | Crear endpoints POST /api/v1/reports/weeklyConsumption/generate-sample y GET /api/v1/reports/weeklyConsumption. | 4h | Mateo Loechle | Done |
| US13 | UT22 | Consulta de consumo diario | Crear endpoints GET /api/v1/consumption/daily y GET /api/v1/consumption/daily/{date}. | 3h | Yeira Huamán | Done |
| US14 | UT23 | Consulta de consumo mensual | Crear endpoint GET /api/v1/consumption/monthly. | 3h | Andrés Torres | Done |
| US15 | UT24 | Consulta de consumo por categorías | Crear endpoint GET /api/v1/consumption/categories. | 3h | Alexis Encalada | Done |
| **EP05 – Metas y Ahorro Energético** | | | | | | |
| US16 | UT25 | Estadísticas del dashboard | Crear endpoints GET/PUT /api/v1/dashboard/stats. | 3h | Yeira Huamán | Done |
| US17 | UT26 | Inicialización de datos | Crear endpoint POST /api/v1/data/initialize. | 4h | Iker Barturen | Done |
| US18 | UT27 | Resumen de datos | Crear endpoint GET /api/v1/data/summary. | 3h | Mateo Loechle | Done |
| US19 | UT28 | Configuración de metas | Permitir configurar metas mensuales y seguimiento. | 3h | Alexis Encalada | Done |
| US20 | UT29 | Comparación de consumo | Mostrar comparación con otros usuarios y ranking. | 3h | Andrés Torres | Done |
| **EP07 – Gestión de Categorías de Dispositivos** | | | | | | |
| US24 | UT33 | Consulta por categoría | Crear endpoint GET /api/v1/devices/category/{category}. | 3h | Alexis Encalada | Done |
| US25 | UT34 | Consumo por categoría | Mostrar consumo agrupado por categoría. | 4h | Yeira Huamán | Done |
| US26 | UT35 | Identificación de dispositivos de alto consumo | Implementar lógica para alertar sobre dispositivos con mayor gasto. | 3h | Andrés Torres | Done |



#### 5.2.3.4. Development Evidence for Sprint Review

En esta secciÃ³n se demuestran los commits relacionados con los principales avances en la implementaciÃ³n.
Estos commits provienen del repositorio del proyecto backend de la organizaciÃ³n de GitHub.

Enlace al repositorio del proyecto backend: https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS

| Repository                                         | Branch                           | Commit Id                                 | Commit Message                                                           | Commit Message Body | Commited on (Date) |
|----------------------------------------------------|----------------------------------|-------------------------------------------|--------------------------------------------------------------------------|---------------------|--------------------|
| Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS    | feature/add-project              | 65d26a57c1fb30780c9db3a55dc3f302eab64082  | Feature/add project                                                      |                     | 29/10/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS    | feature/config-backend           | 0e50511fdc7a99b4f60ac9e78fc236332d488708  | feat: add first version                                                  |                     | 03/11/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS    | feature/profile-init-config      | e9e4e3353c73a0b2301b319c35404c8bc20fade7  | Feat/profile init config                                                 |                     | 06/11/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS    | feature/connection               | 5cc751029426a07941fba60d2735b51363bb834c  | feat(auth): Connect Frontend Authentication With Backend API.            |                     | 07/11/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS    | feature/settings                 | b68c96252d5583f0ff3d7826c89b08ca204f441b  | feat(settings): Implemente User Settings Management With CRUD Operations |                     | 09/11/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS    | feature/add-new-endpoints        | 702447a7b428d61c3cd76a2e0373102990b53515  | Feature/add new endpoints                                                |                     | 13/11/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS    | feature/reports                  | 705573e1ea7091ee0c8a40e87b88b7c95bbd4371  | feat: create reports.                                                    |                     | 13/11/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS    | feature/reports-update           | fb5da2038951b1b1a9068f1012d29064edeec621  | feat: update reports.                                                    |                     | 13/11/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS    | feature/authentication           | b32f475b1eac274a81a18850c109e171f03685ad  | feat: add login credentials.                                             |                     | 13/11/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS    | feature/reports-parameters       | 29a7d839e6481ba5598c7aa17c21b08a4d1887b5  | Feature/reports parameters                                               |                     | 13/11/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS    | feature/repositoryfix            | 4b8073537ccdbc5b6fbd206651b2caa1483fcc0e  | Feature/repositoryfix merged finally.                                    |                     | 14/11/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS    | feature/add-deploy-config        | 333098292deac7dfb546ce1c307ed9b29fc25068  | feat: Feature/add deploy config                                          |                     | 15/11/2025         |
| Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS    | feature/add-deploy-config        | e8ac569ad61685f27637b215afcbd2c70cb24e4f  | feat: remove .env file copy instruction from Dockerfile                  |                     | 15/11/2025         |

#### 5.2.3.5. Execution Evidence for Sprint Review

Durante el desarrollo del sprint se lograron completar todos los puntos para la implementaciÃ³n de las funcionalidades esenciales del backend para el sistema de gestiÃ³n Energix, estableciendo una base sÃ³lida para la administraciÃ³n de energÃ­a en los hogares. Las principales caracterÃ­sticas desarrolladas fueron:

1. API de autenticaciÃ³n completa con endpoints para registro, login y validaciÃ³n de sesiÃ³n.

2. GestiÃ³n de perfiles a travÃ©s de API, permitiendo obtener, actualizar y subir foto de perfil.

3. GeneraciÃ³n y consulta de reportes vÃ­a API, con soporte para reportes semanales y consultas de consumo diario, mensual y por categorÃ­as.

4. CRUD de dispositivos, incluyendo monitoreo en tiempo real, toggle, preferencias y gestiÃ³n por categorÃ­as.

5. ValidaciÃ³n de sesiones y logout seguro, con manejo de errores en autenticaciÃ³n.

6. Arquitectura robusta del backend con integraciÃ³n a base de datos, manejo de alertas y notificaciones, y despliegue en Render con documentaciÃ³n Swagger.

**Capturas de pantalla de la documentacion en Swagger**

**Deployment en Render del Backend**

![Deploy-API.png](assets/Deploy-API.png)

**SEMS API**

![alt text](assets/SEMS-API.png)

#### 5.2.3.6. Services Documentation Evidence for Sprint Review

IntroducciÃ³n

Durante el sprint 3, hemos implementado el despliegue del backend del sistema de Energix en Render, creando una API robusta y documentada con Swagger que soporta todas las funcionalidades esenciales para la gestiÃ³n de energÃ­a en los hogares.

**ImplementaciÃ³n de API centralizada en Render**

Decidimos utilizar Render para el despliegue del backend, asegurando una infraestructura centralizada y escalable. Esta decisiÃ³n nos permitiÃ³ tener un mayor control sobre la API y facilitar la integraciÃ³n con el frontend.

Por motivos de seguridad, implementamos un proxy utilizando Cloudflare Tunnel para ocultar la direcciÃ³n IP real del servidor, ya que exponer pÃºblicamente la URL directa en GitHub representa un riesgo de seguridad. Esta medida de protecciÃ³n es fundamental para prevenir ataques directos al servidor.

La URL base para todos los recursos de nuestra API es:

https://theft-muscles-inner-protection.trycloudflare.com

La documentaciÃ³n interactiva de la API estÃ¡ disponible en Swagger UI en:

https://theft-muscles-inner-protection.trycloudflare.com/swagger-ui/index.html

**ConfiguraciÃ³n del servidor en Render**

El proceso de implementaciÃ³n en Render involucrÃ³ varias etapas para asegurar un despliegue exitoso. Comenzamos creando una nueva cuenta y proyecto en la plataforma, configurÃ¡ndolo especÃ­ficamente para trabajar con Java/Spring Boot como entorno de ejecuciÃ³n.

Conectamos nuestro repositorio de GitHub para habilitar el despliegue automÃ¡tico, lo que nos permite mantener sincronizado el entorno de producciÃ³n con la rama principal del proyecto. Esto ha resultado en un flujo de trabajo mÃ¡s eficiente, donde cada merge a la rama principal actualiza automÃ¡ticamente nuestra API.

| MÃ©todo HTTP | Endpoint                          | DescripciÃ³n                                        | Ejemplo de uso                             |
|-------------|-----------------------------------|----------------------------------------------------|--------------------------------------------|
| POST        | /api/v1/auth/register             | Registra un nuevo usuario                          | Crear cuenta de propietario o estudiante   |
| POST        | /api/v1/auth/login                | Autentica un usuario                               | Iniciar sesiÃ³n                             |
| GET         | /api/v1/auth/validate             | Valida la sesiÃ³n activa                            | Verificar token JWT                        |
| GET         | /api/profile/{userId}             | Obtiene el perfil de un usuario                    | Mostrar datos del perfil                   |
| PUT         | /api/profile/{userId}             | Actualiza el perfil de un usuario                  | Modificar informaciÃ³n personal             |
| GET         | /api/v1/devices                   | Obtiene lista de dispositivos                      | Listar dispositivos registrados            |
| POST        | /api/v1/devices                   | Crea un nuevo dispositivo                          | Agregar dispositivo                        |
| GET         | /api/v1/devices/{deviceId}        | Obtiene un dispositivo especÃ­fico                  | Ver detalles de dispositivo                |
| PUT         | /api/v1/devices/{deviceId}        | Actualiza un dispositivo                           | Editar configuraciÃ³n                       |
| DELETE      | /api/v1/devices/{deviceId}        | Elimina un dispositivo                             | Remover dispositivo                        |
| POST        | /api/v1/devices/{deviceId}/toggle | Cambia el estado de un dispositivo                 | Encender/apagar dispositivo                |
| GET         | /api/v1/alerts                    | Obtiene lista de alertas                           | Mostrar alertas activas                    |
| POST        | /api/v1/alerts                    | Crea una nueva alerta                              | Generar alerta de consumo                  |
| GET         | /api/v1/notifications             | Obtiene notificaciones                             | Listar notificaciones del usuario          |
| GET         | /api/v1/consumption/daily         | Obtiene consumo diario                             | Mostrar grÃ¡fico de consumo diario          |
| GET         | /api/v1/consumption/monthly       | Obtiene consumo mensual                            | Ver resumen mensual                        |
| GET         | /api/v1/reports/weeklyConsumption | Obtiene reporte semanal de consumo                 | Generar y descargar reporte semanal        |
| GET         | /api/v1/dashboard/stats           | Obtiene estadÃ­sticas del dashboard                 | Mostrar mÃ©tricas generales                 |


#### 5.2.3.7. Software Deployment Evidence for Sprint Review

Durante este Sprint, se completÃ³ el desarrollo del backend del Web Service y se realizÃ³ su despliegue utilizando Render como plataforma de publicaciÃ³n. El objetivo fue contar con una primera versiÃ³n accesible en lÃ­nea de la API backend para revisiÃ³n y retroalimentaciÃ³n.

Actividades realizadas: Se creÃ³ el repositorio en GitHub: https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS

Se subiÃ³ el cÃ³digo fuente del backend, incluyendo los archivos Java, Spring Boot, configuraciÃ³n de base de datos y dependencias necesarias.

Se configurÃ³ en Render para el despliegue del backend API.

Se verificÃ³ la correcta publicaciÃ³n del backend en la siguiente URL: https://backend-sems-40cb.onrender.com/

#### 5.2.3.8. Team Collaboration Insights during Sprint

En esta secciÃ³n se evidencia la colaboraciÃ³n de cada integrante en el repositorio del Backend de la AplicaciÃ³n.

Repositorio del Backend de la AplicaciÃ³n: https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS

| **Integrante**                       | **Actividad**                                                                                            |  
|--------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Huaman Olivos, Yeira Shari**       | ImplementaciÃ³n de secciones del **Backend de la AplicaciÃ³n** y contribuciones a los **chapter 5.md**     |
| **Loechle Arias, Mateo Ãtalo**       | ImplementaciÃ³n de secciones del **Backend de la AplicaciÃ³n** y contribuciones a los **chapter 5.md**     |
| **Barturen Panez, Iker Gabriel**     | ImplementaciÃ³n de secciones del **Backend de la AplicaciÃ³n** y contribuciones a los **chapter 5.md**     |
| **Encalada Salazar, Alexis**         | ImplementaciÃ³n de secciones del **Backend de la AplicaciÃ³n** y contribuciones a los **chapter 5.md**     |
| **Torres Lavandera, AndrÃ©s Rodrigo** | ImplementaciÃ³n de secciones del **Backend de la AplicaciÃ³n** y contribuciones a los **chapter 5.md**     |
| **Ynga Amado, Jafeth Worren**        | ImplementaciÃ³n de secciones del **Backend de la AplicaciÃ³n** y contribuciones a los **chapter 5.md**     |

![CommitsBK.png](assets/CommitsBK.png)

![NetBK1.png](assets/NetBK1.png)

![NetBK2.png](assets/NetBK2.png)

### 5.2.4. Sprint 4

#### 5.2.4.1. Sprint Planning 4

Durante el Sprint 4 se implementÃ³ la integraciÃ³n completa entre el frontend y el backend de la plataforma SEMS, enfocÃ¡ndose en la comunicaciÃ³n efectiva entre ambas capas para asegurar una experiencia de usuario fluida. El trabajo incluyÃ³ la conexiÃ³n de APIs, sincronizaciÃ³n de datos, manejo de estados y la validaciÃ³n de la funcionalidad, consolidando una versiÃ³n integrada y funcional del sistema.

| Sprint 4 | Sprint 4 |
| :--- | :--- |
| **Sprint Planning Background** | |
| **Date** | 2025-11-29 |
| **Time** | 2:30 PM |
| **Location** | Via Discord |
| **Prepared By** | Iker Gabriel Barturen Panez |
| **Attendees (to a planning meeting)** | Alexis Encalada Salazar, Yeira Shari Huaman Olivos, Andrés Rodrigo Torres Lavandera, Iker Gabriel Barturen Panez, Mateo Italo Loechle Arias, Jafeth Worren Ynga Amado |
| **Sprint Goal & User Stories** | |
| **Sprint 4 Goal** | Implementar la integración completa entre frontend y backend de la aplicación web Energix, asegurando la comunicación efectiva de APIs, sincronización de datos y validación para una experiencia de usuario fluida. |
| **Sprint 4 Velocity** | 10 |
| **Sum of Story Points** | 89 |

#### 5.2.4.2. Aspect Leaders and Collaborators

Con la finalidad de mejorar la colaboraciÃ³n en equipo a cada integrante se asignÃ³ un rol de lÃ­der por cada aspecto. Los aspectos estÃ¡n relacionados con los entregables.

| Team member (LastName, First Name) | GitHub UserName       | Aspect 1: Connection of Devices & Authentication | Aspect 2: Profile Connection   | Aspect 3: Connection for Reports   | Aspect 4: Backend for Notifications | Aspect 5: Connection for Settings  | Aspect 6:Connection for Dashboard |
|------------------------------------|-----------------------|--------------------------------------------------|--------------------------------|------------------------------------|-------------------------------------|------------------------------------|-----------------------------------|
| Alexis Encalada                    | Alexiz248             | C                                                | C                              | C                                  | C                                   | L                                  | C                                 |
| Yeira Sharia                       | YeiShari              | C                                                | L                              | C                                  | C                                   | C                                  | C                                 |
| AndrÃ©s Torres                      | AndresTorres202312557 | C                                                | C                              | L                                  | C                                   | C                                  | C                                 |
| Iker Barturen                      | krxxg04               | L                                                | C                              | C                                  | C                                   | C                                  | C                                 |
| Mateo Loechle                      | LowMathzzz            | C                                                | C                              | C                                  | L                                   | C                                  | C                                 |
| Jafeth Ynga                        | Jafeth-MV             | C                                                | C                              | C                                  | L                                   | C                                  | L                                 |

#### 5.2.4.3. Sprint Backlog 4

| Sprint 4 – Work Items / Tasks (Web Service SEMS) | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **User Story ID** | **Task ID** | **Title** | **Description** | **Estimation** | **Assigned To** | **Status** |
| **EP01 – Autenticación y Perfil de Usuario** | | | | | | |
| US01 | UT01 | Registro de usuario | Implementar componente de registro en frontend que conecte con endpoint POST /api/v1/auth/register con validaciones de correo y contraseña. | 4h | Mateo Loechle | Done |
| | UT02 | Validar correo duplicado en registro | Implementar verificación en frontend de que el correo no esté registrado previamente conectando con el backend. | 2h | Jafeth Ynga | Done |
| US02 | UT03 | Inicio de sesión | Implementar formulario de login en frontend que conecte con endpoint POST /api/v1/auth/login con autenticación JWT. | 3h | Iker Barturen | Done |
| | UT04 | Manejo de errores en autenticación | Implementar manejo de errores en frontend para credenciales inválidas o usuario inexistente conectando con el backend. | 2h | Jafeth Ynga | Done |
| US03 | UT05 | Gestión de perfil | Implementar vista de perfil en frontend que conecte con endpoints GET/PUT /api/profile/{userId} para obtener y actualizar perfil. | 3h | Andrés Torres | Done |
| | UT06 | Implementar subida de foto de perfil | Implementar funcionalidad de subida de foto en frontend que conecte con endpoint POST /api/profile/{userId}/photo. | 2h | Alexis Encalada | Done |
| US04 | UT07 | Recuperación de contraseña | Implementar formulario de recuperación en frontend que conecte con endpoint POST /api/v1/settings/{userId}/reset. | 3h | Yeira Huamán | Done |
| | UT08 | Implementar actualización de contraseña | Implementar funcionalidad de cambio de contraseña en frontend que conecte con endpoint POST /api/v1/settings/{userId}/password. | 2h | Mateo Loechle | Done |
| US05 | UT09 | Validación de sesión | Implementar validación de sesión activa en frontend conectando con endpoint GET /api/v1/auth/validate. | 3h | Iker Barturen | Done |
| **EP02 – Conexión y Monitoreo de Dispositivos** | | | | | | |
| US06 | UT10 | Gestión de dispositivos | Implementar interfaz de gestión de dispositivos en frontend que conecte con endpoints GET/POST /api/v1/devices y GET/PUT/DELETE /api/v1/devices/{deviceId}. | 4h | Alexis Encalada | Done |
| | UT11 | Validar compatibilidad de dispositivos | Implementar validación de compatibilidad en frontend conectando con lógica del backend. | 2h | Mateo Loechle | Done |
| US07 | UT12 | Toggle de dispositivos | Implementar control de encendido/apagado en frontend que conecte con endpoint POST /api/v1/devices/{deviceId}/toggle. | 3h | Yeira Huamán | Done |
| | UT13 | Implementar preferencias de dispositivos | Implementar configuración de preferencias en frontend conectando con endpoints GET/PUT /api/v1/preferences/devices. | 2h | Iker Barturen | Done |
| US08 | UT14 | Monitoreo de dispositivos activos | Implementar vista de monitoreo en frontend que conecte con endpoint GET /api/v1/devices/active. | 4h | Iker Barturen | Done |
| | UT15 | Manejo de desconexiones | Implementar notificaciones de desconexión en frontend conectando con el backend. | 2h | Yeira Huamán | Done |
| **EP03 – Alertas y Recordatorios de Consumo** | | | | | | |
| US09 | UT16 | Gestión de alertas | Implementar gestión de alertas en frontend que conecte con endpoints GET/POST /api/v1/alerts y PUT /api/v1/alerts/{alertId}/read. | 3h | Mateo Loechle | Done |
| | UT17 | Implementar conteo de alertas no leídas | Implementar contador de alertas no leídas en frontend conectando con endpoint GET /api/v1/alerts/count/unread. | 2h | Jafeth Ynga | Done |
| US10 | UT18 | Gestión de notificaciones | Implementar gestión de notificaciones en frontend que conecte con endpoints GET/POST /api/v1/notifications y PUT /api/v1/notifications/{notificationId}/read. | 3h | Alexis Encalada | Done |
| | UT19 | Implementar conteo de notificaciones no leídas | Implementar contador de notificaciones no leídas en frontend conectando con endpoint GET /api/v1/notifications/count/unread. | 2h | Mateo Loechle | Done |
| US11 | UT20 | Configuración de umbrales | Implementar configuración de umbrales en frontend que permita definir límites conectando con el backend. | 4h | Iker Barturen | Done |
| **EP04 – Reportes y Facturación** | | | | | | |
| US12 | UT21 | Generación de reportes semanales | Implementar generación de reportes semanales en frontend que conecte con endpoints POST /api/v1/reports/weeklyConsumption/generate-sample y GET /api/v1/reports/weeklyConsumption. | 4h | Mateo Loechle | Done |
| US13 | UT22 | Consulta de consumo diario | Implementar vista de consumo diario en frontend que conecte con endpoints GET /api/v1/consumption/daily y GET /api/v1/consumption/daily/{date}. | 3h | Jafeth Ynga | Done |
| US14 | UT23 | Consulta de consumo mensual | Implementar vista de consumo mensual en frontend que conecte con endpoint GET /api/v1/consumption/monthly. | 3h | Andrés Torres | Done |
| US15 | UT24 | Consulta de consumo por categorías | Implementar vista de consumo por categorías en frontend que conecte con endpoint GET /api/v1/consumption/categories. | 3h | Alexis Encalada | Done |
| **EP05 – Metas y Ahorro Energético** | | | | | | |
| US16 | UT25 | Estadísticas del dashboard | Implementar estadísticas del dashboard en frontend que conecte con endpoints GET/PUT /api/v1/dashboard/stats. | 3h | Yeira Huamán | Done |
| US17 | UT26 | Inicialización de datos | Implementar inicialización de datos en frontend que conecte con endpoint POST /api/v1/data/initialize. | 4h | Iker Barturen | Done |
| US18 | UT27 | Resumen de datos | Implementar resumen de datos en frontend que conecte con endpoint GET /api/v1/data/summary. | 3h | Jafeth Ynga | Done |
| US19 | UT28 | Configuración de metas | Implementar configuración de metas en frontend que permita configurar metas mensuales conectando con el backend. | 3h | Alexis Encalada | Done |
| US20 | UT29 | Comparación de consumo | Implementar comparación de consumo en frontend que muestre comparación con otros usuarios conectando con el backend. | 3h | Andrés Torres | Done |
| **EP07 – Gestión de Categorías de Dispositivos** | | | | | | |
| US24 | UT33 | Consulta por categoría | Implementar consulta por categoría en frontend que conecte con endpoint GET /api/v1/devices/category/{category}. | 3h | Alexis Encalada | Done |
| US25 | UT34 | Consumo por categoría | Implementar vista de consumo por categoría en frontend que muestre consumo agrupado conectando con el backend. | 4h | Jafeth Ynga | Done |
| US26 | UT35 | Identificación de dispositivos de alto consumo | Implementar identificación de dispositivos de alto consumo en frontend conectando con lógica del backend. | 3h | Andrés Torres | Done |

#### 5.2.4.4. Development Evidence for Sprint Review

En esta secciÃ³n se demuestran los commits relacionados con los principales avances en la implementaciÃ³n.
Estos commits provienen del repositorio del proyecto backend de la organizaciÃ³n de GitHub.

Enlace al repositorio del proyecto backend: https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS

| Repository | Branch | Commit Id | Commit Message | Committed on (Date) |
|-----------|--------|-----------|----------------|---------------------|
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | develop | fad3594 | feat: update SnakeCase. | Nov 13, 2025        |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | develop | 99a6886 | feat: add post by swagger. | Nov 13, 2025        |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | develop | 705573e | Merge pull request #7 from Upc-pre-1ASI0729-2520-7401-Energix/feature/reports | Nov 13, 2025        |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | develop | 546ddae | feat: add repository and DTO fixes | Nov 14, 2025        |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | develop | f481f5c | feat: add Javadoc documentation for DashboardStatsRepository and fixed identation | Nov 14, 2025        |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | develop | d28ac10 | feat: add Javadoc documentation for DailyConsumptionRepository and fixed maven dependencie | Nov 14, 2025        |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | develop | 4b80735 | Merge pull request #11 from Upc-pre-1ASI0729-2520-7401-Energix/feature/repositoryfix | Nov 14, 2025        |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | develop | 53399ed | feat: update Java version, add Dockerfile, and refactor UserSettings entity to use OneToMany relationships for report frequencies and formats | Nov 15, 2025        |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | develop | 3330982 | Merge pull request #12 from Upc-pre-1ASI0729-2520-7401-Energix/feature/add-deploy-config | Nov 15, 2025        |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | fix/profile-management | de8265d | feat: Refactor authentication and profile management services. | Nov 24, 2025        |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | develop | cbc2e49 | Merge pull request #14 from Upc-pre-1ASI0729-2520-7401-Energix/feature/update-Authentication | Nov 24, 2025        |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | feat/settings | 8d7e29f | feat: remove SettingsController and related classes. | Nov 30, 2025        |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | develop | 7bd6ab2 | feat: Remove unused service and repository files. | Nov 30, 2025        |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | feat/notification | ef1df3d | feat: Implement notification system with command and query services, event handling, and REST API endpoints. | Nov 30, 2025        |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | feat/notification | 5ce91b3 | feat: Refactor device and notification handling, update command structures, and enhance user profile integration. | Nov 30, 2025        |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | feat/dashboard | 6aa1db3 | feat(alert): add AlertResource record for alert data structure. | Dec 1, 2025         |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | feat/dashboard | eea2882 | feat(dashboard): add CategoryConsumptionResource record for category consumption data structure. | Dec 1, 2025         |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | feat/dashboard | 8ad47c7 | feat: add ConsumptionByHourResource record for hourly consumption data structure. | Dec 1, 2025         |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | feat/dashboard | c204343 | feat(dashboard): add DashboardQueryService interface for querying dashboard data by user ID. | Dec 1, 2025         |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | feat/authentication | 00ffb7c | feat(authentication): enhance sign-up process with error logging and role handling improvements. | Dec 2, 2025         |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | fix/profile | d29ccdb | feat(profile): enhance Profile aggregate with profile photo handling and update related resources. | Dec 2, 2025         |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | feature/new-api | 358bcc4 | Merge pull request #15 from Upc-pre-1ASI0729-2520-7401-Energix/feature/new-API | Dec 2, 2025         |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | feat/dashboard | 56cf65a | feat(dashboard): enhance dashboard query service with detailed consumption calculations and alerts. | Dec 3, 2025         |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | feat/docker | 0bf1e38 | feat(docker): update base images to Maven 3.9.9 and Oracle JDK 25 for improved performance. | Dec 3, 2025         |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | develop | 7ba01a7 | Merge pull request #16 from Upc-pre-1ASI0729-2520-7401-Energix/feature/fix-dashboard | Dec 3, 2025         |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | feat/user | d53568c | feat(user): implement email update functionality and secure user retrieval endpoints. | Dec 3, 2025         |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | develop | 32f5656 | feat(preferences): refactor preferences handling to support global user preferences and enhance logging. | Dec 3, 2025         |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | develop | 31120c0 | feat(profile): synchronize email updates with users table and enhance logging. | Dec 3, 2025         |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS | develop | 57fa8d2 | Merge pull request #17 from Upc-pre-1ASI0729-2520-7401-Energix/feature/fix-profiles | Dec 3, 2025         |

Enlace al repositorio del proyecto frontend: https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Frontend-SEMS

| Repository | Branch | Commit Id | Commit Message | Commited on (Date) |
|-----------|--------|-----------|----------------|---------------------|
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Frontend-SEMS | develop | c83edd3 | feat: Update authentication to use email and improve token management. | Nov 15, 2025 |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Frontend-SEMS | fix/profile | ac1dd5b | feat(header.ts): optimize profile fetching with distinctUntilChanged operator | Nov 15, 2025 |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Frontend-SEMS | fix/profile | e405d2e | feat(profile): enhance profile update logic and user ID retrieval from token | Nov 15, 2025 |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Frontend-SEMS | fix/profile | 618f24e | feat: enhance profile management with additional fields and loading states. | Nov 28, 2025 |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Frontend-SEMS | feature/release-1.0 | 04144f5 | feat: add brand and model fields to device management and update related components. | Nov 29, 2025 |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Frontend-SEMS | feature/release-1.0 | 29efdb0 | feat: update category-chart.ts | Nov 30, 2025 |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Frontend-SEMS | feature/release-1.0 | 5164cb | feat: update device-chart. | Nov 30, 2025 |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Frontend-SEMS | feature/release-1.0 | 2e6ae6f | feat: update notifications. | Nov 30, 2025 |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Frontend-SEMS | feature/release-1.0 | 4f82b96 | feat: enhance device management by updating form fields and improving data handling. | Dec 03, 2025 |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Frontend-SEMS | feature/release-1.0 | 20022d2 | feat(settings): Add Support Modals for FAQs and help. | Dec 03, 2025 |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Frontend-SEMS | feature/release-1.0 | dbf3277 | Merge branch 'feature/release-1.0' of https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Frontend-SEMS into feature/release-1.0 | Dec 03, 2025 |
| https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Frontend-SEMS | feature/release-1.0 | a66f6c5 | feat(monthly-chart): enhance monthly chart with Chart.js integration and static data display. | Dec 03, 2025 |




#### 5.2.4.5. Execution Evidence for Sprint Review

Durante el desarrollo del sprint 4 se lograron completar todos los puntos para la integraciÃ³n completa entre frontend y backend de la aplicaciÃ³n SEMS, estableciendo una conexiÃ³n fluida entre las capas del sistema para la gestiÃ³n de energÃ­a en los hogares. Las principales caracterÃ­sticas integradas fueron:

1. IntegraciÃ³n de autenticaciÃ³n completa conectando frontend con endpoints de registro, login y validaciÃ³n de sesiÃ³n.

2. GestiÃ³n de perfiles integrada, permitiendo obtener, actualizar y subir foto de perfil desde el frontend.

3. GeneraciÃ³n y consulta de reportes integrada, con soporte para reportes semanales y consultas de consumo diario, mensual y por categorÃ­as.

4. CRUD de dispositivos integrado, incluyendo monitoreo en tiempo real, toggle, preferencias y gestiÃ³n por categorÃ­as desde la interfaz.

5. ValidaciÃ³n de sesiones y manejo de errores en autenticaciÃ³n integrada.

6. Arquitectura completa con frontend, backend, base de datos y despliegues en plataformas en lÃ­nea para una experiencia de usuario completa.

**Capturas de pantalla de los diferentes despliegues**

**Deployment de Landing Page en Netlify**

![LandingPage-Netlify.png](assets/LandingPage.png)

**Deployment de Frontend en Vercel**

![Frontend-Vercel.png](assets/Frontend-Login.png)

![vercel.png](assets/vercel.png)

**Deployment en Render del Backend**

![alt text](assets/Deploy-New-API.png)

![alt text](assets/Deploy-Proxy.jpeg)

**SEMS API**

![alt text](assets/SEMS-API-Documentation.png)

**Database hosted on Aiven**

![db-Aiven.png](assets/db-Aiven.png)

#### 5.2.4.6. Services Documentation Evidence for Sprint Review

**IntroducciÃ³n**

Durante el sprint 4, hemos implementado la integraciÃ³n completa del sistema de Energix, desplegando landing page en Netlify, frontend en Vercel, backend en Render y la base de datos en Aiven, creando una aplicaciÃ³n completa y funcional para la gestiÃ³n de energÃ­a en los hogares.

**ImplementaciÃ³n de landing page en Netlify**

Utilizamos Netlify para el despliegue de la landing page, asegurando una presentaciÃ³n atractiva y accesible del proyecto.

La URL de la landing page es:

https://energixlp.netlify.app

**ImplementaciÃ³n de frontend en Vercel**

Desplegamos el frontend en Vercel, facilitando la interacciÃ³n del usuario con la aplicaciÃ³n web integrada.

La URL del frontend es:

https://frontend-sems.vercel.app

**ImplementaciÃ³n de API centralizada en Render**

Decidimos utilizar Render para el despliegue del backend, asegurando una infraestructura centralizada y escalable. Esta decisiÃ³n nos permitiÃ³ tener un mayor control sobre la API y facilitar la integraciÃ³n con el frontend.

Por motivos de seguridad y para proteger la direcciÃ³n IP pÃºblica del servidor, hemos implementado un proxy utilizando Cloudflare Tunnel que oculta la direcciÃ³n real del servidor Render. Esto es especialmente importante cuando se publican URLs en repositorios pÃºblicos de GitHub, ya que exponer directamente las IPs representar un riesgo de seguridad.

La URL base para todos los recursos de nuestra API a travÃ©s del proxy seguro es:

https://theft-muscles-inner-protection.trycloudflare.com

La documentaciÃ³n interactiva de la API estÃ¡ disponible en Swagger UI en:

https://theft-muscles-inner-protection.trycloudflare.com/swagger-ui/index.html

**ConfiguraciÃ³n de base de datos en Aiven**

La base de datos se aloja en Aiven, proporcionando un servicio de base de datos en la nube confiable y escalable para almacenar y gestionar los datos del sistema.

| **ParÃ¡metro** | **Valor** |
|---------------|-----------|
| Service URI   | mysql://avnadmin:[REDACTED]@sems-semsv01.i.aivencloud.com:11867/defaultdb?ssl-mode=REQUIRED |
| Database name | defaultdb |
| Host          | sems-semsv01.i.aivencloud.com |
| Port          | 11867 |
| User          | avnadmin |
| Password      | [REDACTED] |
| SSL mode      | REQUIRED |

**ConfiguraciÃ³n del servidor en Render**

El proceso de implementaciÃ³n en Render involucrÃ³ varias etapas para asegurar un despliegue exitoso. Comenzamos creando una nueva cuenta y proyecto en la plataforma, configurÃ¡ndolo especÃ­ficamente para trabajar con Java/Spring Boot como entorno de ejecuciÃ³n.

Conectamos nuestro repositorio de GitHub para habilitar el despliegue automÃ¡tico, lo que nos permite mantener sincronizado el entorno de producciÃ³n con la rama principal del proyecto. Esto ha resultado en un flujo de trabajo mÃ¡s eficiente, donde cada merge a la rama principal actualiza automÃ¡ticamente nuestra API.

| MÃ©todo HTTP | Endpoint                                      | DescripciÃ³n                                        | Ejemplo de uso                             |
|-------------|-----------------------------------------------|----------------------------------------------------|--------------------------------------------|
| POST        | /api/v1/authentication/sign-up                | Registra un nuevo usuario                          | Crear cuenta de propietario o estudiante   |
| POST        | /api/v1/authentication/sign-in                | Autentica un usuario                               | Iniciar sesiÃ³n                             |
| GET         | /api/v1/profiles/{profileId}                  | Obtiene el perfil por ID                           | Mostrar datos del perfil especÃ­fico        |
| PUT         | /api/v1/profiles/{profileId}                  | Actualiza el perfil por ID                         | Modificar informaciÃ³n personal             |
| GET         | /api/v1/profiles/me                           | Obtiene el perfil del usuario actual               | Mostrar datos del perfil propio            |
| PUT         | /api/v1/profiles/me                           | Actualiza el perfil del usuario actual             | Editar informaciÃ³n personal propia         |
| GET         | /api/v1/devices                               | Obtiene lista de dispositivos                      | Listar todos los dispositivos              |
| POST        | /api/v1/devices                               | Crea un nuevo dispositivo                          | Agregar dispositivo                        |
| GET         | /api/v1/devices/{deviceId}                    | Obtiene un dispositivo especÃ­fico                  | Ver detalles de dispositivo                |
| DELETE      | /api/v1/devices/{deviceId}                    | Elimina un dispositivo                             | Remover dispositivo                        |
| GET         | /api/v1/devices/{deviceId}/consumption        | Obtiene el consumo de un dispositivo               | Ver consumo especÃ­fico del dispositivo     |
| GET         | /api/v1/devices/users/{userId}                | Obtiene dispositivos por ID de usuario             | Listar dispositivos de un usuario          |
| GET         | /api/v1/notifications                         | Obtiene todas las notificaciones                   | Listar todas las notificaciones            |
| POST        | /api/v1/notifications                         | Crea una nueva notificaciÃ³n                        | Generar nueva notificaciÃ³n                 |
| GET         | /api/v1/notifications/user/{userId}           | Obtiene notificaciones por ID de usuario           | Ver notificaciones de usuario especÃ­fico   |
| GET         | /api/v1/notifications/device/{deviceId}       | Obtiene notificaciones por ID de dispositivo       | Ver notificaciones de dispositivo          |
| GET         | /api/v1/settings                              | Obtiene configuraciones del usuario                | Ver configuraciones actuales               |
| PUT         | /api/v1/settings                              | Actualiza configuraciones del usuario              | Modificar configuraciones                  |
| POST        | /api/v1/settings/rules                        | AÃ±ade regla de ahorro                              | Crear nueva regla de ahorro                |
| PUT         | /api/v1/settings/rules/{ruleId}               | Actualiza regla de ahorro                          | Editar regla existente                     |
| DELETE      | /api/v1/settings/rules/{ruleId}               | Elimina regla de ahorro                            | Remover regla de ahorro                    |
| GET         | /api/v1/reports/weekly-consumption            | Obtiene reporte de consumo semanal                 | Generar reporte semanal                    |
| GET         | /api/v1/reports/top-devices                   | Obtiene los 3 dispositivos que mÃ¡s consumen        | Ver dispositivos con mayor consumo         |
| GET         | /api/v1/users                                 | Obtiene lista de usuarios                          | Listar todos los usuarios                  |
| GET         | /api/v1/users/{id}                            | Obtiene usuario por ID                             | Ver datos de usuario especÃ­fico            |
| GET         | /api/v1/users/{userId}/preferences            | Obtiene preferencias del usuario                   | Ver preferencias del usuario               |
| PUT         | /api/v1/users/{userId}/preferences            | Actualiza preferencias del usuario                 | Modificar preferencias                     |
| GET         | /api/v1/roles                                 | Obtiene lista de roles                             | Listar roles disponibles                   |
| GET         | /api/v1/roles/{id}                            | Obtiene rol por ID                                 | Ver detalles del rol especÃ­fico            |
| GET         | /api/v1/dashboard                             | Obtiene datos del dashboard                        | Mostrar mÃ©tricas del dashboard             |

#### 5.2.4.7. Software Deployment Evidence for Sprint Review

Durante este Sprint 4, se completÃ³ la integraciÃ³n completa del sistema Energix, incluyendo el despliegue de la landing page, frontend, backend y base de datos en plataformas en lÃ­nea. El objetivo fue contar con una versiÃ³n funcional y accesible del sistema completo para revisiÃ³n y retroalimentaciÃ³n.

Actividades realizadas:

- Se desplegÃ³ la landing page en Netlify: https://energixlp.netlify.app

- Se desplegÃ³ el frontend en Vercel: https://frontend-sems.vercel.app

- Se desplegÃ³ el backend en Render utilizando un proxy seguro de Cloudflare: https://theft-muscles-inner-protection.trycloudflare.com

- Se configurÃ³ la base de datos en Aiven con los parÃ¡metros necesarios para la integraciÃ³n completa.

Se verificÃ³ la correcta publicaciÃ³n de todos los componentes del sistema.

#### 5.2.4.8. Team Collaboration Insights during Sprint

En esta secciÃ³n se evidencia la colaboraciÃ³n de cada integrante en los repositorios de la aplicaciÃ³n.

Repositorio de la Landing Page: https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page

Repositorio del Frontend de la AplicaciÃ³n: https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Frontend-SEMS

Repositorio del Backend de la AplicaciÃ³n: https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS

| **Integrante**                       | **Actividad**                                                                                            |  
|--------------------------------------|----------------------------------------------------------------------------------------------------------|
| **Huaman Olivos, Yeira Shari**       | ImplementaciÃ³n de secciones del **Backend de la AplicaciÃ³n** y contribuciones a los **chapter 5.md**     |
| **Loechle Arias, Mateo Ãtalo**       | ImplementaciÃ³n de secciones del **Backend de la AplicaciÃ³n** y contribuciones a los **chapter 5.md**     |
| **Barturen Panez, Iker Gabriel**     | ImplementaciÃ³n de secciones del **Backend de la AplicaciÃ³n** y contribuciones a los **chapter 5.md**     |
| **Encalada Salazar, Alexis**         | ImplementaciÃ³n de secciones del **Backend de la AplicaciÃ³n** y contribuciones a los **chapter 5.md**     |
| **Torres Lavandera, AndrÃ©s Rodrigo** | ImplementaciÃ³n de secciones del **Backend de la AplicaciÃ³n** y contribuciones a los **chapter 5.md**     |
| **Ynga Amado, Jafeth Worren**        | ImplementaciÃ³n de secciones del **Backend de la AplicaciÃ³n** y contribuciones a los **chapter 5.md**     |

#### 5.3. Validation Interviews

Las entrevistas de validaciÃ³n representan una fase crucial en el proceso de desarrollo del producto SEMS (Sistema de Monitoreo EnergÃ©tico Inteligente). Esta metodologÃ­a nos permite evaluar la efectividad, usabilidad y aceptaciÃ³n de la soluciÃ³n implementada por parte de nuestros segmentos objetivo identificados en el capÃ­tulo anterior.

#### 5.3.1. DiseÃ±o de Entrevistas

El diseÃ±o de las entrevistas de validaciÃ³n se estructura en torno a la evaluaciÃ³n prÃ¡ctica del producto SEMS desarrollado. Las entrevistas estÃ¡n dirigidas a los mismos segmentos objetivo identificados en el capÃ­tulo 2: propietarios de vivienda y estudiantes que alquilan, con el fin de validar si la soluciÃ³n implementada satisface sus necesidades especÃ­ficas de monitoreo energÃ©tico.

#### Preguntas para Segmento #1: Propietarios de Vivienda

1. Al ingresar a la plataforma, Â¿quÃ© es lo primero que llama su atenciÃ³n?
2. Sin leer instrucciones, Â¿puede identificar cuÃ¡l es el propÃ³sito principal de esta aplicaciÃ³n?
3. Â¿La informaciÃ³n presentada en el dashboard le resulta clara y comprensible?
4. Â¿Puede localizar fÃ¡cilmente la informaciÃ³n sobre su consumo energÃ©tico actual?
5. Â¿QuÃ© opina sobre la forma en que se presentan los datos de consumo (grÃ¡ficos, nÃºmeros, alertas)?
6. Â¿Las alertas de consumo le resultan Ãºtiles y fÃ¡ciles de entender?
7. Â¿La funciÃ³n de control remoto de dispositivos le parece intuitiva de usar?
8. Â¿Considera que esta herramienta podrÃ­a ayudarle realmente a reducir sus gastos de electricidad?
9. Â¿QuÃ© funcionalidad le resulta mÃ¡s valiosa de las que ha visto?
10. Â¿El diseÃ±o y colores le transmiten confianza y profesionalismo?
11. Â¿Encuentra alguna dificultad para navegar entre las diferentes secciones?
12. Â¿Los Ã­conos y botones son claros en su funciÃ³n?
13. BasÃ¡ndose en lo que ha visto, Â¿estarÃ­a dispuesto(a) a usar esta plataforma regularmente?
14. Â¿RecomendarÃ­a esta soluciÃ³n a otros propietarios de vivienda?
15. Â¿QuÃ© mejorarÃ­a para que la plataforma sea perfecta para sus necesidades?

#### Preguntas para Segmento #2: Estudiantes que Alquilan

1. Â¿La interfaz le parece amigable para alguien de su perfil tecnolÃ³gico?
2. Â¿Puede entender rÃ¡pidamente cÃ³mo esta aplicaciÃ³n le ayudarÃ­a a gestionar sus gastos de luz?
3. Â¿La informaciÃ³n se presenta de una manera que le resulte familiar y fÃ¡cil de procesar?
4. Â¿Los datos de consumo le ayudan a entender mejor en quÃ© se va su dinero de electricidad?
5. Â¿Las alertas le parecen Ãºtiles para controlar mejor sus gastos mensuales?
6. Â¿Puede identificar fÃ¡cilmente cuÃ¡nto podrÃ­a ahorrar usando esta herramienta?
7. Â¿La funciÃ³n de monitoreo en tiempo real le resulta prÃ¡ctica para su estilo de vida?
8. Â¿Esta herramienta le ayudarÃ­a a mantenerse dentro de su presupuesto mensual?
9. Â¿QuÃ© caracterÃ­stica considera mÃ¡s importante para su situaciÃ³n como estudiante?
10. Â¿El ahorro promedio mostrado le parece realista y atractivo?
11. Al ser una aplicaciÃ³n responsive, Â¿Puede usar la aplicaciÃ³n fÃ¡cilmente desde su dispositivo mÃ³vil?
12. Â¿Hay algo que le parezca confuso o complicado de entender?
13. Â¿Con quÃ© frecuencia cree que usarÃ­a esta plataforma?
14. Â¿Se siente motivado(a) a cambiar sus hÃ¡bitos de consumo despuÃ©s de ver esta herramienta?


#### 5.3.2. Registro de Entrevistas

Esta secciÃ³n se dedica a la documentaciÃ³n sistemÃ¡tica de cada entrevista con los segmentos objetivo. Se organiza la informaciÃ³n para presentar el perfil de cada entrevistado, junto con sus respuestas directas y los hallazgos mÃ¡s significativos. Este registro es crucial para comprender la perspectiva del usuario y validar nuestro proyecto.

**ENTREVISTAS SEGMENTO OBJETIVO 1: PROPIETARIOS DE VIVIENDA**

**ENTREVISTA 1**

Link de las entrevistas

Foto de la entrevista
![EntrevistaEmpe.png](assets/EntrevistaEmpe.png)

Inicia:00.00

DuraciÃ³n:10:07

Nombre: Emperatriz Sessarego

Edad: 57

Distrito: JesÃºs MarÃ­a
 
Resumen: La propietaria de vivienda Emperatriz regresa para ser presentada ante la pÃ¡gina web junto a beneficios que ofrecemos y luego es redirigida hacia la aplicaciÃ³n web donde se le hizo un recurrido sobre las diferentes herramientas que ofrece la aplicaciÃ³n. Emperatriz resume su experiencia como agradeble, cree que la plataforma le serÃ¡ uitl al momento de controlar su consumo energÃ©tico. Define la aplicaciÃ³n como fÃ¡cile de enterder y navegar y concluye que si usarÃ­a la aplicaciÃ³n y la recomendarÃ­a a otros propietarios de vivienda.



**ENTREVISTA 2**

Foto de la entrevista
![EntrevistaAna.png](assets/EntrevistaAna.png)
Inicia:00:00

DuraciÃ³n: 05:43

Nombre: Ana Vivar

Edad: 28 

Distrito: San Miguel 

Resumen: La propietaria de vivienda Ana Vivar evaluÃ³ la aplicaciÃ³n web y afirmÃ³ que sÃ­ estarÃ­a dispuesta a utilizarla, resaltando que le pareciÃ³ intuitiva, clara y fÃ¡cil de navegar. DestacÃ³ que los datos detallados sobre el consumo energÃ©tico le serÃ­an muy Ãºtiles para optimizar el uso de energÃ­a en su hogar y reducir su factura elÃ©ctrica, y que el diseÃ±o de la plataforma transmite profesionalismo, con botones bien definidos y un dashboard especialmente valioso por la forma en que presenta la informaciÃ³n. AdemÃ¡s, mencionÃ³ que recomendarÃ­a la aplicaciÃ³n a amigos que, como ella, son propietarios de vivienda.


**ENTREVISTAS SEGMENTO OBJETIVO 2: ESTUDIANTES QUE ALQUILAN**

**ENTREVISTA 1**

![Entrevista-1-Estudiantes.png](assets/Entrevista-1-Estudiantes.png)

Inicia: 00:00

DuraciÃ³n: 

Nombre: Johnny Ricardo Mallqui Cueva

Edad: 19

Distrito: Chorrillos

Resumen: Johnny Mallqui (19 aÃ±os) estudia en la UPC y alquila un cuarto en Chorrillos, se relaciaona a menudo con la tecnologÃ­a ya que estudia ingenierÃ­a de Sistemas. Al probar nuestra herramienta nos comento que fue de su agrado y qeu si la usaria, mas que nada si esta se puede usar en un dispositivo movil ya que si una herramienta que solo esta disponible para laptop o PC, nos comento que no valdria la pena, en su caso si esta dispuesto a usarla, ya que al usar tantos dispositivos, seria una herramienta que facilite el ahorro de consumo energetico, tambien nos menciono que la aplicacion es intuitiva y que es muy facil de usar. 

**ENTREVISTA 2**

Foto de la entrevista 
![EntrevistaSimon.png](assets/EntrevistaSimon.png)
Inicia: 00:00

DuraciÃ³n: 04:21 

Nombre: SimÃ³n Gabriel Molina Chirinos

Edad: 19

Distrito: Pueblo Libre

Resumen:SimÃ³n es un estudiante que alquila un cuarto. SegÃºn sus propias palabras, la interfaz de la aplicaciÃ³n le parece amigable, ay que todo estÃ¡ bien distribuido y es intuitivo. AdemÃ¡s, el diseÃ±o de la aplicaciÃ³n le resulta cÃ³modo para entender los datos. Asmimismo, comprende de quÃ© manera los datos se relacionan con sus gastos en sÃ­. Menciona que las alertas de la aplicaciÃ³n le parecen Ãºtiles para identificar alguna anomalÃ­a en sus consumos. TambiÃ©n, se siente motivado al ver que puede visualizar una estimaciÃ³n de ahorros. Le resulta Ãºtil el monitoreo constante, ya que puede corregir malos hÃ¡bitos al momento. AdemÃ¡s, considera que esta aplicaciÃ³n tendrÃ­a un impacto positivo en cuanto al recibo mensual de luz. TambiÃ©n, considera que lo mÃ¡s importante de esta aplicaciÃ³n es el apartado visual, ya que le ayuda a entender mejor los datos y gestionar su consumo. Asimismo, considera que los iconos de la aplicaciÃ³n podrÃ­an tener alguna breve explicaciÃ³n sobre su uso. Finalmente, el entrevistado declara que la aplicaciÃ³n le beneficiarÃ­a totalmente a mejorar sus hÃ¡bitos y su consumo energÃ©tico.

#### 5.3.3. Evaluaciones segÃºn heurÃ­sticas

                  **UX Heuristicis & Principles Evaluation**
            **Usability - Inclusive Desing - Information Architecture**

Carrera : IngenierÃ­a de Software

Curso : Desarrollo de Aplicaciones Open Source

SecciÃ³n : 7401

Profesor : Hugo Allan Mori Paiva 

Auditor : ENERGIX - SEMS

Clientes(S): Emperatriz Sessarego


Site O APP a evaluar : ENERGIX - SEMS

Tareas a evaluar: 

El enlace de esta evaluaciÃ³n incluye la revisiÃ³n de la usabilidad de las sigueintes tareas:

1. VisualicaciÃ³n de la Landing Page
2. ComprensiÃ³n del valor ofrecido por Energix
3. Proceso de registro
4. Primera navegaciÃ³n dentro de la aplicaciÃ³n 
5. ComprensiÃ³n de mÃ©tricas (promedios, consumos)
6. VinculaciÃ³n de dispositivos
7. PercepciÃ³n general del flujo de uso

No estÃ¡n incluidas en esta versiÃ³n de la evaluaciÃ³n las siguientes tareas:

1. IntegraciÃ³n con dispositivos fÃ­sicos reales
2. GestiÃ³n avanzada del perfil
3. PersonalizaciÃ³n de alertas y notificaciones
4. Flujos administrativos o de facturaciÃ³n 
5. VisualicaciÃ³n de consumo hitÃ³rico a profundidad

 **Escala de Severidad:**

Los errores serÃ¡n puntuados tomando en cuenta las siguiente escala de severidad

| **Nivel** | **DescripciÃ³n**                                                                                                                                                    |  
|-----------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1         | Problema superficial: puede ser fÃ¡cilmente superado por el usuario o ocurre con muy poca frecuencia. No necesita ser arreglado salvo que exista tiempo disponible. |
| 2         | Problema menor: puede ocurrir un poco mÃ¡s frecuentemente o es ligeramente mÃ¡s difÃ­cil de superar. Se recomienda atenderlo en el siguiente release.                 |
| 3         | Problema mayor: ocurre con frecuencia o los usuarios no pueden resolverlo por sÃ­ mismos. Se debe corregir con prioridad alta                                       |
| 4         | Problema muy grave: impide al usuario continuar. Debe corregirse antes del lanzamiento.                                                                            |


**Tabla Resumen:**

| # | **Problema**                                                                                                                                                                                                              | **Escala de severidad** | **HeurÃ­stica/Principio violada(o)**                                                                                               |
|---|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
| 1 | Complicaciones al momento de ingresar un dispositivo y rellenar el campo de consumo de energÃ­a, al no saber el nÃºmero exacto que consumiÃ³ ese dispositivo por lo que no podrÃ¡ ingresar de manera correcta su dispositivo  | 2                       | Flexibilidad y eficiencia del uso / Conocer al usaurio (el sistema no se adapta completamente a los hÃ¡bitos reales del segmento)  |

**Problema #1**

Seriedad: 2

HeurÃ­stica violada: Flexibilidad y eficiencia de uso / Conocer al usuario

Problema: Complicaciones al momento de ingresar un dispositivo y rellenar el campo de consumo de energÃ­a, al no saber el nÃºmero exacto que consumiÃ³ ese dispositivo por lo que no podrÃ¡ ingresar de manera correcta su dispositivo

Figura: 

![HeurÃ­stica.png](assets/Heur%C3%ADstica.png)

Nota. ElaboraciÃ³n propia.

**RecomendaciÃ³n**

Cambiar el campo de relleno de dispositivos o guiar al usuario a como saber el consumo exacto, o un aproximado, de su dispositivo para que asÃ­ pueda ingresarlo de manera correcta.

https://upcedupe-my.sharepoint.com/:v:/g/personal/u20211g491_upc_edu_pe/IQDtm0AcL_c0QKGTVb4n202MARBQ2nAm9br2eGLkukIA7Uo?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=HHs7jm

#### 5.4. Video About-the-Product

https://upcedupe-my.sharepoint.com/:v:/g/personal/u20211g491_upc_edu_pe/IQBMBgRkkbaZQoNKZogSwzK7ASTIv5MFKZhfDqUM_oBKvvU?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=6NmzRb

### Conclusiones

Nuestro proyecto durante el desarrollo de los diferentes sprints ha logrado cumplir con los objetivos planteados al inicio de nuestro proyecto, llegando a alcanzar un MVP funcional y despliegue: frontend, backend, landing page y base de datos, lo que permite demostraciones y pruebas end-to-end.
Hemos implementado una soluciÃ³n integral que aborda las necesidades de monitoreo y gestiÃ³n energÃ©tica para nuestros segmentos objetivo, propietarios de vivienda y estudiantes que alquilan. La integraciÃ³n completa entre el frontend y backend ha sido un logro significativo, permitiendo una experiencia de usuario fluida y eficiente.
Las entrevistas de validaciÃ³n han proporcionado informaciÃ³n valiosa sobre la usabilidad y aceptaciÃ³n de nuestra soluciÃ³n, confirmando que nuestra aplicaciÃ³n es intuitiva y Ãºtil para nuestros usuarios. Los comentarios recibidos nos han ayudado a identificar Ã¡reas de mejora y a validar que estamos en el camino correcto para satisfacer las necesidades de nuestros usuarios.
El despliegue en plataformas en lÃ­nea ha sido exitoso, permitiendo el acceso a nuestra aplicaciÃ³n desde cualquier lugar y facilitando la demostraciÃ³n de nuestras funcionalidades. Esto ha sido crucial para validar nuestro producto en un entorno real.
En resumen, el desarrollo de nuestro proyecto ha sido exitoso, logrando una integraciÃ³n completa y funcional que satisface las necesidades de nuestros usuarios. Estamos satisfechos con los resultados obtenidos y confiamos en que nuestra soluciÃ³n tendrÃ¡ un impacto positivo en la gestiÃ³n energÃ©tica de nuestros segmentos objetivo.


---

### Recomendaciones

Mejorar los campos al momento de ingresar un dispositivo, ya que algunos usuarios no saben el consumo exacto de su dispositivo y esto puede generar confusiÃ³n al momento de registrar un nuevo dispositivo en la aplicaciÃ³n.
Implementar tutoriales o guÃ­as interactivas dentro de la aplicaciÃ³n para ayudar a los usuarios a familiarizarse con las funcionalidades y maximizar el uso de la plataforma.
Implementar opciones de ayuda para las personas con discapacidad visual, auditiva o motriz, para hacer la aplicaciÃ³n mÃ¡s inclusiva.
Realizar pruebas de usabilidad adicionales con una muestra mÃ¡s amplia de usuarios para identificar posibles mejoras en la experiencia de usuario.
Continuar recopilando comentarios de los usuarios despuÃ©s del lanzamiento para iterar y mejorar continuamente la aplicaciÃ³n.
Explorar la integraciÃ³n con dispositivos inteligentes y tecnologÃ­as IoT para automatizar el monitoreo y control del consumo energÃ©tico.

# BibliografÃ­a

**Angular**
- VersiÃ³n actual: v20
- Angular. (2025). _Angular Documentation_. Recuperado de https://angular.dev

**TypeScript**
- TypeScript. (2025). _TypeScript Handbook_. Recuperado de https://www.typescriptlang.org

**CSS**
- VersiÃ³n actual: CSS3
- Mozilla Foundation. (2025). _MDN CSS Reference_. Recuperado de https://developer.mozilla.org/es/docs/Web/CSS

**HTML**
- VersiÃ³n actual: HTML5
- Mozilla Foundation. (2025). _MDN HTML Reference_. Recuperado de https://developer.mozilla.org/es/docs/Web/HTML

**JavaScript**
- Mozilla Foundation. (2025). _MDN JavaScript Reference_. Recuperado de https://developer.mozilla.org/es/docs/Web/JavaScript

**JSON**
- VersiÃ³n actual: EstÃ¡ndar RFC 8259
- JSON.org. (2024). _Introducing JSON_. Recuperado de https://www.json.org/json-es.html

# Anexos

- Link de la OrganizaciÃ³n
  https://github.com/Upc-pre-1ASI0729-2520-7401-Energix
- Link del Repositorio del Reporte
  https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Proyect-Report
- Link del Repositorio de la landing Page
  https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Energix-Landing-Page
- Link del Repositorio del Frontend de la AplicaciÃ³n Web
  https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Frontend-SEMS
- link del Repositorio del Backend de la AplicaciÃ³n Web
  https://github.com/Upc-pre-1ASI0729-2520-7401-Energix/Backend-SEMS 
- Link de la landing page
  https://energixlp.netlify.app
- Link del Frontend de la AplicaciÃ³n Web
  https://frontend-sems.vercel.app
- Link del Backend de la AplicaciÃ³n Web
  https://theft-muscles-inner-protection.trycloudflare.com
- Link de la DocumentaciÃ³n de la API
  https://theft-muscles-inner-protection.trycloudflare.com/swagger-ui/index.html
- Link del Figma
  https://www.figma.com/design/tmJAly092Cbckme5PFfA6Z/Energix?node-id=26-4210&t=4xEBZLNYgT1IM6IQ-1
- Link del video de la presentaciÃ³n
  https://upcedupe-my.sharepoint.com/:v:/g/personal/u20211g491_upc_edu_pe/EatERr_u0z9PsPV9zBCf2qMBBoBO00PC-Phz8dJyZh1iqw?e=RAb0qG
- Link entrevista sector propietario de vivienda #1
  https://upcedupe-my.sharepoint.com/:v:/g/personal/u20211g491_upc_edu_pe/IQDtm0AcL_c0QKGTVb4n202MARBQ2nAm9br2eGLkukIA7Uo?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=HHs7jm
- Link entrevista sector propietario de vivienda #2
  https://upcedupe-my.sharepoint.com/:v:/g/personal/u20211g491_upc_edu_pe/IQAXsgGxJZCwR5eFhUh0CMDWAWvq2dZPMMWJKTpcCTocupY?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=xPgl48
- Link entrevista sector estudiante #1
  https://upcedupe-my.sharepoint.com/:v:/g/personal/u20211g491_upc_edu_pe/IQADaQcdzzp0Qqm_tbgwlU7CAaav4-E6-z39dvRS6P2YqWY?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=7zcGoF
- Link entrevista sector estudiante #2
  https://upcedupe-my.sharepoint.com/:v:/g/personal/u20211g491_upc_edu_pe/IQDqn_-FIILbRKryQAhvq9DbAciKO12cO4dR5XIu6PgI-7Q?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=PPthd0
- Link video-about-team
  https://upcedupe-my.sharepoint.com/:v:/g/personal/u20211g491_upc_edu_pe/IQC00BXTE4A6SbyrQPvdosB6AZM1EWFJ8cu5V_esCS3jf7Q?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=fdv3jR
- Link video about-the-product
  https://upcedupe-my.sharepoint.com/:v:/g/personal/u20211g491_upc_edu_pe/IQBMBgRkkbaZQoNKZogSwzK7ASTIv5MFKZhfDqUM_oBKvvU?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=6NmzRb






# Capítulo V: Product Implementation, Validation & Deployment

## 5.1. Software Configuration Management

En esta sección como equipo establecimos las decisiones y convenciones que nos permitirán mantener la consistencia durante el ciclo de vida.

### 5.1.1. Software Development Environment Configuration

En la siguiente sección se describe la ruta de referencia de cada uno de los productos de software para que cualquier miembro del equipo pueda desarrollar cada punto del trabajo.

- **UXPressia:** Plataforma que nos permitirá crear los user stories y también realizar múltiples mapas para evaluar sus prioridades. Además, ofrece opciones gráficas para mejorar el aspecto de nuestro trabajo. Puedes acceder a la plataforma en el siguiente enlace: [UXPressia](https://www.uxpressia.com/)
- **Figma:** Herramienta colaborativa que nos permitirá desarrollar los respectivos Wireframes y Mockups de nuestra Landing Page. Se puede acceder a la plataforma en el siguiente enlace: [Figma](https://www.figma.com/).
- **Vertabelo:** Plataforma que nos permitirá crear nuestro Diagrama de Base de Datos. Se puede acceder a la plataforma en el siguiente enlace: [Vertabelo](https://www.vertabelo.com/).
- **LucidChart:** Aplicación web destinada a la elaboración de Wireflows, Lean UX Canvas, User Flows y Diagramas de clases. Se puede acceder a la plataforma en el siguiente enlace: [LucidChart](https://www.lucidchart.com/).
- **GitHub:** Repositorio colaborativo en la nube utilizado para almacenar los avances de nuestro proyecto. Se puede acceder a la plataforma en el siguiente enlace: [Github](https://github.com/).
- **Visual Studio Code:** Entorno de desarrollo utilizado por nuestro equipo para el desarrollo del proyecto en general, incluido el Informe. Se puede acceder a la plataforma en el siguiente enlace: [Visual Studio Code](https://code.visualstudio.com/).
- **GitHub Pages:** Plataforma que permite hacer deployments sencillos y rápidos para nuestras páginas web. Se puede acceder a la plataforma en el siguiente enlace: [Github Pages](https://pages.github.com/).

- **HTML5:** Lenguaje para la elaboración de nuestra página web.
- **CSS3:** Tecnología para darle estilos a nuestra página web.
- **JavaScript:** Lenguaje de programación orientado a objetos que nos sirvió para implementar funcionalidades en nuestra Landing Page.

### 5.1.2. Source Code Management

Para gestionar las modificaciones en nuestro proyecto, emplearemos GitHub como plataforma y sistema de control de versiones. A continuación, se detallan los repositorios de GitHub para cada uno de nuestros productos:

- Organización del Equipo: https://github.com/Open-Source-The-Project-Chow
- Repositorio del Informe: https://github.com/Open-Source-The-Project-Chow/Informe-Final
- Repositorio del Landing Page: https://github.com/Open-Source-The-Project-Chow/Landing-page
- Enlace del Landing Page: https://open-source-the-project-chow.github.io/Landing-page/

Para estructurar nuestro control de versiones, implementaremos el modelo GitFlow como nuestro flujo de trabajo estándar. Este modelo se basa en dos ramas principales: main (rama principal) y develop (rama de desarrollo), y varias ramas auxiliares, incluyendo feature, release, y hotfix, cada una con un propósito específico:

#### Ramas Principales:

- Main Branch (Rama Principal): Esta rama contiene siempre el código en producción, es decir, el código que ha sido liberado y que es estable. No se realizan cambios directos en esta rama, excepto para la integración de release branches o hotfix branches.

- Develop Branch (Rama de Desarrollo): Esta rama sirve como base para el desarrollo continuo. Aquí se integran los cambios provenientes de las feature branches. La rama develop contiene la última versión del código con nuevas funcionalidades que aún no han sido liberadas.

- Release Branches: Antes de lanzar una nueva versión, crearemos una rama de release para realizar pruebas finales y correcciones.
- Hotfix Branches: En caso de surgir problemas en el desarrollo, se crearán branches de hotfix para poder solucionarlos sin afectar la rama principal.

#### Ramas Auxiliares:

- Feature Branches: Estas ramas se utilizan para desarrollar nuevas funcionalidades o mejoras específicas. Cada funcionalidad se desarrolla en su propia rama, que se deriva de develop y se fusiona de nuevo en develop una vez que la funcionalidad ha sido completada y probada.

- Release Branches: Estas ramas se utilizan para preparar una nueva versión de producción. Una vez que develop ha alcanzado un estado estable, se crea una release branch para realizar ajustes finales y pruebas antes de fusionarla en main.

- Hotfix Branches: Estas ramas se utilizan para corregir rápidamente problemas en producción. Se derivan de main y, una vez corregido el problema, se fusionan tanto en main como en develop para asegurar que la corrección se mantenga en el desarrollo futuro.

Además, los mensajes de commit seguirán el formato de Conventional Commits, que estandariza los mensajes para que sean claros y útiles. Este formato sigue la estructura:

tipo(<área opcional>): <descripción>

Ejemplos de tipos comunes:

- feat: para nuevas funcionalidades.
- fix: para corrección de errores.
- docs: para cambios en la documentación.
- style: para cambios que no afectan la lógica del código (espacios, formateo, etc.).

### 5.1.3. Source Code Style Guide & Conventions

A continuación, se detallan las referencias y convenciones que adoptaremos para programar en los diferentes lenguajes utilizados en nuestro proyecto:

Utilizaremos las siguientes referencias para establecer nuestras convenciones.
1. **HTML**:
- "HTML Style Guide and Coding Conventions"
- "Google HTML/CSS Style Guide"

2. **CSS**:
- "Google HTML/CSS Style Guide"

3. **JavaScript**:
- "Google JavaScript Style Guide"
- "MDN JavaScript guidelines"
- "W3C JavaScript Style Guide"
- "Angular coding style guide".

4. **Gherkin**:
- "Gherkin Conventions for Readable Specifications".

Es importante destacar que todas las convenciones y referencias mencionadas están en inglés, siguiendo las prácticas comunes en el desarrollo de software. De tal modo que, al seguir estas referencias nos ayudará a mantener un código claro, coherente y fácilmente comprensible para todo el equipo de desarrollo.

### 5.1.4. Software Deployment Configuration

Para desplegar nuestra landing page en la plataforma de GitHub, seguimos los siguientes pasos:

1. Creación del Repositorio Remoto en GitHub:

- Creamos un nuevo repositorio en GitHub de nuestro proyecto, el cual se utilizará para el desarrollo y deployment.

2. Inicialización del Repositorio:

- Se utilza el comando "*git init*" para inicializar el repositorio.

3. Subida de Archivos al Repositorio Remoto:

- Añadimos los archivos de nuestra landing page al repositorio local.
- Subimos los archivos al repositorio de GitHub con el comando "*git push -u origin master*" o sino utilizando Github Desktop.

4. Configuración de GitHub Pages:

- Accedemos a la sección de configuración del repositorio en GitHub y entramos a la sección de Github Pages.

- Seleccionamos la rama de GitHub Pages (main) como fuente para el deployment de nuestra Landing Page

5. Despliegue:

- Accedemos a la URL proporcionada por GitHub Pages para verificar que nuestra landing page se haya desplegado correctamente.

De tal modo, nuestra Landing Page estará inicializada utilizando Github Pages y podrá ser visible para cualquier usuario que tenga el enlace.

Enlace del Landing Page: https://open-source-the-project-chow.github.io/Landing-page/

## 5.2. Landing Page, Services & Applications Implementation

En esta sección se explicará y evidenciará el proceso de implementación, pruebas,
documentación y despliegue del Landing Page.

### 5.2.1. Sprint 1

### 5.2.1.1. Sprint Planning 1

Para este primer sprint nos enfocaremos en los tasks para la
elaboración del Landing Page. Nos dividiremos entre nosotros cada
una de las tareas identificadas para el sprint.
<table>
<tr>
    <th colspan="5">Sprint #</th>
    <th colspan="9">Sprint 1</th>
  </tr>
      <tr>
    <td colspan="13">Sprint Planning Background</td>
  </tr>
  <tr>
    <td colspan="5">Date</td>
    <td colspan="8">2024-08-25</td>
</tr>
  <tr>
    <td colspan="5">Time</td>
    <td colspan="8">10:38 PM</td>
  </tr>
  <tr>
    <td colspan="5">Location</td>
    <td colspan="8">Via Discord y Google Meet</td>
<tr>
    <td colspan="5">Prepared By</td>
    <td colspan="8">Gabriel Garcia</td>
</tr>
<tr>
    <td colspan="5">Attendees (to planning meeting)</td>
    <td colspan="8">Gabriel Garcia, Diego Flores, Salvador Chamorro, Héctor Rentería, Bryan Espejo</td>
</tr>
<tr>
    <td colspan="5">Sprint n – 1 Review Summary</td>
    <td colspan="8">En esta seccion se planteo el desarrollo del landing page para nuestro proyecto llamado CraftSync</td>
</tr>
<tr>
    <td colspan="5">Sprint n – 1 Retrospective Summary</td>
    <td colspan="8">En esta seccion todos los integrantes mencionaron tener aciertos en partes del codigo y en otras partes poder mejorar sus habilidades realizando landing pages</td>
</tr>
<tr>
    <td colspan="13">Sprint Goal & User Stories</td>
</tr>
<tr>
    <td colspan="5">Sprint n Goal</td>
    <td colspan="8">Culminar el landing Page</td>
</tr>
<tr>
    <td colspan="5">Sprint n Velocity</td>
    <td colspan="8">5 story points</td>
</tr>
<tr>
    <td colspan="5">Sum of Story Points</td>
    <td colspan="8">6 Story Points</td>
</tr>
</table>

### 5.2.1.2. Sprint Backlog 1

<table>
<tr>
    <th colspan="3">Sprint #</th>
    <th colspan="10">Sprint 1</th>
  </tr>
      <tr>
    <td colspan="3">User Story</td>
    <td colspan="10">Work-Item/Task</td>
  </tr>
  <tr>
    <td colspan="1">Id</td>
    <td colspan="2">Title</td>
    <td colspan="1">Id</td>
    <td colspan="2">Title</td>
    <td colspan="3">Description</td>
    <td colspan="1"> Estimation</td>
    <td colspan="2">Assigned To</td>
    <td colspan="1">Status(To-do /InProcess /To-Review /Done)</td>
</tr>
  <tr>
    <td colspan="1">US01</td>
    <td colspan="2">Sección About Us</td>
    <td colspan="1">T01</td>
    <td colspan="2">Añadir sección About Us en el Landing Page</td>
    <td colspan="3">Yo, como distribuidor visitante del Landing Page, quiero una sección About Us para informarme sobre la empresa y sus detalles.</td>
    <td colspan="1">1</td>
    <td colspan="2">Diego</td>
    <td colspan="1">Done</td>
  </tr>
  <tr>
    <td colspan="1">US25</td>
    <td colspan="2">Visualización de los servicios disponibles</td>
    <td colspan="1">T02</td>
    <td colspan="2">Añadir sección Services en el Landing Page</td>
    <td colspan="3">Como Artesano/Distribuidor visitante del Landing page de CraftSync, quiero una sección “Services” para informarme sobre los servicios que ofrece la plataforma.</td>
    <td colspan="1">1</td>
    <td colspan="2">Salvador</td>
    <td colspan="1">Done</td>
<tr>
    <td colspan="1">US24</td>
    <td colspan="2">Visualización de lista de tipos de suscripción</td>
    <td colspan="1">T03</td>
    <td colspan="2">Añadir sección Plans en el Landing Page</td>
    <td colspan="3">Como Artesano/Distribuidor visitante del Landing page de CraftSync, quiero visitar la lista de tipos de suscripción para seleccionar alguno.</td>
    <td colspan="1">1</td>
    <td colspan="2">Marcelo</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US23</td>
    <td colspan="2">Visualización de la sección Contact Us</td>
    <td colspan="1">T04</td>
    <td colspan="2">Añadir sección Contact Us al Landing Page</td>
    <td colspan="3">Como Artesano/Distribuidor visitante del Landing page de CraftSync, quiero una sección “Contact us” para solicitar información acerca de la plataforma</td>
    <td colspan="1">1</td>
    <td colspan="2">Gabriel</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US22</td>
    <td colspan="2">Visualización de los desarrolladores</td>
    <td colspan="1">T05</td>
    <td colspan="2">Añadir sección Creators al Landing Page</td>
    <td colspan="3">Como Artesano/Distribuidor visitante del Landing page de CraftSync, quiero una sección “Creadores” para informarme sobre los desarrolladores de la plataforma.</td>
    <td colspan="1">1</td>
    <td colspan="2">Bryan</td>
    <td colspan="1">Done</td>
</tr>
<tr>
    <td colspan="1">US02</td>
    <td colspan="2">Selector de Idioma</td>
    <td colspan="1">T06</td>
    <td colspan="2">Añadir un botón que cambie el idioma del texto mostrado</td>
    <td colspan="3">Yo, como distribuidor visitante del Landing Page, quiero un selector de idioma para leer el contenido en mi idioma de preferencia.</td>
    <td colspan="1">1</td>
    <td colspan="2">Marcelo</td>
    <td colspan="1">InProcess</td>
</tr>
</table>

### 5.2.1.3. Development Evidence for Sprint Review

<table>
    <tr>
        <th colspan="2">Repository</th>
        <th colspan="2">Branch</th>
        <th colspan="2">Commit Id</th>
        <th colspan="2">Commit Message</th>
        <th colspan="2">Commit Message Body</th>
        <th colspan="2">Commited on (Date)</th>
    </tr>
        <tr>
        <td colspan="2">Open-Source-The-Project-Chow/Landing-page</td>
        <td colspan="2">Main</td>
        <td colspan="2">f5d9fcc58f6fd2d8427bdba752fd785f6320917c</td>
        <td colspan="2">Initial commit</td>
        <td colspan="2">-</td>
        <td colspan="2">25/08/2024</td>
    </tr>
        <tr>
        <td colspan="2">Open-Source-The-Project-Chow/Landing-page</td>
        <td colspan="2">Main</td>
        <td colspan="2">b7b42a92091922d250317487e5a217839520b21b</td>
        <td colspan="2">feat: added contact us section.</td>
        <td colspan="2">-</td>
        <td colspan="2">02/09/2024</td>
    </tr>
     <tr>
        <td colspan="2">Open-Source-The-Project-Chow/Landing-page</td>
        <td colspan="2">Main</td>
        <td colspan="2">c4d528fcb2b49e0139ee2c102ca42c6ed43ff6de</td>
        <td colspan="2">feat: added contact us section styles.</td>
        <td colspan="2">-</td>
        <td colspan="2">02/09/2024</td>
    </tr>
    <tr>
        <td colspan="2">Open-Source-The-Project-Chow/Landing-page</td>
        <td colspan="2">Main</td>
        <td colspan="2">f03d4381e72b5b5e63ca81f27092c64ac0ddec8e</td>
        <td colspan="2">feat(header): added navbar.</td>
        <td colspan="2">-</td>
        <td colspan="2">03/09/2024</td>
    </tr>
    <tr>
        <td colspan="2">Open-Source-The-Project-Chow/Landing-page</td>
        <td colspan="2">Main</td>
        <td colspan="2">be8e8eda97562ec0d04fed20d8b6fe4ed9e396a1</td>
        <td colspan="2">feat(header): added javascript function for the menu.</td>
        <td colspan="2">-</td>
        <td colspan="2">03/09/2024</td>
    </tr>
    <tr>
        <td colspan="2">Open-Source-The-Project-Chow/Landing-page</td>
        <td colspan="2">Main</td>
        <td colspan="2">5b06567cb71a165535b3a7345a5668f4d9ff10c9</td>
        <td colspan="2">faet(header): added background image and logo.</td>
        <td colspan="2">-</td>
        <td colspan="2">03/09/2024</td>
    </tr>
    <tr>
        <td colspan="2">Open-Source-The-Project-Chow/Landing-page</td>
        <td colspan="2">Main</td>
        <td colspan="2">7d0f7d76293d10f9daa4a95e791fa06544714cd2</td>
        <td colspan="2">feat(plans): Added Plans section index.</td>
        <td colspan="2">-</td>
        <td colspan="2">04/09/2024</td>
    </tr>
    <tr>
        <td colspan="2">Open-Source-The-Project-Chow/Landing-page</td>
        <td colspan="2">Main</td>
        <td colspan="2">b217183d00b244b72869bee16853fe1ba8d2f48f</td>
        <td colspan="2">feat(plans): Added Plans section styles.</td>
        <td colspan="2">-</td>
        <td colspan="2">04/09/2024</td>
    </tr>
    <tr>
        <td colspan="2">Open-Source-The-Project-Chow/Landing-page</td>
        <td colspan="2">Main</td>
        <td colspan="2">77672962d0d4d5825b6adcfb5fe5362b2620c7e1</td>
        <td colspan="2">feat(services): Added services section</td>
        <td colspan="2">-</td>
        <td colspan="2">04/09/2024</td>
    </tr>
    <tr>
        <td colspan="2">Open-Source-The-Project-Chow/Landing-page</td>
        <td colspan="2">Main</td>
        <td colspan="2">7d4fb5e6d73ba415a58159c94196f6f8a9d64a3c</td>
        <td colspan="2">feat(services): Added services section styles</td>
        <td colspan="2">-</td>
        <td colspan="2">04/09/2024</td>
    </tr>
    <tr>
        <td colspan="2">Open-Source-The-Project-Chow/Landing-page</td>
        <td colspan="2">Main</td>
        <td colspan="2">b22e13a9389f6db6a1753d2d69d3a98f695bcf98</td>
        <td colspan="2">feat(services):added images</td>
        <td colspan="2">-</td>
        <td colspan="2">04/09/2024</td>
    </tr>
    <tr>
        <td colspan="2">Open-Source-The-Project-Chow/Landing-page</td>
        <td colspan="2">Main</td>
        <td colspan="2">0669b4ce80e7f6593c6729f24fbd46459a74e0cc</td>
        <td colspan="2">feat: added section index and styels</td>
        <td colspan="2">-</td>
        <td colspan="2">04/09/2024</td>
    </tr>
    <tr>
        <td colspan="2">Open-Source-The-Project-Chow/Landing-page</td>
        <td colspan="2">Main</td>
        <td colspan="2">1eeb8e46faac2db4b075e2313327fdd02a112eca</td>
        <td colspan="2">fix: fixed little mistakes.</td>
        <td colspan="2">-</td>
        <td colspan="2">05/09/2024</td>
    </tr>
    <tr>
        <td colspan="2">Open-Source-The-Project-Chow/Landing-page</td>
        <td colspan="2">Main</td>
        <td colspan="2">c9a095f5d0fb73dfc77705c65b51dab1db795b63</td>
        <td colspan="2">feat: added footer section.</td>
        <td colspan="2">-</td>
        <td colspan="2">05/09/2024</td>
    </tr>
    <tr>
        <td colspan="2">Open-Source-The-Project-Chow/Landing-page</td>
        <td colspan="2">Main</td>
        <td colspan="2">f203b4c4f5b0ad52cd0e475eb64753bca289c656</td>
        <td colspan="2">feat: added footer styles.</td>
        <td colspan="2">-</td>
        <td colspan="2">05/09/2024</td>
    </tr>
    <tr>
        <td colspan="2">Open-Source-The-Project-Chow/Landing-page</td>
        <td colspan="2">Main</td>
        <td colspan="2">9e3782330ac3a7a08dd2c3b4e2c85e9435f42712</td>
        <td colspan="2">fix: fixed mistake points.</td>
        <td colspan="2">-</td>
        <td colspan="2">05/09/2024</td>
    </tr>
    <tr>
        <td colspan="2">Open-Source-The-Project-Chow/Landing-page</td>
        <td colspan="2">Main</td>
        <td colspan="2">358ac140118a051d77bf0e8d42b5bfdec54233b7</td>
        <td colspan="2">fix: fixed bad calling to image.</td>
        <td colspan="2">-</td>
        <td colspan="2">05/09/2024</td>
    </tr>
</table>

### 5.2.1.4. Testing Suite Evidence for Sprint Review

En este sprint, no se desarrollaron Web Services, por lo que no hubo ningpun Unit Testing relacionado a estos.

### 5.2.1.5. Execution Evidence for Sprint Review

Para esta primera entrega, nuestro equipo a conseguido elaborar la Landing Page del proyecto "CraftSync". De tal modo, se podrá visualizar la información necesaria de lo que ofrece nuestro proyecto.

**Sección de Inicio**: Se implementó el Header y About Us de nuestra Landing Page.
![alt text](../assets/img/evidence1.png)
**Sección de Servicios**: Se implementó la sección de los servicios ofrecidos.
![alt text](../assets/img/evidence2.png)
**Sección de Planes**: Se implementó la sección de ver los tipos de suscripción.
![alt text](../assets/img/evidence3.png)
**Sección de Contacto**:  la sección de contacto para facilitar la comunicación con los usuarios.
![alt text](../assets/img/evidence4.png)
**Sección de Creadores**: Se agregaron secciones de información sobre los creadores del proyecto
![alt text](../assets/img/evidence5.png)
**Sección de Footer**: Se añadió un footer para la navegación y contacto.
![alt text](../assets/img/evidence6.png)

### 5.2.1.6. Services Documentation Evidence for Sprint Review

### 5.2.1.7. Software Deployment Evidence for Sprint Review

Para el despliegue del Landing Page, hemos utilizado la herramienta de Github Pages para poder hacer un deployment. Para eso, hemos creado un repositorio donde hemos colocado el código de desarrollo de nuestra Landing Page.

![alt text](../assets/img/deploy1.png)

Una vez creado el repositorio, entraremos a configuración del repositorio y escogemos el apartado de Pages. Se coloca la información necesaria, como la fuente del branch a utilizar para realizar el deployment. Luego de eso, Github Pages nos brindará el link y desplegará nuestra landing page en la Web.

![alt text](../assets/img/deploy2.png)

### 5.2.1.8. Team Collaboration Insights during Sprint

Para el desarrollo de este primer sprint, todos los miembros del equipo desarrollaron y colaboraron de manera activa y continua. De tal modo, se muestra como evidencia los insights de cada miembro del equipo.

Commits:
![alt text](../assets/img/insight1.png)
Analiticas de Colaboración:
![alt text](../assets/img/insight2.png)

# Conclusiones
- La aplicación permitirá a los artesanos gestionar eficientemente sus pedidos, materiales y procesos de producción, optimizando su flujo de trabajo. Podrán organizar sus inventarios de manera efectiva mediante un sistema de estanterías y actualizar el progreso de sus pedidos, lo que fomenta la transparencia y la mejora de la planificación.
- Los distribuidores tendrán visibilidad en tiempo real del estado de los pedidos que realizan a los artesanos, lo que facilita el control del progreso y los plazos de entrega, promoviendo una mayor confianza y satisfacción en la relación comercial.
- La herramienta de gestión de inventarios facilita la administración de los materiales y recursos que los artesanos utilizan en sus talleres. Esto permitirá un mejor control del stock, la reducción de desperdicios, y la planificación anticipada de compras de insumos necesarios para futuros pedidos.
- Dado que este proyecto es una iniciativa completamente nueva, hay muchas oportunidades para refinar el producto a través de la retroalimentación de usuarios y la experimentación con nuevas características. El uso de métricas clave y el análisis del comportamiento del usuario permitirá ajustar y mejorar la solución de manera continua.

# Bibliografía
- Conne, M(2024). _The Markdown Guide_. MarkdownGuide. Recuperado de: https://www.markdownguide.org/

- Gothelf, J (2016). _Lean UX, 2nd Edition_. O'reilly. Recuperado de: https://learning.oreilly.com/library/view/lean-ux-2nd/9781491953594/foreword01.html

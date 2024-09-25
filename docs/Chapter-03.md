# Capítulo III: Requirements Specification

## 3.1. To-Be Scenario Mapping

Segmento objetivo artesanos:

![artesanos-to-be](/assets/img/artesano-to-be.png)

Segmento objetivo distribuidores:

![distribuidores-to-be](/assets/img/distribuidor-to-be.png)

## 3.2. User Stories

Los User Stories sirven para describir de manera más detallada las diferentes funciones de la aplicación, adaptándolas a las necesidades y prioridades de los usuarios. Estas historias también capturan el propósito de uso de las personas, brindando una comprensión más completa de cómo se relacionan con la aplicación y qué esperan lograr con ella.

<table>
    <tr>
        <th>Epic / Story ID</th>
        <th>Título</th>
        <th>Descripción</th>
        <th>Criterios de Aceptación</th>
        <th>Relacionado con (Epic ID)</th>
    </tr>
    <tr>
        <td>EP01</td>
        <td>Landing Page</td>
        <td>Yo, como visitante del Landing Page, quiero que tenga secciones de información, para saber más del producto.</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>EP02</td>
        <td>Inventario</td>
        <td>Yo, como artesano, quiero herramientas de gestión, para poder manejar mi inventario más fácilmente.</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>EP03</td>
        <td>Comunicación</td>
        <td>Yo, como artesano, quiero opciones de interacción con el distribuidor, para mejorar la relación de trabajo entre los 2.</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>EP04</td>
        <td>Pedidos</td>
        <td>Yo, como distribuidor, quiero funciones relacionadas con los pedidos, para monitorearlos de forma más conveniente.</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>EP05</td>
        <td>Visualización de Apartados</td>
        <td>Yo, como distribuidor, quiero una buena interfaz visual, para mejorar mi experiencia en la plataforma.</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>EP06</td>
        <td>Funciones de Usuario</td>
        <td>Yo, como artesano, quiero distintas funciones de usuario, para realizar las acciones que necesito con mi cuenta.</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>EP07</td>
        <td>Technical Stories</td>
        <td>Yo, como desarrollador, quiero interactuar con el backend API de la aplicación, para conectar funciones de mi aplicación con una base de datos.</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>US01</td>
        <td>Sección About Us</td>
        <td>Yo, como distribuidor visitante del Landing Page, quiero una sección About Us para informarme sobre la empresa y sus detalles.</td>
        <td>
            Scenario: Visualización de una sección About Us<br><br>
            GIVEN un distribuidor visita la Landing Page,<br>
            WHEN baje hasta la sección de "About Us",<br>
            THEN se le brinda información acerca de la empresa cuyos servicios le interesan.
        </td>
        <td>EP01</td>
    </tr>
    <tr>
        <td>US02</td>
        <td>Selector de Idioma</td>
        <td>Yo, como distribuidor visitante del Landing Page, quiero un selector de idioma para leer el contenido en mi idioma de preferencia.</td>
        <td>
            Scenario: Cambio de inglés a español<br><br>
            GIVEN un distribuidor visita la Landing Page,<br>
            WHEN presione el selector de idioma<br>
            THEN el contenido de la página se muestra en español<br><br>
            Scenario 2: Cambio de español a inglés<br><br>
            GIVEN un distribuidor visita la Landing Page,<br>
            AND el contenido esté en español<br>
            WHEN presione el selector de idioma<br>
            THEN el contenido de la página se muestra en inglés
        </td>
        <td>EP01</td>
    </tr>
    <tr>
        <td>US03</td>
        <td>Solicitud de Trabajo</td>
        <td>Yo, como artesano usuario de la plataforma, quiero mandar solicitudes a los distribuidores, para obtener pedidos de su parte.</td>
        <td>
            Scenario 1: Artesano manda una solicitud<br><br>
            GIVEN el artesano está en el perfil de un distribuidor<br>
            WHEN el artesano seleccione la opción de Solicitar Trabajo<br>
            THEN se notifica al distribuidor de la solicitud
        </td>
        <td>EP03</td>
    </tr>
    <tr>
        <td>US04</td>
        <td>Asignar Pedidos</td>
        <td>Yo, como usuario distribuidor de la plataforma, quiero asignar pedidos a los artesanos, para enviarlos a los compradores una vez hechos.</td>
        <td>
            Scenario 1: Distribuidor asigna un pedido<br><br>
            GIVEN el distribuidor está en el perfil de un artesano<br>
            AND el artesano le ha mandado una solicitud de trabajo<br>
            WHEN el distribuidor seleccione la opción de Asignar Pedidos<br>
            AND rellene los datos necesarios<br>
            THEN el pedido aparece en la lista del artesano
        </td>
        <td>EP03</td>
    </tr>
    <tr>
        <td>US05</td>
        <td>Actualizar Progreso</td>
        <td>Yo, como usuario artesano de la plataforma, quiero actualizar los detalles del pedido, para mantener informado al distribuidor.</td>
        <td>
            Scenario 1: Cambiar la cantidad de pedidos hechos<br><br>
            GIVEN el artesano está en viendo un pedido<br>
            AND haya avanzado con el progreso<br>
            WHEN edite la cantidad de pedidos hechos<br>
            AND guarde los cambios<br>
            THEN el distribuidor es notificado del cambio
        </td>
        <td>EP04</td>
    </tr>
    <tr>
        <td>US06</td>
        <td>Visualización de perfil de usuario propio.</td>
        <td>Como Artesano/Distribuidor usuario de la plataforma, quiero visualizar mi perfil para verificar que mi información es correcta.</td>
        <td>
            Scenario 1: Artesano/Distribuidor visualiza su perfil de usuario<br><br>
            GIVEN el Artesano/Distribuidor está en la barra de navegación<br>
            WHEN el Artesano/Distribuidor ingrese a la sección "Perfil",<br>
            THEN obtiene acceso a toda la información de su perfil de usuario.
        </td>
        <td>EP05</td>
    </tr>
    <tr>
        <td>US07</td>
        <td>Visualización de otros perfiles de usuario</td>
        <td>Como Artesano/Distribuidor usuario de la plataforma, quiero visualizar otros perfiles de usuario para ver su información e interactuar.</td>
        <td>
            Scenario 1: Artesano/Distribuidor visualiza el perfil de otros usuarios desde la barra de búsqueda<br><br>
            GIVEN el Artesano/Distribuidor está en la barra de búsqueda,<br>
            WHEN el Artesano/Distribuidor seleccione a un usuario<br>
            THEN obtiene la información del perfil de usuario seleccionado.<br><br>
            Scenario 2: Artesano/Distribuidor visualiza el perfil de otros usuarios desde una publicación<br><br>
            GIVEN el Artesano/Distribuidor  está en el foro,<br>
            WHEN el Artesano/Distribuidor  seleccione a un usuario<br>
            THEN obtiene la información del perfil de usuario seleccionado.
        </td>
        <td>EP05</td>
    </tr>
    <tr>
        <td>US08</td>
        <td>Actualización de  información de perfil.</td>
        <td>Como Artesano/Distribuidor usuario de la plataforma,  quiero poder actualizar mi información personal y de contacto para mantener mis datos actualizados.</td>
        <td>
            Scenario 1: Actualización exitosa de información<br><br>
            GIVEN el Artesano/Distribuidor está en la vista de su perfil,<br>
           WHEN el Artesano/Distribuidor selecciona el botón de editar perfil, actualiza el formulario correctamente y selecciona el botón guardar cambios,<br>
            THEN se ve reflejado el perfil actualizado.<br><br>
            Scenario 2: Error en la actualización por campos obligatorios faltantes<br><br>
            GIVEN el Artesano/Distribuidor está en la vista de su perfil,<br>
            WHEN el Artesano/Distribuidor selecciona el botón de editar perfil<br>
            AND deja algún espacio en blanco en el formulario<br>
            AND selecciona el botón guardar cambios,<br>
            THEN el sistema mostrará un mensaje de error indicando los campos faltantes y no se actualizan los datos del perfil.
        </td>
        <td>EP06</td>
    </tr>
    <tr>
        <td>US09</td>
        <td>Borrar cuenta</td>
        <td>Como Artesano/Distribuidor usuario de la plataforma, quiero borrar mi cuenta para proteger la integridad de mi persona.</td>
        <td>
          Scenario 1: Usuario borra su cuenta satisfactoriamente<br><br>
            GIVEN el artesano está en la vista de su perfil,<br>
          WHEN el artesano selecciona el botón de editar perfil, actualiza el formulario y luego selecciona el botón aceptar<br>
            THEN se ve reflejado el perfil actualizado. 
        </td>
        <td>EP06</td>
    </tr>
    <tr>
        <td>US10</td>
        <td>Cerrar sesión</td>
        <td>Como Artesano/Distribuidor usuario de la plataforma, quiero cerrar sesión para proteger la integridad de mi cuenta.</td>
        <td>
            Scenario 1: Artesano/Distribuidor cierra sesión satisfactoriamente<br><br>
            GIVEN el artesano está en la vista de su perfil,<br>
          WHEN el artesano selecciona el botón de editar perfil, actualiza el formulario y luego selecciona el botón aceptar<br>
            THEN se ve reflejado el perfil actualizado. 
        </td>
        <td>EP06</td>
    </tr>
    <tr>
        <td>US11</td>
        <td>Visualización de la sección de inventarios</td>
        <td>Como artesano usuario de la plataforma, quiero ver mis inventarios de trabajo para estar al tanto de lo que se tiene disponible.</td>
        <td>
            Scenario 1: Acceder a la sección de Inventarios.<br><br>
            GIVEN el artesano está en la barra de navegación,<br>
          WHEN el artesano ingrese a la sección "Inventarios",<br>
            THEN obtiene información de todos los inventarios disponibles. 
        </td>
        <td>EP02</td>
    </tr>
    <tr>
        <td>US12</td>
        <td>Crear inventario</td>
        <td>Como artesano usuario de la plataforma, quiero agregar inventarios para mantener un orden en mis diferentes proyectos.</td>
        <td>
            Scenario 1: Agregar inventario.<br><br>
            GIVEN el artesano está en la sección de inventarios,<br>
            WHEN el artesano selecciona el botón de agregar inventario,<br>
            THEN se agrega un nuevo inventario.
        </td>
        <td>EP02</td>
    </tr>
    <tr>
        <td>US13</td>
        <td>Eliminar inventario</td>
        <td>Como artesano usuario de la plataforma, quiero eliminar inventarios para no tener información innecesaria</td>
        <td>Scenario 1: Eliminar inventario.<br><br>
            GIVEN el artesano está en la sección de inventarios,<br>
            WHEN el artesano selecciona el botón de eliminar inventario,<br>
            THEN se elimina el inventario seleccionado.</td>
        <td>EP02</td>
    </tr>
    <tr>
        <td>US14</td>
        <td>Agregar materiales en inventario</td>
        <td>Como artesano usuario de la plataforma, quiero agregar materiales en mis inventarios para llevar un control detallado de los materiales disponibles.</td>
        <td>Scenario 1: Agregar materiales<br><br>
            GIVEN el artesano está en la vista de algún inventario,<br>
            WHEN el artesano selecciona el botón agregar material<br>
            THEN se agrega el material dentro del inventario.</td>
        <td>EP02</td>
    </tr>
    <tr>
        <td>US15</td>
        <td>Visualizar detalles de un material</td>
        <td>Como artesano usuario de la plataforma, quiero visualizar toda la información de un material para llevar un control detallado de tal material.</td>
        <td>Scenario 1: visualización de materiales<br><br>
            GIVEN el artesano está en la vista de algún inventario,<br>
            WHEN el artesano selecciona el botón revisar dentro de un inventario,<br>
            THEN se muestra toda la información de tal material</td>
        <td>EP05</td>
    </tr>
    <tr>
        <td>US16</td>
        <td>Búsqueda de Materiales en Inventario</td>
        <td>Como artesano usuario de la plataforma, quiero buscar materiales específicos dentro de mi inventario para localizarlos rápidamente y utilizarlos en mi proceso de producción.</td>
        <td>Scenario 1: Búsqueda por nombre<br><br>
            GIVEN el usuario se encuentra en la sección de Inventarios,<br>
           WHEN ingrese el nombre del material en la barra de búsqueda,<br>
            THEN el sistema mostrará los resultados correspondientes que coincidan con el nombre ingresado.<br><br>
            Scenario 2: Búsqueda por filtros<br><br>
            GIVEN el usuario se encuentra en la sección de Inventarios,<br>
            WHEN seleccione una categoría de materiales en el filtro de búsqueda,<br>
            THEN el sistema filtra los resultados y mostrará solo los materiales pertenecientes a esa categoría.</td>
        <td>EP02</td>
    </tr>
    <tr>
        <td>US17</td>
        <td>Visualización de la sección de foro</td>
        <td>Como artesano usuario de la plataforma, quiero una sección de foros para estar en contacto con otros artesanos.</td>
        <td>Scenario 1: Acceder a la sección de Foros.<br><br>
            GIVEN el artesano está en la barra de navegación,<br>
            WHEN el artesano ingrese a la sección "Foros",<br>
            THEN obtiene acceso a todos los foros disponibles.</td>
        <td>EP03</td>
    </tr>
    <tr>
        <td>US18</td>
        <td>Crear publicación</td>
        <td>Como artesano usuario de la plataforma, quiero crear publicaciones en el foro para compartir con otros usuarios.</td>
        <td>Scenario 1: Artesano crea una publicación satisfactoriamente.<br><br>
            GIVEN el artesano está en la sección de foro,<br>
            WHEN el artesano selecciona el botón de crear publicación, llena el formulario y presiona el botón publicar.<br>
            THEN se crea la publicación en el foro.</td>
        <td>EP03</td>
    </tr>
    <tr>
        <td>US19</td>
        <td>Editar publicación</td>
        <td>Como artesano usuario de la plataforma, quiero editar mis publicaciones en el foro para tener control total en estas.</td>
        <td>Scenario 1: Artesano edita una publicación satisfactoriamente.<br><br>
            GIVEN el artesano está en su publicación,<br>
            WHEN el artesano selecciona el botón de editar publicación, actualiza el formulario y presiona el botón editar<br>
            THEN se edita la publicación.</td>
        <td>EP03</td>
    </tr>
    <tr>
        <td>US20</td>
        <td>Eliminar publicación.</td>
        <td>Como artesano usuario de la plataforma, quiero eliminar mis publicaciones en el foro para mantener un orden en mi perfil.</td>
        <td>Scenario 1: Artesano elimina una publicación satisfactoriamente.<br><br>
            GIVEN el artesano está en su publicación,<br>
            WHEN el artesano selecciona el botón de eliminar publicación, se le aparecen dos botones y selecciona el botón aceptar.<br>
            THEN se elimina la publicación.<br><br>
            Scenario 2: Artesano cancela eliminar publicación.<br><br>
            GIVEN el artesano está en su publicación,<br>
            WHEN el artesano selecciona el botón de eliminar publicación, se le aparecen dos botones y selecciona el botón cancelar.<br>
            THEN la publicación no se elimina y el usuario regresa a la sección foro.</td>
        <td>EP06</td>
    </tr>
    <tr>
        <td>US21</td>
        <td>Comentar publicación</td>
        <td>Como artesano usuario de la plataforma, quiero comentar en las publicaciones del foro para contactarme con personas del mismo interés.</td>
        <td>Scenario 1: Artesano comenta satisfactoriamente una publicación<br><br>
           GIVEN el artesano está en la sección de foro,<br>
            WHEN el artesano selecciona el botón de agregar comentario en alguna publicación, llena el formulario y selecciona el botón comentar.<br>
            THEN se agrega el comentario en la publicación.</td>
        <td>EP03</td>
    </tr>
    <tr>
        <td>US22</td>
        <td>Visualización de los desarrolladores</td>
        <td>Como Artesano/Distribuidor visitante del Landing page de CraftSync, quiero una sección “Creadores” para informarme sobre los desarrolladores de la plataforma.</td>
        <td>Scenario: Visualización de una sección Creadores<br><br>
            GIVEN un Artesano/Distribuidor  visita la Landing Page,<br>
           WHEN baje hasta la sección de "Creadores"<br>
            OR presione el botón en la barra de navegación<br>
            THEN se le muestra información acerca de los desarrolladores de la plataforma.
        </td>
        <td>EP01</td>
    </tr>
    <tr>
        <td>US23</td>
        <td>Visualización de la sección Contact Us</td>
        <td>Como Artesano/Distribuidor visitante del Landing page de CraftSync, quiero una sección “Contact us” para solicitar información acerca de la plataforma</td>
        <td>Scenario: Visualización de una sección Contact us<br><br>
            GIVEN un Artesano/Distribuidor  visita la Landing Page,<br>
           WHEN baje hasta la sección "Contact us".<br>
            OR presione el botón en la barra de navegación<br>
            THEN se le muestra la opción de solicitar información.</td>
        <td>EP01</td>
    </tr>
    <tr>
        <td>US24</td>
        <td>Visualización de lista de tipos de suscripción</td>
        <td>Como Artesano/Distribuidor visitante del Landing page de CraftSync, quiero visitar la lista de tipos de suscripción para seleccionar alguno.</td>
        <td>Scenario: Visualización de una sección Contact us<br><br>
            GIVEN un Artesano/Distribuidor  visita la Landing Page,<br>
           WHEN baje hasta la sección de Suscripciones<br>
            OR presione el botón en la barra de navegación<br>
            THEN se le muestran las promociones que tiene el sitio web.</td>
        <td>EP01</td>
    </tr>
    <tr>
        <td>US25</td>
        <td>Visualización de los servicios disponibles</td>
        <td>Como Artesano/Distribuidor visitante del Landing page de CraftSync, quiero una sección “Services” para informarme sobre los servicios que ofrece la plataforma.</td>
        <td>Scenario: Visualización de una sección Contact us<br><br>
            GIVEN un Artesano/Distribuidor  visita la Landing Page,<br>
           WHEN baje hasta la sección de “Services”.<br>
            OR presione el botón en la barra de navegación<br>
            THEN se le muestra información detallada acerca de los servicios que ofrece la plataforma.</td>
        <td>EP01</td>
    </tr>
    <tr>
        <td>US26</td>
        <td>Manejo de Distribución de Pedidos</td>
        <td>Como Distribuidor, quiero un sistema de Distribución para manejar los pedidos disponibles.</td>
        <td>Scenario: Visualización de Pedidos a Distribuir<br><br>
            GIVEN un Distribuidor acepte un pedido,<br>
            AND el sistema lo procese,<br>
           WHEN accede a la sección de Distribución.<br>
            THEN se le muestra un sistema de organización de pedidos según Comprador.</td>
        <td>EP04</td>
    </tr>
    <tr>
        <td>US27</td>
        <td>Visualización de Pedidos</td>
        <td>Como Distribuidor, quiero un sistema de listado de Pedidos para organizar los Pedidos que tengo asignados con Artesano.</td>
        <td>Scenario: Visualización de Pedidos<br><br>
            GIVEN un Artesano solicite trabajo,<br>
            AND el Distribuidor le asigna un pedido,<br>
           WHEN accede a la sección de Pedidos.<br>
            THEN se le muestra una lista de todos los Pedidos asignados por el Distribuidor.</td>
        <td>EP04</td>
    </tr>
    <tr>
        <td>US28</td>
        <td>Generación de Pedidos</td>
        <td>Como Artesano, quiero generar un Pedido desde la plataforma para organizar pedidos no relacionados a Distribuidores.</td>
        <td>Scenario: Generación de Pedidos<br><br>
            GIVEN un Artesano está en la sección Pedidos,<br>
           WHEN presione el botón de Generar Pedido.<br>
            AND llene los datos,<br>
            THEN se le muestra el Pedido con opciones básicas de gestión.</td>
        <td>EP04</td>
    </tr>
    <tr>
        <td>US29</td>
        <td>Añadir artesanos mediante RESTful API</td>
        <td>Como Desarrollador, quiero añadir artesanos a la API, para conectarlos a las funciones de mi aplicación Web.</td>
        <td>Scenario 1: Añadir artesano con datos correctos<br><br>
            GIVEN el endpoint "api/v1/craftsmen" existe,<br>
           WHEN se envíe un request POST con los datos pertinentes.<br>
            AND no exista un artesano con el mismo nombre de usuario,<br>
            THEN se envía un response de estado 201.<br>
            AND un Recurso de Artesano con ID autogenerado y los datos correspondientes.<br><br>
            Scenario 2: Añadir artesano con datos existentes<br><br>
            GIVEN el endpoint "api/v1/craftsmen" existe,<br>
           WHEN se envíe un request POST con los datos pertinentes.<br>
            AND ya exista un artesano con el mismo nombre de usuario,<br>
            THEN se envía un response de estado 400<br>
            AND se muestra un mensaje de error indicando que ya existe ese nombre de usuario registrado.</td>
        <td>EP07</td>
    </tr>
    <tr>
        <td>US30</td>
        <td>Añadir distribuidores mediante RESTful API</td>
        <td>Como Desarrollador, quiero añadir distribuidores a la API, para conectarlos a las funciones de mi aplicación Web.</td>
        <td>Scenario 1: Añadir distribuidor con datos correctos<br><br>
            GIVEN el endpoint "api/v1/distributors" existe,<br>
           WHEN se envíe un request POST con los datos pertinentes.<br>
            AND no exista un artesano con el mismo nombre de usuario,<br>
            THEN se envía un response de estado 201.<br>
            AND un Recurso de Distribuidor con ID autogenerado y los datos correspondientes.<br><br>
            Scenario 2: Añadir distribuidor con datos existentes<br><br>
            GIVEN el endpoint "api/v1/craftsmen" existe,<br>
           WHEN se envíe un request POST con los datos pertinentes.<br>
            AND ya exista un artesano con el mismo nombre de usuario,<br>
            THEN se envía un response de estado 400<br>
            AND se muestra un mensaje de error indicando que ya existe ese nombre de usuario registrado.</td>
        <td>EP07</td>
    </tr>
    <tr>
       <td>US31</td>
        <td>Añadir pedidos mediante RESTful API</td>
        <td>Como Desarrollador, quiero añadir pedidos a la API, para conectarlos a las funciones de mi aplicación Web.</td>
        <td>Scenario 1: Añadir pedido<br><br>
            GIVEN el endpoint "api/v1/items" existe,<br>
           WHEN se envíe un request POST con los datos pertinentes.<br>
            THEN se envía un response de estado 201.<br>
            AND un Recurso de Pedido con ID autogenerado y los datos correspondientes.</td>
        <td>EP07</td>
    </tr>
    <tr>
        <td>US32</td>
        <td>Añadir inventarios mediante RESTful API</td>
        <td>Como Desarrollador, quiero añadir inventarios a la API, para conectarlos a las funciones de mi aplicación Web.</td>
        <td>Scenario 1: Añadir inventario con datos correctos<br><br>
            GIVEN el endpoint "api/v1/inventories" existe,<br>
           WHEN se envíe un request POST con los datos pertinentes.<br>
            AND no exista un inventario con el mismo nombre,<br>
            THEN se envía un response de estado 201.<br>
            AND un Recurso de Inventario con ID autogenerado y los datos correspondientes.<br><br>
            Scenario 2: Añadir inventario con datos existentes<br><br>
            GIVEN el endpoint "api/v1/inventories" existe,<br>
           WHEN se envíe un request POST con los datos pertinentes.<br>
            AND ya exista un inventario con el mismo nombre,<br>
            THEN se envía un response de estado 400<br>
            AND se muestra un mensaje de error indicando que ya existe ese nombre registrado.</td>
        <td>EP07</td>
    </tr>
    <tr>
        <td>US33</td>
        <td>Añadir materiales mediante RESTful API</td>
        <td>Como Desarrollador, quiero añadir materiales a la API, para conectarlos a las funciones de inventarios de mi aplicación Web.</td>
        <td>Scenario 1: Añadir material con datos correctos<br><br>
            GIVEN los endpoint "api/v1/inventories" y "api/v1/materials" existen,<br>
           WHEN se envíe un request POST con los datos pertinentes.<br>
            AND el inventario relacionado exista,<br>
            THEN se envía un response de estado 201.<br>
            AND un Recurso de Material con ID autogenerado y los datos correspondientes.<br><br>
            Scenario 2: Añadir material con datos incorrectos<br><br>
            GIVEN los endpoint "api/v1/inventories" y "api/v1/materials" existen,<br>
           WHEN se envíe un request POST con los datos pertinentes.<br>
            AND el inventario relacionado no exista,<br>
            THEN se envía un response de estado 400<br>
            AND se muestra un mensaje de error indicando que no existe el inventario al que se referencia.</td>
        <td>EP07</td>
    </tr>
    <tr>
        <td>US34</td>
        <td>Añadir publicaciones mediante RESTful API</td>
        <td>Como Desarrollador, quiero añadir inventarios a la API, para conectarlos a las funciones de foro de mi aplicación Web.</td>
        <td>Scenario 1: Añadir publicación<br><br>
            GIVEN el endpoint "api/v1/posts" existe,<br>
           WHEN se envíe un request POST con los datos pertinentes.<br>
            THEN se envía un response de estado 201.<br>
            AND un Recurso de Publicación con ID autogenerado y los datos correspondientes.</td>
        <td>EP07</td>
    </tr>
    <tr>
        <td>US35</td>
        <td>Añadir comentarios mediante RESTful API</td>
        <td>Como Desarrollador, quiero añadir comentarios a la API, para conectarlos a las funciones de publicaciones de mi aplicación Web.</td>
        <td>Scenario 1: Añadir comentario con datos correctos<br><br>
            GIVEN los endpoint "api/v1/posts" y "api/v1/comments" existen,<br>
           WHEN se envíe un request POST con los datos pertinentes.<br>
            AND la publicación relacionada exista,<br>
            THEN se envía un response de estado 201.<br>
            AND un Recurso de Comentario con ID autogenerado y los datos correspondientes.<br><br>
            Scenario 2: Añadir comentario con datos incorrectos<br><br>
            GIVEN los endpoint "api/v1/posts" y "api/v1/comments" existen,<br>
           WHEN se envíe un request POST con los datos pertinentes.<br>
            AND la publicación relacionada no exista,<br>
            THEN se envía un response de estado 400<br>
            AND se muestra un mensaje de error indicando que no existe la publicación al que se referencia.</td>
        <td>EP07</td>
    </tr>
</table>

## 3.3. Impact Mapping

En esta sección, se plantearon metas de negocio utilizando los criterios SMART para elaborar el Impact Mapping en base a nuestras User Personas y User Stories.

Segmento 1:

![Segmento1](/assets/img/Segemento1.png)

Segmento 2:

![Segmento2](/assets/img/Segemento2.png)

## 3.4. Product Backlog

<table>
    <tr>
        <th>Orden</th>
        <th>User Story Id</th>
        <th>Título</th>
        <th>Descripción</th>
        <th>Story Points (1 / 2 / 3 / 5 / 8)</th>
    </tr>
    <tr>
        <td>1</td>
        <td>US01</td>
        <td>Sección About Us</td>
        <td>Yo, como distribuidor visitante del Landing Page, quiero una sección About Us para informarme sobre la empresa y sus detalles.</td>
        <td>1</td>
    </tr>
    <tr>
        <td>2</td>
        <td>US25</td>
        <td>Visualización de los servicios disponibles</td>
        <td>Como Artesano/Distribuidor visitante del Landing page de CraftSync, quiero una sección “Services” para informarme sobre los servicios que ofrece la plataforma.</td>
        <td>1</td>
    </tr>
    <tr>
        <td>3</td>
        <td>US24</td>
        <td>Visualización de lista de tipos de suscripción</td>
        <td>Como Artesano/Distribuidor visitante del Landing page de CraftSync, quiero visitar la lista de tipos de suscripción para seleccionar alguno.</td>
        <td>1</td>
    </tr>
    <tr>
        <td>4</td>
        <td>US23</td>
        <td>Visualización de la sección Contact Us</td>
        <td>Como Artesano/Distribuidor visitante del Landing page de CraftSync, quiero una sección “Contact us” para solicitar información acerca de la plataforma</td>
        <td>1</td>
    </tr>
    <tr>
        <td>5</td>
        <td>US22</td>
        <td>Visualización de los desarrolladores</td>
        <td>Como Artesano/Distribuidor visitante del Landing page de CraftSync, quiero una sección “Creadores” para informarme sobre los desarrolladores de la plataforma.</td>
        <td>1</td>
    </tr>
     <tr>
        <td>6</td>
        <td>US02</td>
        <td>Selector de Idioma</td>
        <td>Yo, como distribuidor visitante del Landing Page, quiero un selector de idioma para leer el contenido en mi idioma de preferencia.</td>
        <td>1</td>
    </tr>
    <tr>
        <td>7</td>
        <td>US27</td>
        <td>Visualización de Pedidos.</td>
        <td>Como Distribuidor, quiero un sistema de listado de Pedidos para organizar los Pedidos que tengo asignados con Artesano.</td>
        <td>3</td>
    </tr>
    <tr>
        <td>8</td>
        <td>US05</td>
        <td>Actualizar Progreso</td>
        <td>Yo, como usuario artesano de la plataforma, quiero actualizar los detalles del pedido, para mantener informado al distribuidor.</td>
        <td>2</td>
    </tr>
    <tr>
        <td>9</td>
        <td>US11</td>
        <td>Visualización de la sección de inventarios</td>
        <td>Como artesano usuario de la plataforma, quiero ver mis inventarios de trabajo para estar al tanto de lo que se tiene disponible.</td>
        <td>2</td>
    </tr>
    <tr>
        <td>10</td>
        <td>US12</td>
        <td>Crear inventario</td>
        <td>Como artesano usuario de la plataforma, quiero agregar inventarios para mantener un orden en mis diferentes proyectos.</td>
        <td>2</td>
    </tr>
    <tr>
        <td>11</td>
        <td>US17</td>
        <td>Visualización de la sección de foro</td>
        <td>Como artesano usuario de la plataforma, quiero una sección de foros para estar en contacto con otros artesanos.</td>
        <td>5</td>
    </tr>
    <tr>
        <td>12</td>
        <td>US18</td>
        <td>Crear publicación</td>
        <td>Como artesano usuario de la plataforma, quiero crear publicaciones en el foro para compartir con otros usuarios.</td>
        <td>2</td>
    </tr>
    <tr>
        <td>13</td>
        <td>US06</td>
        <td>Visualización de perfil de usuario propio.</td>
        <td>Como Artesano/Distribuidor usuario de la plataforma, quiero visualizar mi perfil para verificar que mi información es correcta.</td>
        <td>2</td>
    </tr>
    <tr>
        <td>14</td>
        <td>US26</td>
        <td>Manejo de Distribución de Pedidos</td>
        <td>Como Distribuidor, quiero un sistema de Distribución para manejar los pedidos disponibles.</td>
        <td>5</td>
    </tr>
    <tr>
        <td>15</td>
        <td>US28</td>
        <td>Generación de Pedidos</td>
        <td>Como Artesano, quiero generar un Pedido desde la plataforma para organizar pedidos no relacionados a Distribuidores.</td>
        <td>3</td>
    </tr>
    <tr>
        <td>16</td>
        <td>US04</td>
        <td>Asignar Pedidos</td>
        <td>Yo, como usuario distribuidor de la plataforma, quiero asignar pedidos a los artesanos, para enviarlos a los compradores una vez hechos.</td>
        <td>2</td>
    </tr>
    <tr>
        <td>17</td>
        <td>US14</td>
        <td>Agregar materiales en inventario</td>
        <td>Como artesano usuario de la plataforma, quiero agregar materiales en mis inventarios para llevar un control detallado de los materiales disponibles.</td>
        <td>2</td>
    </tr>
    <tr>
        <td>18</td>
        <td>US03</td>
        <td>Solicitud de Trabajo</td>
        <td>Yo, como artesano usuario de la plataforma, quiero mandar solicitudes a los distribuidores, para obtener pedidos de su parte.</td>
        <td>2</td>
    </tr>
    <tr>
        <td>19</td>
        <td>US07</td>
        <td>Visualización de otros perfiles de usuario</td>
        <td>Como Artesano/Distribuidor usuario de la plataforma, quiero visualizar otros perfiles de usuario para ver su información e interactuar.</td>
        <td>2</td>
    </tr>
    <tr>
        <td>20</td>
        <td>US15</td>
        <td>Visualizar detalles de un material</td>
        <td>Como artesano usuario de la plataforma, quiero visualizar toda la información de un material para llevar un control detallado de tal material.</td>
        <td>2</td>
    </tr>
    <tr>
        <td>21</td>
        <td>US13</td>
        <td>Eliminar inventario</td>
        <td>Como artesano usuario de la plataforma, quiero eliminar inventarios para no tener información innecesaria</td>
        <td>2</td>
    </tr>
    <tr>
        <td>22</td>
        <td>US16</td>
        <td>Búsqueda de Materiales en Inventario</td>
        <td>Como artesano usuario de la plataforma, quiero buscar materiales específicos dentro de mi inventario para localizarlos rápidamente y utilizarlos en mi proceso de producción.</td>
        <td>3</td>
    </tr>
    <tr>
        <td>23</td>
        <td>US21</td>
        <td>Comentar publicación</td>
        <td>Como artesano usuario de la plataforma, quiero comentar en las publicaciones del foro para contactarme con personas del mismo interés.</td>
        <td>3</td>
    </tr>
    <tr>
        <td>24</td>
        <td>US20</td>
        <td>Eliminar publicación.</td>
        <td>Como artesano usuario de la plataforma, quiero eliminar mis publicaciones en el foro para mantener un orden en mi perfil.</td>
        <td>2</td>
    </tr>
    <tr>
        <td>25</td>
        <td>US19</td>
        <td>Editar publicación	</td>
        <td>Como artesano usuario de la plataforma, quiero editar mis publicaciones en el foro para tener control total en estas.	</td>
        <td>2</td>
    </tr>
    <tr>
        <td>26</td>
        <td>US08</td>
        <td>Actualización de información de perfil.</td>
        <td>Como Artesano/Distribuidor usuario de la plataforma, quiero poder actualizar mi información personal y de contacto para mantener mis datos actualizados.</td>
        <td>2</td>
    </tr>
    <tr>
        <td>27</td>
        <td>US29</td>
        <td>Añadir artesanos mediante RESTful API</td>
        <td>Como Desarrollador, quiero añadir artesanos a la API, para conectarlos a las funciones de mi aplicación Web.</td>
        <td>3</td>
    </tr>
    <tr>
        <td>28</td>
        <td>US30</td>
        <td>Añadir distribuidores mediante RESTful API</td>
        <td>Como Desarrollador, quiero añadir distribuidores a la API, para conectarlos a las funciones de mi aplicación Web.</td>
        <td>3</td>
    </tr>
    <tr>
        <td>29</td>
        <td>US31</td>
        <td>Añadir pedidos mediante RESTful API</td>
        <td>Como Desarrollador, quiero añadir pedidos a la API, para conectarlos a las funciones de mi aplicación Web.</td>
        <td>3</td>
    </tr>
    <tr>
        <td>30</td>
        <td>US32</td>
        <td>Añadir inventarios mediante RESTful API</td>
        <td>Como Desarrollador, quiero añadir inventarios a la API, para conectarlos a las funciones de mi aplicación Web.</td>
        <td>3</td>
    </tr>
    <tr>
        <td>31</td>
        <td>US33</td>
        <td>Añadir materiales mediante RESTful API</td>
        <td>Como Desarrollador, quiero añadir materiales a la API, para conectarlos a las funciones de inventario de mi aplicación Web.</td>
        <td>3</td>
    </tr>
    <tr>
        <td>32</td>
        <td>US34</td>
        <td>Añadir publicaciones mediante RESTful API</td>
        <td>Como Desarrollador, quiero añadir publicaciones a la API, para conectarlos a las funciones de foro de mi aplicación Web.</td>
        <td>3</td>
    </tr>
    <tr>
        <td>33</td>
        <td>US35</td>
        <td>Añadir comentarios mediante RESTful API</td>
        <td>Como Desarrollador, quiero añadir comentarios a la API, para conectarlos a las funciones de publicaciones de mi aplicación Web.</td>
        <td>3</td>
    </tr>
    <tr>
        <td>34</td>
        <td>US10</td>
        <td>Cerrar sesión</td>
        <td>Como Artesano/Distribuidor usuario de la plataforma, quiero cerrar sesión para proteger la integridad de mi cuenta.</td>
        <td>1</td>
    </tr>
    <tr>
        <td>35</td>
        <td>US09</td>
        <td>Borrar cuenta</td>
        <td>Como Artesano/Distribuidor usuario de la plataforma, quiero borrar mi cuenta para proteger la integridad de mi persona.</td>
        <td>1</td>
    </tr>
</table>

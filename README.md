# Integrantes

- Caceres Gonzales, Alonso
- Espinoza Carrión, Edgar F.
- Nuñez, Alessandra
- Leite, Josue

# Primer avance
## 1. Caso de Negocio
### 1. 1. Generalidades 

**Nombre de la Startup:** ExpertConnect  

**Situación de la startup:** ExpertConnect es una plataforma en línea diseñada para abordar la creciente demanda de acceso a expertos y asesoramiento especializado en una variedad de campos. La plataforma surge en un mundo cada vez más conectado y digitalizado, donde las personas buscan respuestas y orientación de expertos en diversas áreas sin la necesidad de desplazarse físicamente a una ubicación específica. Esta plataforma se enfoca en conectar a personas que necesitan asesoramiento con expertos en una amplia gama de disciplinas.  

**Estructura de la solución:**  
- Módulo de registro e inicio de sesión: Los usuarios podrán registrarse e iniciar sesión en la plataforma. Estos usuarios pueden tener dos roles: 'aprendices', quienes solicitan el servicio de asesoría, y 'mentores', profesionales que brindan estos servicios. 
- Módulo de búsqueda de profesionales: Los 'aprendices' pueden explorar perfiles de los 'mentores', ver sus calificaciones, reseñas y áreas de especialización. Pueden buscar expertos por categoría o palabras clave.  
- Módulo de gestión de citas: Los 'aprendices' pueden ver la disponibilidad de los 'mentores' y solicitar una reunión. Esta funcionalidad tendrá la opción para que el usuario añada la cita a su calendario de Google o Microsoft.
- Módulo de sala de asesorías: La plataforma ofrece una solución de videollamada integrada y segura para las sesiones entre usuarios.
- Módulo de gestión de documentos y grabaciones: Tanto 'aprendices' como 'mentores' pueden compartir documentos entre sí y subir sus documentos a una carpeta propia almacenada en la nube. Junto a estos documentos, los 'aprendices' también pueden almacenar en la nube grabaciones de las asesorías bajo un costo extra.
- Módulo de chat en tiempo real: La plataforma ofrece la opción de mensajería instantánea entre 'aprendices' y 'mentores', así como soporte en tiempo real a través de un chat con un especialista.
- Módulo de pagos: Los pagos se realizan de manera segura a través de la plataforma, y ExpertConnect retiene una comisión por cada sesión de asesoramiento.

**Mercado de la startup**
- Profesionales Independientes: Freelancers y autónomos que pueden requerir asesoramiento en aspectos legales, fiscales, de marketing, tecnología, etc.
- Emprendedores: Personas que están lanzando sus propios negocios y necesitan orientación en estrategia empresarial, financiación, desarrollo de productos, etc.
- Estudiantes: Estudiantes universitarios que buscan asesoramiento académico y profesional de expertos en su campo de estudio.
- Empresas Pequeñas y Medianas: Empresas en crecimiento que necesitan asesoramiento en áreas específicas como gestión de recursos humanos, estrategia de negocios, marketing digital, etc.
- Personas en Búsqueda de Empleo: Individuos en busca de consejos de carrera y orientación profesional para mejorar sus oportunidades laborales.

### 1.2. Modelo de Negocio (canvas)
![modelo del negocio](https://github.com/DarkShadow76/ArquiSoft-Grupo1/blob/master/canvasv1.png)

### 1.3. Estructura del equipo
![estructura del equipo](https://github.com/DarkShadow76/ArquiSoft-Grupo1/blob/master/Estructura%20del%20equipo.png)

### 1.4. Listado de stakeholders

| Rol  | Encargado | Descripción |
| --- | --- | ------ |
| Cliente  | Usuarios | Para este proyecto, los clientes interesados son los usuarios finales (profesionales y clientes que pagan por el servicio de asesoría). |
| Gestor del negocio  |  | Asegura que la arquitectura del proyecto se alinee con las metas de la empresa. |
| Arquitecto de software  |  | Define la arquitectura y se asegura que se cumplan los requerimientos establecidos. |
| Diseñador  |  | Responsable de aplicar la arquitectura del proyecto en referencia a los requerimientos centrados para el mismo. |
| Implementador e integrador  |  | Desarrolla e integra diferentes elementos y componentes en función del diseño de requerimientos y arquitectura. |
| Responsable de mantenimiento  |  | Asegura el funcionamiento correcto del proyecto, solucionando cualquier problema que se presente a lo largo de su vida. |
| Analista  |  | Asegura que el sistema cumpla con los requerimientos de calidad y que se ajuste a lo que espera el cliente y el negocio. |

## Requerimientos del sistema
### Requerimientos funcionales
1. Módulo de registro e inicio de sesión  
    - **RF1. Registro de Usuarios:** La plataforma debe permitir que dos tipos de usuarios, clientes y profesionales, se registren proporcionando información personal, de contacto y detalles de su profesión al crear sus cuentas. Además, los profesionales deben poder listar sus servicios en la plataforma, incluyendo descripciones detalladas, tarifas y disponibilidad para que los clientes puedan acceder a esta información al buscar servicios.  
    - **RF2. Inicio de sesión:** Tanto los usuarios como los profesionales deben tener la capacidad de iniciar sesión en sus cuentas utilizando su correo y contraseña.
    - **RF12. Registro de Usuarios:** El sistema debe enviar un correo electrónico de confirmación al usuario tras la creación de una cuenta.
    - **RF13. Registro de Usuarios:** El sistema   que el email no esté siendo utilizado en otra cuenta ya ingresada en el sistema, pues solo se permite una cuenta por usuario.
2. Módulo de búsqueda de profesionales  
    - **RF3. Búsqueda de Profesionales:** Los usuarios deben tener la posibilidad de buscar profesionales según categorías, ubicación, calificaciones y otros criterios relevantes.
    - **RF9. Calificaciones y Reseñas:** Los usuarios deben poder calificar y dejar reseñas sobre los profesionales y los servicios ofrecidos, permitiendo que los profesionales respondan a estas reseñas.
3. Módulo de gestión de citas  
    - **RF5. Sistema de Reserva de Citas:** Los usuarios deben poder programar citas con profesionales según la disponibilidad de estos, recibiendo confirmaciones por correo electrónico o mensajes de texto.  
    - **RF6. Gestión de Citas:** Los usuarios y profesionales deben poder ver y administrar sus citas programadas, con la opción de cancelar o reprogramar citas cuando sea necesario.  
    - **RF10. Sistema de Notificaciones:** Los usuarios deben recibir notificaciones sobre citas programadas, mensajes nuevos y otros eventos relevantes dentro de la plataforma.  
4. Módulo de creación de sala de conferencias  
    - **RF7. Videoconferencias:** La plataforma debe incluir una función de videoconferencia integrada para las asesorías programadas, permitiendo que usuarios y profesionales se conecten en el horario acordado.  
    - **RF11. Videoconferencias:** La plataforma debe permitir el acceso de invitados a traves de un enlace generado por el mentor. se les pedira que ingresen su nombre y tendran que ser aprobados por el mentor. 
        ![VideoConferencia](https://github.com/DarkShadow76/ArquiSoft-Grupo1/blob/master/Wireframes/Modulo%20de%20Creacion%20de%20sala%20de%20videoconferencias/Video%20-%20Reservar%20Asesoria.png)
    - Historial de Reuniones
        ![Historico de Reuniones](https://github.com/DarkShadow76/ArquiSoft-Grupo1/blob/master/Wireframes/Modulo%20de%20Creacion%20de%20sala%20de%20videoconferencias/Video%20-%20Historico%20de%20reuniones.png)

5. Módulo de gestión de documentos y grabaciones  
        ![mis archivos](https://github.com/DarkShadow76/ArquiSoft-Grupo1/blob/master/Wireframes/Módulo%20de%20archivos/imagen_2023-09-20_212831592.png)
    - **Subida de archivos:** Los usuarios deben poder subir archivos en cualquier formato a su carpeta de Archivos. El límite de almacenamiento gratuito por usuario será de 1GB.
    - **Opción de fingerprinting (firma digital):** Para cada archivo a subir, deberá haber una opción de fingerprinting como garantía de la integridad y autenticidad.
        ![subida archivos](https://github.com/DarkShadow76/ArquiSoft-Grupo1/blob/master/Wireframes/Módulo%20de%20archivos/imagen_2023-09-20_213043086.png)
    - **Lectura de archivos:** Los usuarios deben poder abrir y leer en línea archivos en los formatos .pptx, .xlsx, .docx y .txt.
        ![lectura archivos](https://github.com/DarkShadow76/ArquiSoft-Grupo1/blob/master/Wireframes/Módulo%20de%20archivos/imagen_2023-09-20_213104763.png)
    - **Grabaciones en la nube:** Si el usuario realizó el pago para que la asesoría sea almacenada en la nube, esta se almacenará en una nueva sección en la carpeta de Archivos del usuario.
    - **Gestión de archivos:** Tanto para archivos subidos por el usuario como las grabaciones de las asesorías, los usuarios podrán copiar, pegar, mover entre carpetas, eliminar y crear enlaces para compartir estos archivos o grabaciones.
        ![gestion archivos](https://github.com/DarkShadow76/ArquiSoft-Grupo1/blob/master/Wireframes/Módulo%20de%20archivos/imagen_2023-09-20_213004043.png)
6. Módulo de pagos  
    - **RF4. Carrito de Compras y Pago Integrado:** Los usuarios deben poder agregar servicios al carrito de compras y realizar pagos seguros en línea para reservar citas o adquirir servicios.
    - **RF14. Pasarela de Pago:** El módulo debe permitir a los usuarios realizar pagos con tarjetas de crédito, débito y PayPal principalmente.
    - **RF15. Confirmación de Pago:** El sistema debe enviar un mensaje el cual recompila la información del pago realizado por el aprendiz, especificando el monto pagado y algunas cualidades de la reunión.

7. Módulo de chat en tiempo real  
    - **RF8. Chat en Tiempo Real:** Debe existir la capacidad de comunicación en tiempo real a través de chat para que los usuarios y profesionales puedan interactuar antes y después de programar una cita, con notificaciones para mensajes nuevos.  
  
### Escenarios de atributos de calidad
ID | Atributo | Fuente | Estímulo | Artefacto | Entorno | Respuesta | Medida
--- | --- | --- |--- |--- |--- | --- | ---
ESC-01 | Disponibilidad | Usuario | El usuario busca visualizar el listado de profesionales activos en el sistema | Módulo de búsqueda de profesionales | Operacion bajo los estandares de normalidad | El modulo de busqueda de profesionales recuperara el listado de profesionales presentes | La búsqueda de profesionales se completa en 2 segundos o menos.
ESC-02 | Disponibilidad | Usuario | El usuario busca realizar una transaccion bancaria a travez del sistema integrado en la aplicacion | Módulo de pagos | Operacion bajo los estandares de normalidad | El modulo de pagos realizara la transaccion, dependiendo del funcionamiento actual del sistema integrado de pagos | El tiempo de respuesta del modulo de pagos es de 8 segundos o menos.
ESC-03 | Mantenibilidad | Equipo de desarrollo | Necesidad de mejorar la funcionalidad del sistema de notificaciones en tiempo real | Módulo de notificaciones | Entorno de desarrollo de la plataforma, repositorio de código | La actualización se completa sin afectar otras áreas funcionales de la plataforma | La cantidad de bugs introducidos en los otros módulos es 0
ESC-04 | Mantenibilidad | Fallo crítico  | Usuarios detectan un error en la función de programación de citas | Código fuente de la plataforma | Producción en vivo de la plataforma | El equipo de desarrollo aisla el módulo fallido y resuelve el fallo crítico en la plataforma | La plataforma se restaura en menos de 1 hora
ESC-05 | Rendimiento | Usuarios | Multiples usuarios dan uso al sistema de busqueda de profesionales al mismo tiempo | Módulo de búsqueda de profesionales, servidores de la plataforma | Conexión a Internet estable en todos los usuarios | El sistema de busqueda de profesionales busca resolver cada transaccion de datos con normalidad y se mantiene | Tiempo de procesamiento de 2 segundos.
ESC-06 | Seguridad | Usuario | El usuario busca ingresar a una cuenta, pero falla el sistema de verificacion de identificacion base 3 veces seguidas | Módulo de registro e inicio de sesión | Operacion bajo los estandares de normalidad | El sistema deniega los siguientes intentos de ingreso por parte de ese usuario y se informa al titular de la cuenta de un posible intento de ingreso no legitimo | El sistema bloquea temporalmente el acceso a la cuenta y registra el incidente.
ESC-07 | Seguridad | Usuarios | El usuario sube documentos que contienen información personal y confidencial. | Módulo de almacenamiento de archivos | Conexión a Internet estable, navegador web actualizado. | La plataforma cifra y almacena los documentos de forma segura. | Los documentos solo son accesibles para el usuario.
ESC-08 | Usabilidad | Usuarios | El usuario abre la plataforma desde Colibri Web Browser | Plataforma ExpertConnect | Conexión a Internet estable, navegador basado en Chromium | La plataforma se carga correctamente en el navegador al tener soporte para Chromium | La plataforma es funcional y presenta una interfaz de usuario coherente en el navegador
ESC-09 | Rendimiento | Mentor y aprendices invitados | El mentor inicia una conferencia y se unen cientos de invitados al mismo tiempo | Módulo de videoconferencias de la plataforma, servidores de la plataforma | Conexiones a Internet variadas de los usuarios | Los participantes pueden unirse a la conferencia sin problemas y disfrutan de una experiencia de video y audio fluida | Los recursos del servidor no excedan el 80% de su capacidad máxima
### Restricciones 
- La aplicación se basará en un entorno web únicamente.
- El sistema se desarrollará con un único lenguaje de programación en mente, el cual será JavaScript.
- La plataforma deberá ser completada a mediados de diciembre y se deben realizar el desarrollo, las pruebas y el envío a producción.


## Decisiones a Nivel de Arquitectura

### Asignación de Responsabilidades
- **Módulo de registro e inicio de sesión:** Módulo responsable del registro y autentificación de los usuarios.
- **Módulo de búsqueda de profesionales:** Módulo responsable de presentar a los usuarios profesionales en la plataforma, permitiendo la búsqueda entre estos.
- **Módulo de gestión de citas:** Módulo responsable en la coordinación y preparación de las citas con los profesionales.
- **Módulo de creación de sala de conferencias:** Módulo responsable de la creación de las conferencias, al igual que el aseguramiento de su seguridad.
- **Módulo de gestión de documentos y grabaciones:** Módulo encargado del almacenamiento de datos relacionados con las conferencias, asegurando su disponibilidad e integridad.
- **Módulo de pagos:** Módulo encargado de la pasarela de pagos y las implementaciones relacionadas.
- **Módulo de chat en tiempo real:** Módulo encargado de permitir una comunicación directa entre el profesional y el usuario antes de la cita programada.

### Modelo de Coordinación
El proyecto implementará conexiones asíncronas y síncronas para su correcto funcionamiento.

- **Comunicación síncrona:** Será implementada para el módulo de chat en tiempo real, el módulo de videollamadas y finalmente el módulo de registro y autentificación.
- **Comunicación asíncrona:** Será implementada para el módulo de pagos, el módulo de almacenamiento de grabaciones y archivos y el módulo de gestión de citas.

### Modelo de Datos
- **Base de datos relacional:** El modelo de datos relacional se utilizará para almacenar información personal y de contacto de los mentores y de los aprendices. Asimismo, se usará para almacenar información del módulo de gestión de citas. 

- **Base de datos no relacional:** El modelo de datos no relacional se utilizará principalmente para almacenar las grabaciones de las videollamadas o videoconferencias y los documentos que suban los usuarios a su unidad. También se empleará este modelo de datos para la mensajería instantánea que tiene el módulo de chat en tiempo real, ya que en este chat se podrán enviar fotos y documentos, aparte de texto. 

### Mapeo entre Elementos de Arquitectura
- Diagrama de Contexto

- Diagrama de contenedores
 
### Elección de Tecnología
- **Frontend:** Angular y Angular Material para la interfaz de usuario. Se eligió esta opción pues en Angular se han construido bastantes aplicaciones web robustas y dinámicas. 
- **Backend:** Node.js es una opción sólida para construir aplicaciones en tiempo real (videollamadas y mensajería) y escalables. Se usará Express.js para simplificar el desarrollo. 
- **Bases de datos:** MongoDB como opción para almacenar datos no estructurados y PostgreSQL para los datos estructurados de los usuarios y sus citas.
- **Pasarela de pagos:** Al ser una iniciativa que apunta al mercado internacional, se usarán las pasarelas de pagos Stripe y PayPal.
- **Almacenamiento en la nube:** Se usará Amazon S3 para almacenar archivos y videos.
- **Videollamadas:** Se usará el servicio de Agora.io para las videollamadas y videoconferencias, al ser mejor que su competidor Twilio.
- **Escalabilidad y despliegue:** Se desplegará en AWS.

## Tácticas 

### Disponibilidad 
La disponibilidad es sumamente importante considerando que la plataforma brinda un servicio de videoconferencias de manera síncrona. Este servicio puede coordinarse para darse a cualquier hora, desde cualquier parte del mundo, lo que debe estar activo la mayor parte del tiempo posible. 

Se esperan que las medidas de respuesta sean las siguientes:
- Tiempo de disponibilidad del sistema: 99.9% (Inactivo 8.76h en el año)
- Tiempo para detectar la falla: Entre 10 a 25 minutos como máximo
- Tiempo para recuperarse de la falla: Entre 30 minutos a 1.5 horas como máximo.

**Tácticas a emplear:**
- **Tiempo de espera:** Delimitaciones de los tiempos de esperas, indicando una posible falla al detectar una falla en los tiempos de carga y levantando una excepción.
- **Rollback:** Una versión del estado anterior, la cual puede ser utilizada para recuperar el sistema en caso de una falla total. Es de alta importancia poner un enfoque en actualizar esta versión constantemente.
- **Remover de servicio:** En caso de un problema mayor se deberá de remover el servicio por el tiempo presente hasta que el problema se vea solucionado para evitar un empeoramiento del mismo.

### Mantenibilidad
En cuanto a la facilidad de mantener el sistema en buen funcionamiento, es esencial que cualquier modificación o mejora se pueda abordar de manera eficaz y sin dificultades. La capacidad de mantenimiento contribuye a un proceso de desarrollo más fluido y a una reducción en el tiempo necesario para implementar nuevas actualizaciones.
**Tácticas a emplear:**
- **Modularidad:** Se dividirá la aplicación en módulos lo más independiente posible con el fin de facilitar el desarrollo en uno de ellos sin que termine afectando a los demás. Ejm: módulo usuario, módulo videoconferencia, módulo documentos, etc.
- **Disminución de acoplamiento:** Se mantendrán las interdependencias de los módulos al mínimo con técnicas de encapsulamiento y refactoring.

### Interoperabilidad
La interoperabilidad se refiere a la capacidad de sistemas, aplicaciones o componentes de software para comunicarse, interactuar y funcionar de manera efectiva y armoniosa entre sí, incluso si han sido desarrollados por diferentes proveedores o en distintas plataformas. Es un concepto esencial en el mundo de la tecnología de la información y las comunicaciones, ya que permite que sistemas heterogéneos colaboren y compartan datos de manera eficiente.
**Tácticas a emplear:**
- **Servicios Web y API RESTful:** Diseñar interfaces de programación de aplicaciones (API) basadas en REST para permitir la comunicación entre sistemas de manera sencilla.
- **Middleware de Integración:** Implementar middleware o capas de integración que faciliten la comunicación y la transferencia de datos entre sistemas heterogéneos.
- **Estandarización de Protocolos y Formatos de Datos:** Utilizar formatos de datos comunes y legibles por humanos para facilitar la comunicación entre sistemas.
- **Uso de Contenedores y Orquestación de Contenedores:** Utilizar contenedores (como Docker) y orquestadores (como Kubernetes) para crear entornos portátiles y escalables que faciliten la interoperabilidad.

### Rendimiento
El rendimiento conlleva el enfoque en la capacidad del sistema en poder manejar y cumplir la carga de trabajo esperada, respondiendo de manera oportuna y manteniendo una estabilidad al hacerlo.

Se esperan que las métricas dé respuesta sean las siguientes:
Máximo de 5 segundos de demora cada transacción.

**Tácticas a emplear:**
- **Diseño modular:** Subdividir el sistema en módulos de menor tamaño creados de manera independiente, lo cual de igual manera permite una optimización independiente de cada módulo.
- **Introducir concurrencia:** Presentar la capacidad de manejar múltiples solicitudes en paralelo, posiblemente reduciendo tiempos de inactividad o bloque en el sistema. 
- **Aumentar recursos:** Incrementar la capacidad de procesamiento de los sistemas al observar un incremento en los usuarios o los servicios presentados.

### Seguridad
La seguridad es un aspecto crítico en cualquier proyecto de desarrollo de software. La falta de medidas de seguridad adecuadas puede exponer sistemas y datos a amenazas como ataques cibernéticos, robo de información, interrupciones del servicio y otros riesgos. A continuación, información sobre las tácticas clave para garantizar la seguridad en el presente proyecto de desarrollo de software:

**Tácticas a emplear:**
- **Autenticación y Autorización:** Implementa un sólido sistema de autenticación para verificar la identidad de los usuarios. Utiliza mecanismos de autorización para controlar el acceso a las funciones y los datos según los roles y permisos de cada usuario.
- **Cifrado de Datos:** Utiliza técnicas de cifrado para proteger la confidencialidad de los datos en reposo y en tránsito. El cifrado de extremo a extremo es especialmente importante al trabajar con información sensible.
- **Pruebas de Seguridad:** Realiza pruebas de seguridad regulares, como pruebas de penetración y evaluaciones de seguridad, para identificar y corregir vulnerabilidades en tu aplicación.
- **Políticas y Normativas de Seguridad:** Cumple con las políticas y regulaciones de seguridad aplicables a tu industria. Esto puede incluir estándares como el Reglamento General de Protección de Datos (RGPD), HIPAA o PCI DSS.
- **Seguridad en la Infraestructura:** Asegúrate de que la infraestructura en la que se ejecuta tu software (servidores, redes, almacenamiento) también esté protegida adecuadamente.

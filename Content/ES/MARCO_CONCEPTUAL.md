## 4.2 MARCO CONCEPTUAL

### 4.2.1  Arquitectura de Software.

La arquitectura de software es el proceso de definición de una solución estructurada que usa un conjunto de patrones para que dicha solución cumpla con todos los requisitos técnicos y operativos, al tiempo que optimiza los atributos de calidad comunes, como el rendimiento, la seguridad y la capacidad de gestión. También implica una serie de decisiones basadas en una amplia gama de factores, y cada una de estas decisiones puede tener un impacto considerable en la calidad, el rendimiento, la facilidad de mantenimiento y el éxito general de la  aplicación \[1\].

Philippe Kruchten, Grady Booch, Kurt Bittner y Rich Reitman derivaron y perfeccionaron una definición de arquitectura basada en el trabajo de Mary Shaw y David Garlan \(Shaw y Garlan 1996\). Su definición es:

"La arquitectura de software abarca el conjunto de decisiones importantes sobre la organización de un sistema de software que incluye la selección de los elementos estructurales y sus interfaces de las que se compone el sistema; Comportamiento especificado en la colaboración entre esos elementos; Composición de estos elementos estructurales y de comportamiento en subsistemas más grandes; Y un estilo arquitectónico que guía a esta organización. La arquitectura del software también implica funcionalidad, usabilidad, resistencia, rendimiento, reutilización, comprensibilidad, limitaciones económicas y tecnológicas, compromisos y preocupaciones estéticas ".

¿Por qué es importante la arquitectura de software? Al igual que en la creacion de cualquier otra estructura compleja, el software debe construirse sobre bases solidas.

Figura 1: Usuario, negocio y sistema como objetivos.

Se debe encontrar un equilibrio entre los requisitos a través de estas tres áreas. Por ejemplo, la experiencia general del usuario es a menudo una función del negocio y la infraestructura de TI, y los cambios en uno u otro pueden afectar significativamente la experiencia del usuario final. Del mismo modo, los cambios en los requisitos de la experiencia del usuario pueden tener un impacto significativo en los requisitos de negocio y de infraestructura de TI. El rendimiento puede ser un objetivo importante para el usuario y el negocio, pero es posible que el administrador del sistema no pueda invertir en el hardware necesario para cumplir esa meta el 100 por ciento del tiempo. Un punto de equilibrio podría ser alcanzar el objetivo sólo el 80 por ciento del tiempo.

Una lista de preocupaciones de alto nivel al pensar en la arquitectura del software podría ser:

* ¿Cómo utilizarán los usuarios la aplicación?

* ¿Cómo se desplegará la aplicación en producción y se administrará?

* ¿Cuáles son los requisitos de atributos de calidad para la aplicación, como seguridad, rendimiento, concurrencia, internacionalización y configuración?

* ¿Cómo se puede diseñar la aplicación para que sea flexible y mantenible con el tiempo?

* ¿Cuáles son las tendencias arquitectónicas que podrían afectar su aplicación ahora o después de que se ha implementado?


Para utilizar o aplicar estos conceptos y objetivos se han desarrollado ciertos patrones arquitectónicos, entre los más populares se encuentran:

* Arquitectura Cliente – Servidor

* Arquitectura Basada en componentes

* Diseño impulsado por dominio

* Arquitectura en Capas

* Arquitectura de Bus de Mensajes

* Arquitectura N-Niveles \/ 3 Niveles

* Arquitectura Orientada a Objetos

* Arquitectura Orientada a Servicios \(SOA\)

* Arquitectura de Microservicios

* Arquitectura Cebolla


### 4.2.2 Componente.

Por definición un componente encapsula una parte del software del sistema, contiene una interfaz con la que se comunican otras partes del sistema y estas sirven de base de la estructura de todo el software. A nivel de programación los componentes son representados como módulos, clases, objetos y funciones.

### 4.2.3 Subsistema.

Un subsistema es un conjunto de Componentes que realizan una tarea determinada, se considera una entidad separada dentro de la arquitectura de software, puede interactuar con otros subsistemas y componentes.

### 4.2.4 Patrón Arquitectónico.

Un patrón arquitectónico expresa la organización estructural fundamental de un sistema de software en un esquema. Proporciona un conjunto de subsistemas predefinidos, sus responsabilidades e incluye normas y directrices para organizando las relaciones entre ellos.

### 4.2.5 Arquitectura Cliente-Servidor.

El patrón Cliente-Servidor \(Client-Server Architecture\)  es un modelo de arquitectura de software que básicamente integra dos partes, sistemas cliente y sistemas de servidor, que se comunican a través de una red de ordenadores o en el mismo ordenador. La aplicación de servidor de cliente proporciona una mejor manera de compartir la carga de trabajo. El cliente siempre inicia una conexión con el servidor, mientras que el servidor siempre espera las solicitudes de cualquier cliente. Las arquitecturas cliente-servidor a veces se llaman arquitecturas de dos niveles\(Two-Tier\).

Figura 2 Diagrama del patrón cliente-servidor

### 4.2.6  Arquitectura en Capas.

El patrón de arquitectura en capas \(Layered Architecture\) se enfoca en el agrupamiento de la funcionalidad relacionada dentro de una aplicación en distintas capas que se apilan verticalmente una encima de otra. La funcionalidad dentro de cada capa está relacionada por un rol o responsabilidad común. La comunicación entre capas es explícita y ligeramente acoplada. Realizar una buena selección de las preocupaciones de cada capa apoya la flexibilidad y la facilidad de mantenimiento.

 Figura 3 arquitectura en capas.

### 4.2.7 Arquitectura de Microservicios.

El término "Arquitectura de Microservicios" ha surgido en los últimos años para describir una forma particular de diseñar aplicaciones de software como suites de servicios desplegables de forma independiente. Si bien no existe una definición precisa de este estilo arquitectónico, existen ciertas características comunes alrededor de la organización en torno a la capacidad empresarial, el despliegue automatizado, la inteligencia en los puntos finales y el control descentralizado de lenguajes y datos \[6\].

### 4.2.8 Modelo Vista Controlador \(MVC\).

Model View Controller \(MVC\) es un patrón de diseño para software de computadora. Este enfoque busca distinguir entre el modelo de datos, el control de procesamiento y la interfaz de usuario. Separa cuidadosamente la interfaz gráfica mostrada al usuario del código que gestiona las acciones del usuario. El objetivo es proporcionar un marco que imponga un diseño mejor y más preciso. En cuanto a la comunicación entre las partes es directa.

Figura 4 modelo vista controlador.

Existen unas variaciones en la forma de implementar el mismo patron, entre las que tenemos:

* El modelo pasivo, en el que se emplea un controlador para manipula el modelo exclusivamente. El controlador modifica el modelo y luego informa a la vista que el modelo ha cambiado y debe actualizarse \(ver Figura 5\). El modelo en este escenario es completamente independiente de la vista y el controlador, lo que significa que no hay ningún medio para que el modelo informe de cambios en su estado. El protocolo HTTP es un ejemplo de esto. No hay una forma sencilla en el navegador para obtener actualizaciones asíncronas desde el servidor. El navegador muestra la vista y responde a la entrada del usuario, pero no detecta cambios en los datos del servidor. Sólo cuando el usuario solicita explícitamente una actualización es el servidor interrogado para realizar cambios.

* Figura 5 Comportamiento del modelo pasivo.

* Modelo Activo, este modelo se utiliza cuando el modelo cambia de estado sin la participación del controlador. Esto puede ocurrir cuando otras fuentes están cambiando los datos y los cambios deben reflejarse en las vistas. Considere una visualización de stock-ticker. Recibe datos de stock de una fuente externa y desea actualizar las vistas \(por ejemplo, una banda de ticker y una ventana de alerta\) cuando cambia los datos de stock. Debido a que sólo el modelo detecta cambios en su estado interno cuando se producen, el modelo debe notificar las vistas para actualizar la pantalla.

  Sin embargo, una de las motivaciones del uso del patrón MVC es hacer que el modelo sea independiente de las vistas. Para respetar esto se utiliza un patrón de desarrollo llamado Observer, el cual proporciona un mecanismo para alertar a otros objetos de cambios de estado sin introducir dependencias en ellos. Las vistas individuales implementan la interfaz Observer y se registran con el modelo. El modelo rastrea la lista de todos los observadores que se suscriben a los cambios. Cuando un modelo cambia, el modelo itera a través de todos los observadores registrados y los notifica del cambio. Este enfoque se denomina a menudo "publicar-suscribirse".

* Figura 6 Modelo activo utilizando el patrón Observer.

 



### 4.2. Desarrollo Front-End.

### 4.2. Desarrollo Back-End.

### 4.2. Middleware.

### 4.2. Protocolos.

\[1\] https:\/\/msdn.microsoft.com\/en-us\/library\/ee658098.aspx

\[2\] http:\/\/www.lucemorker.com\/blog\/introduction-to-software-architecture

\[3\] https:\/\/www.pearsonhighered.com\/product\/Bass-Software-Architecture-in-Practice-2nd-Edition\/9780321154958.html

\[4\] https:\/\/www.pearsonhighered.com\/program\/Fowler-Patterns-of-Enterprise-Application-Architecture\/PGM298863.html

\[5\] L. Bass, P. Clements, R. Kazman, Software Architecture in Practice, 2nd Edition, Addison Wesley, 2003

\[6\] http:\/\/www.martinfowler.com\/articles\/microservices.html

\[7\] http:\/\/www.nyu.edu\/classes\/jcf\/g22.3033-007\/slides\/session2\/g22\_3033\_011\_c23.pdf

\[8\] https:\/\/msdn.microsoft.com\/en-us\/library\/ff649643.aspx

\[9\] https:\/\/www.techopedia.com\/definition\/3842\/model-view-controller-mvc

\[10\] http:\/\/www.lab.inf.uc3m.es\/~a0080802\/RAI\/mvc.html


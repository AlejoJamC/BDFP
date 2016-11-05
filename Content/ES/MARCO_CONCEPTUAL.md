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


### 4.2.2 Arquitectura Cliente-Servidor.

El patrón Cliente-Servidor \(Client-Server Architecture\)  es un modelo de arquitectura de software que básicamente integra dos partes, sistemas cliente y sistemas de servidor, que se comunican a través de una red de ordenadores o en el mismo ordenador. La aplicación de servidor de cliente proporciona una mejor manera de compartir la carga de trabajo. El cliente siempre inicia una conexión con el servidor, mientras que el servidor siempre espera las solicitudes de cualquier cliente. Las arquitecturas cliente-servidor a veces se llaman arquitecturas de dos niveles\(Two-Tier\).

Figura 2 Diagrama del patrón cliente-servidor

### 4.2.3  Arquitectura en Capas

El patrón de arquitectura en capas \(Layered Architecture\) se enfoca en el agrupamiento de la funcionalidad relacionada dentro de una aplicación en distintas capas que se apilan verticalmente una encima de otra. La funcionalidad dentro de cada capa está relacionada por un rol o responsabilidad común. La comunicación entre capas es explícita y ligeramente acoplada. Realizar una buena selección de las preocupaciones de cada capa apoya la flexibilidad y la facilidad de mantenimiento.

 Figura 3 arquitectura en capas.

### 4.2.4 Arquitectura de Microservicios

El término "Arquitectura de Microservicios" ha surgido en los últimos años para describir una forma particular de diseñar aplicaciones de software como suites de servicios desplegables de forma independiente. Si bien no existe una definición precisa de este estilo arquitectónico, existen ciertas características comunes alrededor de la organización en torno a la capacidad empresarial, el despliegue automatizado, la inteligencia en los puntos finales y el control descentralizado de lenguajes y datos \[6\].

### 4.2. Modelo Vista Controlador \(MVC\).

### 4.2. Desarrollo Front-End.

### 4.2. Desarrollo Back-End.

### 4.2. Middleware.

### 4.2. Protocolos.

### 4.2. Servidor Virtual Privado \(VPS\).

### 4.2. Dominios de internet.

### 4.2.  Secure Sockets Layer \(SSL\).

### 4.2. HTTPS

\[1\] https:\/\/msdn.microsoft.com\/en-us\/library\/ee658098.aspx

\[2\] http:\/\/www.lucemorker.com\/blog\/introduction-to-software-architecture

\[3\] https:\/\/www.pearsonhighered.com\/product\/Bass-Software-Architecture-in-Practice-2nd-Edition\/9780321154958.html

\[4\] https:\/\/www.pearsonhighered.com\/program\/Fowler-Patterns-of-Enterprise-Application-Architecture\/PGM298863.html

\[5\] L. Bass, P. Clements, R. Kazman, Software Architecture in Practice, 2nd Edition, Addison Wesley, 2003

\[6\] http:\/\/www.martinfowler.com\/articles\/microservices.html


# Oracle Cloud Infraestructure Foundations ☁️

_Dentro de este repositorio podrán encontrarse notas, recursos extra y/o prácticas referentes al curso [Oracle Cloud Infraestructure Foundations](https://mylearn.oracle.com/component/-/108432/166230)_ **(OCI)**

## OCI Architecture ⚙️
Conceptos básicos:
* **Región:** Es un área localizada geográficamente que consta de uno o más _dominios de disponibilidad_.

* **Dominios de disponibilidd:** (O medios de disponibilidad) Son uno o más _centros de datos tolerantes a fallos_ que se ubican dentro de _una región_ que se conectan entre sí por una red de banda ancha.

* **Dominios de errores:** Es una agrupación de HW e infraestructura dentro de un _dominio de disponibilidad_ para proporcionar anti-afinidad. También conocidos como centros de datos lógicos.

**Para elegir una región** 
* 1) Elegir la región más cercana a los usuarios 
     * Latencia baja
     * Rendimiento alto
* 2) Requisitos de residencia y conformidad de datos
* 3) Disponibilidad del servicio

## Identity and Access Management 👥

**IAM**

Conocido como Control de Acceso Detallado o Servicio de Control de Acceso basado en roles.

* AuthN: Autenticación > lidida con la identidad o _quién es alguien_

* AuthZ: Autorización > lidia con el permiso o _lo que alguien puede hacer_

* Dominios de identidad: Contenedor para usuarios de grupos 

**Compartments**

El compartimento raiz es una construcción lógica donde se pueden mantener todos los recursos en la nube.

* Se crean para aislamiento y control de acceso

* Cada recursp que se crea pertenece a un único compartimento

* Se pueden escribir políticas para evitar que los usuarios accedan a recursos de una región específica.

* Todos los compartimentos que se crean son globales y están disponibles en todas las regiones a las que se tenga acceso

* Se pueden crear compartimentos anadidos








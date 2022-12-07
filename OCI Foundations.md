# Oracle Cloud Infraestructure Foundations ☁️

_Dentro de este repositorio podrán encontrarse notas, recursos extra y/o prácticas referentes al curso [Oracle Cloud Infraestructure Foundations](https://mylearn.oracle.com/component/-/108432/166230)_ **(OCI)**.

Para acceder solo da clic en cualquier flecha.

<details><summary> OCI Architecture ⚙️ </summary>


Conceptos básicos:
    
* **Región:** Es un área localizada geográficamente que consta de uno o más _dominios de disponibilidad_.

* **Dominios de disponibilidd:** (O medios de disponibilidad) Son uno o más _centros de datos tolerantes a fallos_ que se ubican dentro de _una región_ que se conectan entre sí por una red de banda ancha.

* **Dominios de errores:** Es una agrupación de HW e infraestructura dentro de un _dominio de disponibilidad_ para proporcionar anti-afinidad. También conocidos como centros de datos lógicos.

**Para elegir una región** 
 1) Elegir la región más cercana a los usuarios 
     * Latencia baja
     * Rendimiento alto
 2) Requisitos de residencia y conformidad de datos
 3) Disponibilidad del servicio
    
</details>

<details><summary> Identity and Access Management 👥 </summary>

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

**AuthN and AuthZ**

Un principal es una entidad de IAM que puede interactuar con recursos de OCI. Existen 2 tipos de principales:
    * Los usuarios: Las personas que inician sesión en la consola de CLI o SDK, seres humanos que realmente utilizan los recursos en la nube.
    * Los recursos

* Autenticación o AuthN: Claves de firma de API (públicas y privadas), los tokens que son cadenas de token generadas por Oracle.

* Autorización o AuthZ: Se ocupa de los permisos y de averiguar qué permisos tiene. En OCI se realiza mediante políticas de IAM. Las políticas se pueden asociar a un compartimento o se pueden asociar a un arrendamiento. 

* Niveles de Verbs: Administrador/Manage, Uso/Use, Lectura/Read e Inspección/Inspect.

**Tenancy Setup**

Tenancy Admin > OCI Admin > OCI-admin-groups > Policies > name-compartment

Mejores prácticas:
 1) No usar la cuenta de admin de arrendamiento para operaciones diarias.
 2) Crear compartimentos dedicados para aislar recursos
 3) Aplicar el uso de la autenticación multifactor

Ejemplo para otorgar permisos de admin a un grupo de administradores de OCI:
    
![ ](imgOCI/OCI-create-policy.png)
    
</details>

<details><summary> Networking 🌐📡  </summary>

**VCN Introduction**


</details>



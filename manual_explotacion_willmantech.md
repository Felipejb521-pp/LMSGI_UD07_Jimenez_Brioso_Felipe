## Introduccion y Arquitectura
    Documento técnico que servirá de guia para administradores de sistemas y usuarios que usen el ERP.
    Optimizaremos flujos de ventas y facturación.

* **  t-call Invoca el contenedor HTML base de Odoo.
* **  t-foreach Itera sobre los documentos a renderizar
* **  t-field  Vincula campos del modelo al HTML
* **  t-if Oculta la columna si ninguna linea tiene descuento

## Guia de instalacion y reinstalacion

# Requisitos  
    |-Docker
    |-Docker compose
    |-Git
* 1º Clonar Repositorio git
* 2º Crear Fichero
* 3º Levantar los contenedores
* 4º Verificar que los contenedores estan corriendo

## Seguridad y control de acceso
* ** Verificación mediante contraseña fuerte (8-16 caracteres)
* ** Roles definidos de Administrador(Acceso total), Contable y Comercial

## Procedimiento de Backup y restauracion
 El proceso de backup tiene como objetivo garantizar la recuperación íntegra del sistema ERP ante fallos lógicos, errores humanos, corrupción de datos o desastres de infraestructura.

# El respaldo debe cubrir:

* Base de datos relacional.
* Archivos adjuntos y documentos.
* Configuración del entorno.
* Volúmenes Docker persistentes.

# Flujo Operativo de Facturación e Informes
* **Acceso cliente web --> Proxy --> Aplicacion ERP --> Motor BD --> Almacenamiento de Archivos

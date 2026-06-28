
# CMS Builder Community Edition

CMS Builder Community Edition es un generador de aplicaciones CRUD desarrollado en PHP y MySQL que permite crear paneles de administración completos de forma visual, sin necesidad de programar cada módulo manualmente.

El sistema genera automáticamente tablas, formularios, relaciones entre módulos y una API REST lista para consumir desde cualquier aplicación.

Este proyecto contiene la base del instalador y la configuración inicial necesaria para preparar una instalación del sistema.

La versión actual del CMS se encuentra en:

https://github.com/puricalvo/cms-builder

## Características

* Instalación guiada en menos de un minuto.
* Dashboard totalmente configurable.
* Generador visual de módulos CRUD.
* API REST integrada.
* Gestión dinámica de tablas y formularios.
* Sistema de permisos por roles.
* Configuración visual del dashboard.
* Integración con ChatGPT mediante API.
* Arquitectura MVC sencilla y extensible.

## Requisitos

* PHP 8.1 o superior.
* MySQL o MariaDB.
* Composer.
* Servidor Apache o Nginx.

## Instalación

1. Clona o descarga el proyecto.

2. Instala las dependencias de Composer.

---
```bash
composer install
```
---

3. Copia el archivo:

---
```text
.env.template
```
---

como:

---
```text
.env
```
---

y configura las variables de entorno.

4. Crea una base de datos vacía.

5. Accede desde el navegador al instalador.

Durante la instalación se crearán automáticamente:

* El dashboard.
* El módulo de administradores.
* El usuario SuperAdmin.
* La estructura inicial del sistema.

## Estructura del proyecto

---
```text
web/
│
├── controllers/
├── modules/
├── views/
│   ├── assets/
│   ├── pages/
│   └── template.php
│
├── vendor/
├── .env.template
├── composer.json
├── index.php
└── README.md
```
---

## API REST

Todos los módulos creados desde el dashboard generan automáticamente sus correspondientes endpoints REST.

La API permite realizar operaciones:

* GET
* POST
* PUT
* DELETE

sin necesidad de escribir código adicional.

## ChatGPT

CMS Builder permite integrar ChatGPT dentro de cualquier módulo mediante campos dinámicos.

Para utilizar esta funcionalidad es necesario configurar las credenciales de OpenAI desde el panel de administración.

## Personalización

El dashboard permite configurar:

* Nombre del proyecto.
* Símbolo.
* Color principal.
* Tipografía.
* Imagen de fondo del login.

## Licencia

CMS Builder Community Edition se distribuye para fines educativos y de desarrollo.

Puedes modificarlo y adaptarlo a tus propios proyectos respetando las condiciones de la licencia correspondiente.

## Autor

Desarrollado por **Puri Calvo**.

Proyecto creado para facilitar el desarrollo rápido de aplicaciones administrativas mediante una arquitectura visual basada en PHP, MySQL y API REST.


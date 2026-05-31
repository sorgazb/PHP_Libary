# PHP Library

![PHP](https://img.shields.io/badge/PHP-8-777bb4?style=for-the-badge&logo=php)&nbsp;![MySQL](https://img.shields.io/badge/MySQL-Database-4479a1?style=for-the-badge&logo=mysql)&nbsp;![Bootstrap](https://img.shields.io/badge/Bootstrap-5-7952b3?style=for-the-badge&logo=bootstrap)&nbsp;![Composer](https://img.shields.io/badge/Composer-Dependencias-885630?style=for-the-badge&logo=composer)&nbsp;![DWES - DAW](https://img.shields.io/badge/DWES-GS--DAW-1565c0?style=for-the-badge)

> **PHP Library** es una aplicación web de gestión de biblioteca desarrollada en **PHP** con arquitectura **MVC**, como proyecto de la asignatura **Desarrollo Web en Entorno Servidor (DWES)** del ciclo **GS-DAW** en el **IES Augustobriga**. Permite gestionar libros, socios y préstamos con persistencia en **MySQL** y envio de notificaciones por correo.

---

## 📋 Descripción

Aplicación web completa para la gestión integral de una biblioteca, con sistema de autenticación y panel de administración. Sus funcionalidades principales incluyen:

- **Gestión de libros**: alta, baja, modificación y consulta del catálogo.
- **Gestión de socios**: registro, edición y consulta de usuarios de la biblioteca.
- **Gestión de préstamos**: control de préstamos activos y devoluciones.
- **Sistema de login**: autenticación de usuarios con sesiones PHP.
- **Envío de correos**: notificaciones automáticas via `Correo.php` con Composer.
- **Script SQL**: base de datos lista para importar (`scriptBiblioteca.sql`).

---

## 🏗️ Estructura del Proyecto

```txt
PHP_Libary/
└── Biblioteca/
    ├── Libro.php              # Clase entidad Libro
    ├── Socio.php              # Clase entidad Socio
    ├── Prestamo.php           # Clase entidad Préstamo
    ├── Usuario.php            # Clase entidad Usuario
    ├── Correo.php             # Envio de correos con Composer
    ├── Modelo.php             # Capa de acceso a datos (MySQL)
    ├── controlador.php        # Lógica de negocio y enrutamiento
    ├── login.php              # Vista de autenticación
    ├── menu.php               # Vista del menú principal
    ├── libros.php             # Vista de gestión de libros
    ├── socios.php             # Vista de gestión de socios
    ├── prestamos.php          # Vista de gestión de préstamos
    ├── scriptBiblioteca.sql   # Script de creación de la base de datos
    ├── composer.json          # Dependencias PHP
    ├── composer.lock
    └── vendor/                # Librerías instaladas por Composer
```

---

## ⚙️ Instalación y Ejecución

Clona el repositorio:
```txt
git clone https://github.com/sorgazb/PHP_Libary.git
cd PHP_Libary/Biblioteca
```

Instala las dependencias con Composer:
```txt
composer install
```

Importa la base de datos en MySQL:
```txt
mysql -u root -p < scriptBiblioteca.sql
```

Sirve el proyecto con un servidor local (XAMPP, Laragon o PHP built-in):
```txt
php -S localhost:8000
```

---

## 📸 Ejemplos de Ejecución

<p align="center">
  <img src="https://github.com/user-attachments/assets/d6d14c0d-96ef-4bee-859c-e0efe9fd1a9f" alt="Captura 1" width="700"/>
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/c6fb576a-56f9-43bc-82be-d7574302c531" alt="Captura 2" width="700"/>
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/8f6d72a5-3816-4d5e-88af-942172032872" alt="Captura 3" width="700"/>
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/390c92a3-84cb-4fa9-bde5-4ef6dcedcac1" alt="Captura 4" width="700"/>
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/f9685a77-f92c-4595-990e-c92d67a66a6e" alt="Captura 5" width="700"/>
</p>

---

## 🤝 Contribución

Haz fork del repositorio.

Crea una rama de trabajo:

```txt
git checkout -b feature/nueva-funcionalidad
```

Realiza tus cambios y haz commit.

Abre un Pull Request describiendo tus mejoras.

---

<p align="center">
  <strong>Desarrollo Web en Entorno Servidor (DWES)</strong> &nbsp;&middot;&nbsp; GS-DAW &nbsp;&middot;&nbsp; IES Augustobriga
  <br/>
  Sergio Orgaz Bravo
</p>

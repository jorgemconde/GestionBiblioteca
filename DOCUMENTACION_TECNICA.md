# Sistema de Gestión de Biblioteca

**Autor:** Jorge  
**Asignatura:** Programación Avanzada - ACA Final  
**Fecha:** 2026  

---

## 1. Introducción
El presente documento describe el diseño, la arquitectura y el desarrollo del Sistema de Gestión de Biblioteca, una aplicación de escritorio desarrollada para automatizar y administrar eficientemente los procesos bibliotecarios de una institución educativa.

## 2. Planteamiento del Problema
Las instituciones educativas requieren un control riguroso sobre su inventario bibliográfico, el registro de usuarios y el flujo de préstamos y devoluciones. La ausencia de un sistema centralizado genera inconsistencias en los datos, pérdida de libros y dificultades en la generación de reportes y seguimiento de préstamos activos.

## 3. Objetivos
* **Objetivo General:** Desarrollar una aplicación de escritorio en C#, Windows Forms y SQL Server para la gestión integral de la biblioteca, aplicando los principios de la Programación Orientada a Objetos y arquitectura por capas.
* **Objetivos Específicos:**
  * Implementar operaciones CRUD para libros, autores, editoriales y usuarios.
  * Gestionar el control de préstamos y devoluciones con validaciones de integridad.
  * Diseñar una base de datos relacional robusta en SQL Server.

## 4. Arquitectura del Sistema
El proyecto se estructuró bajo una arquitectura lógica de tres capas para separar las responsabilidades:
* **Capa de Presentación (Windows Forms):** Formularios e interfaz gráfica para la interacción con el usuario.
* **Capa de Negocio (BLL):** Validación de reglas de negocio y procesamiento de datos.
* **Capa de Datos (DAL):** Gestión de la conexión y ejecución de consultas parametrizadas hacia SQL Server.

## 5. Módulos Desarrollados
* **Módulo de Inicio:** Interfaz principal y navegación general del sistema.
* **Módulo de Libros:** Registro, consulta, edición y eliminación de registros bibliográficos enlazados con autores y editoriales.
* **Módulos de Autores, Editoriales y Usuarios:** Administración completa de los actores y entidades del sistema.
* **Módulo de Préstamos y Devoluciones:** Control de asignación de libros a usuarios y actualización de estados.
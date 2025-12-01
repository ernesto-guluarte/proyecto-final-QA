# 🏆 Proyecto Final de Entrenamiento: Urban Scooter QA

---

## 📝 Descripción del Proyecto

Este proyecto es una **simulación de entorno real** que consolida el conocimiento y las habilidades de un QA Tester, cubriendo un amplio espectro de actividades de prueba manual:

1.  **Pruebas Web:** Validación funcional y de datos en la aplicación web Urban Scooter.
2.  **Pruebas Móviles:** Elaboración y ejecución de casos de prueba para la aplicación móvil (notificaciones, manejo de conexión).
3.  **Pruebas de API (Backend):** Creación de listas de comprobación para validar *endpoints* de Repartidores y Pedidos.
4.  **Prueba Teórica:** Demostración de conocimientos fundamentales de la teoría de QA y diseño de pruebas.

El propósito principal fue aplicar diversas técnicas de diseño de pruebas (Mapas Mentales, Listas de Comprobación, Casos de Prueba, Clases de Equivalencia y Valores Límite) para identificar y reportar fallas en las tres plataformas del sistema.

---

## 🛠️ Tecnologías y Artefactos

El enfoque del proyecto fue completamente en las pruebas **Manuales de Caja Negra** y la creación de artefactos de prueba siguiendo estándares profesionales.

| Categoría | Artefactos Desarrollados | Enfoque de Pruebas |
| :--- | :--- | :--- |
| **Pruebas Web** | Mapa Mental, Lista de Comprobación, Casos de Prueba, Validación de Datos. | Pruebas funcionales, pruebas de validación de entradas, *testing* en distintos navegadores (Chrome, Opera). |
| **Pruebas Móviles** | Casos de Prueba. | Pruebas de usabilidad, manejo de interrupciones y fallas de conexión, notificaciones *push*. |
| **Pruebas de API (Backend)** | Lista de Comprobación. | Pruebas de funcionalidad de *endpoints* (`POST /courier`, `GET /orders`), validación de códigos de respuesta (HTTP) y pruebas de frontera de datos. |
| **Teoría de QA** | Preguntas/Respuestas de Conceptos. | Demostración de conocimientos sobre el ciclo de vida de los requisitos, diseño de pruebas y estrategias de automatización. |

---

## 🎯 Tareas Solicitadas

Esta sección transcribe las instrucciones recibidas por parte de la supervision para este proyecto, detallando las tareas que se desarrollaron y cuyos resultados se encuentran en el archivo `Tareas - Contenido.xlsx`.

### Tarea 1: Teoría de las Pruebas

Tarea de conocimiento teórico sobre QA para demostrar entendimiento en conceptos fundamentales. Las preguntas y respuestas se encuentran en la pestaña "Tarea 1" del archivo `Tareas - Contenido.xlsx`.

### Tarea 2: Aplicación Web Urban Scooter

Pruebas manuales para la aplicación web de Urban Scooter.

Para esta tarea, supervisión solicitó realizar lo siguiente:

* **Desarrollo de un Mapa Mental** de la función del formulario de pedido.
* **Elaboración de una Lista de Comprobación** de los requisitos de función de la pantalla **"Estado del pedido"**.
* **Creación de Casos de Prueba** para validar los campos de la pantalla **"Hacer pedido"** (incluyendo la validación de datos y el uso de técnicas de diseño como Clases de Equivalencia y Valores Límite).
* **Prueba de las funciones en base a listas de comprobación/tablas resultantes.**

Para realizar esta tarea se tomo la información de sobre la pantalla para realizar pedido y pantalla de estado de pedido, que se muestra en el documento de requisitos (ubicado en la ruta: “requisitos\2_requisitos_aplicacion_web.pdf”). Y también como material de apoyo para ver las pantallas se pueden usar las capturas de pantalla (ubicadas en la carpeta “imágenes\”) y para validar los campos de la pantalla “Realizar Pedido”, los datos validos para dichos campos se especifica en el documento de requisitos de aplicación web.

El mapa mental, la lista de comprobación y los casos de prueba para esta tarea, se encuentra en el archivo “Tareas – Contenido.xlsx” en las pestañas tituladas: "Tarea 2: mapa mental", "Tarea 2: lista de comprobación", "Tarea 2: datos de validación" del archivo `Tareas - Contenido.xlsx`.

### Tarea 3: Aplicación Móvil Urban Scooter

Pruebas manuales para la aplicación móvil de Urban Scooter.

En esta tarea supervisión solo solicito realizar pruebas de lo que aparece en texto en negrita del documento de requisitos de la aplicación móvil.: (requisitos\3_requisitos_aplicacion_movil). Lo cual se resume en la realización de las siguientes actividades:

* **Creación de Casos de Prueba** para la función de **notificaciones push**.
* **Creación de Casos de Prueba** para verificar el manejo de una **falla de conexión** a Internet.
* **Prueba de las funciones** en base a los casos de prueba creados.

Los casos de prueba para esta tarea, se encuentra en el archivo `Tareas - Contenido.xlsx` en la pestaña titulada “Tarea 3 casos de prueba”

### Tarea 4: Pruebas de API (Backend)

Pruebas funcionales para la API del backend de Urban Scooter. 

En esta tarea supervisión solo solicitó realizar pruebas de lo que aparece en texto en negrita del documento de requisitos del backend: (requisitos\3_requisitos_backend), lo cual se resume en la validacion de las siguientes:

* **URL para Repartidores:**
    * Debe estar presente y permitir el **registro** (`login`, `passwordHash`, `firstName`).
    * El campo `login` debe ser **único**.
    * Si el registro es exitoso, la entrada debe aparecer en la base de datos (tabla Couriers). Si no, debe devolver un error.
    * Debe haber una URL para **eliminar la cuenta** del repartidor (borrando pedidos vinculados en la tabla Orders).
* **URL para los Pedidos:**
    * Debe haber una URL para **recuperar los datos del pedido** a partir de su número de seguimiento.
    * Si se encuentra un pedido, se devuelven sus datos; de lo contrario, se debe devolver un error.

La lista de comprobación para esta tarea, se encuentra en el archivo `Tareas - Contenido.xlsx` en la pestañas titulada "Tarea 4: lista de comprobación”

---

## 📂 Estructura del Proyecto

La carpeta principal contiene los siguientes archivos y directorios:

| Archivo/Carpeta                                  | Contenido |
|:-------------------------------------------------| :--- |
| `README.md`                                      | Este documento de información consolidada. |
| [Tareas - Contenido.xlsx]                        | Archivo central que contiene todos los resultados de la ejecución de pruebas. Pruebas teóricas (Tarea 1), Mapa Mental (Tarea 2), Listas de Comprobación (Tarea 2 y 4) y Casos de Prueba (Tarea 2 y 3). |
| `/imagenes`                                      | Contiene las capturas de pantalla relacionadas con las pruebas (si aplica). | — |
| `/requisitos`                                    | Contiene la documentación de requisitos de las aplicaciones probadas. | — |
| `/mapa_mental`                                   | Contiene una imagen del Mapa Mental de la función "Hacer pedido" de la Web. | — |
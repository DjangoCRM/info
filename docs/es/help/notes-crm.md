---
title: Trabajar con memos (notas del CRM)
description: Aprende a utilizar la lista de memos del CRM en Django CRM para ver, ordenar, filtrar y gestionar notas internas, así como realizar un seguimiento de las tareas relacionadas.
---

# **Trabajar con memos en Django CRM**

Las notas del CRM ofrecen a los usuarios una funcionalidad práctica para trabajar con **memos (notas del CRM)**,
que son mensajes internos que pueden servir como notas personales, memorandos de oficina o notas de servicio.
Cualquier usuario del CRM puede crear un memo y especificar para quién está destinado:
para sí mismo, para su responsable de departamento o para la empresa.

Los memos permiten documentar las comunicaciones internas y mantener toda la información relacionada dentro del módulo de notas del CRM.
Esta función ayuda a los equipos a conservar un registro estructurado de comunicaciones, decisiones y acciones de seguimiento.

---

## **Roles de usuario en los memos del CRM**

Cada memo tiene varios roles de usuario que definen cómo interactúan los participantes con él:

- **Propietarios** – usuarios que crean los memos del CRM.
- **Destinatarios** – personas para quienes están destinados los memos.
- **Suscriptores** – usuarios que deben recibir notificaciones sobre el memo y, si procede, sobre las tareas creadas como resultado de su revisión.

---

## **Estados de los memos**

Hay disponibles los siguientes estados para informar a los participantes:

- **Pendiente** – el memo está esperando ser revisado.
- **Aplazado** – la revisión se ha retrasado.
- **Considerado** – el memo ya ha sido revisado.

El estado de un memo del CRM lo actualiza su destinatario.
Después de establecer el estado **“considerado”**, el propietario ya no puede editarlo ni cambiar
los archivos adjuntos.

Todos los participantes reciben automáticamente una notificación en la interfaz del CRM y por correo electrónico cuando se crea o revisa un memo.
Se usa el mismo método de notificación para los mensajes del chat del memo.

---

## **Chat del memo y tareas relacionadas**

Cada memo incluye un **chat** donde los participantes pueden intercambiar mensajes y archivos.
Por ejemplo, los usuarios pueden aclarar detalles o notificar a otros sobre acciones de seguimiento después de revisar el memo.
Si se crea una tarea como resultado de la revisión del memo, la comunicación posterior debe realizarse en el **chat de la tarea**.

En la lista de memos aparece un botón **“Ver tarea”** junto a los memos que dieron lugar a una tarea.
El **color del botón** indica el estado de la tarea, y la **información emergente** muestra el nombre del estado al pasar el cursor por encima.

La integración entre memos y tareas en **Notas CRM** garantiza que las decisiones y las acciones permanezcan conectadas, permitiendo a los usuarios seguir cada paso desde la comunicación hasta la ejecución.

---

## **Resumen de la lista de memos**

La **página de la lista de memos** es el espacio de trabajo principal para gestionar todas las notas del CRM.
Aquí, los usuarios pueden ver, ordenar, filtrar y buscar memos, así como crear nuevos o duplicar los existentes.

Los memos se muestran en una tabla con la siguiente información:

- **Título del memo**
- **Destinatario** (a quién está dirigido el memo)
- **Icono de archivo** (indica los adjuntos)
- **Icono de estado** (aparece una información emergente al pasar el cursor)
- **Fecha revisada** (cuando el destinatario revisó el memo)
- **Botón de tarea abierta** — aparece si se creó una tarea después de la revisión del memo; su color corresponde al estado de la tarea (también muestra una información emergente al pasar el cursor)
- **Propietario del memo (autor)**
- **Departamento del propietario**
- **Fecha de creación**
- **Botón de copiar memo** – abre un nuevo formulario de memo precargado con los datos del memo actual

---

## **Ordenación, filtrado y búsqueda**

Los usuarios pueden navegar fácilmente por los memos utilizando herramientas integradas:

- **Ordenación** – por título, destinatario, autor y fecha de creación.
- **Filtrado** – por estado, destinatario, propietario o fecha de creación.
- **Búsqueda** – por palabra clave o ID del memo.

Cada usuario solo ve los memos en los que aparece en cualquier rol (propietario, destinatario o suscriptor).

---

## **Ver también**

Para obtener más información sobre cómo crear o gestionar memos, consulta los siguientes temas relacionados:

- [Crear un memo en Django CRM](creating-crm-note.md)
- [Editar y revisar memos](editing-updating-crm-note.md)
- [Notas del CRM y tareas](../features/tasks-app-features.md)

---

## **Notas del CRM**

El uso de la funcionalidad de memos en Django CRM ayuda a organizar la comunicación interna y conservar información importante relacionada con el trabajo dentro del sistema.
Con **Notas CRM**, los usuarios pueden crear, compartir y revisar memos de forma eficiente, adjuntar archivos de apoyo y vincular las conversaciones a tareas ejecutables.
Esta funcionalidad convierte Django CRM en una solución práctica para gestionar tanto notas diarias como correspondencia empresarial formal en un solo lugar.

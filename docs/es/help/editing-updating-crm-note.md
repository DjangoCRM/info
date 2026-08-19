---
title: Editar y actualizar memos del CRM
description: Aprende a editar y actualizar memos del CRM en Django CRM, incluyendo permisos, cambios de estado e integración con tareas y proyectos.
---

# **Editar y actualizar memos del CRM**

Django CRM permite a los usuarios editar o actualizar [memos](notes-crm.md) existentes — notas del CRM — manteniendo
una transparencia total sobre quién realizó cambios y cuándo. Un memo solo puede editarse por su **propietario (autor)**
o **destinatario**, lo que garantiza un acceso controlado y responsabilidad.

---

## **Quién puede editar un memo**

* **El propietario (autor)** puede editar o eliminar el memo del CRM mientras su estado es **Pendiente**.
* **El destinatario** puede actualizar el estado del memo a **Considerado** o **Aplazado**. Una vez que el destinatario cambia el estado, el autor pierde la capacidad de editar o eliminar el memo.

El campo **"Modificado por"** muestra el nombre del último usuario que editó el memo, y puede ver el **historial completo de ediciones** haciendo clic en el botón **Historial**.

---

## **Reenvío y cambios de estado**

Los destinatarios pueden **reenviar un memo** a otro usuario seleccionando un nuevo destinatario. Esto permite que el memo avance por la cadena de aprobación o revisión adecuada.

Cambiar el estado del memo ayuda a seguir el progreso y a garantizar que cada nota reciba la atención oportuna.

---

## **Crear una tarea o proyecto como resultado de la revisión del memo**

El destinatario puede **[crear una tarea](creating-assigning-tasks.md) o un proyecto** directamente desde un memo. En este caso:

* Todos los datos del memo, incluidas las fichas adjuntas, se transferirán automáticamente.
* El **autor y los suscriptores** del memo pasarán a ser **suscriptores de la nueva tarea o proyecto** y recibirán notificaciones.
* El destinatario puede añadir sus propias notas o conclusiones en el campo **"Conclusión"**.

Si se ha creado una tarea o un proyecto, aparecerá un **botón para verlo** en el memo.

> Más información: [CRM y gestión de tareas](../features/tasks-app-features.md) | [CRM y gestión de proyectos](../features/crm-and-project-management.md)

---

## **Crear recordatorios o nuevos memos**

Puede crear fácilmente un **recordatorio** o una **nota nueva** basada en el memo actual haciendo clic en el botón **Copiar**. Esto simplifica la documentación repetitiva y ayuda a realizar un seguimiento de las actividades relacionadas.

> Tema relacionado: [Creación de un memo](creating-crm-note.md)

---

## **Usar el chat integrado**

Cada memo tiene un **chat integrado** donde los usuarios pueden discutir su contenido y coordinar actualizaciones.

* El **autor** puede utilizar el chat para comentar o proporcionar actualizaciones después de que el memo haya sido revisado (ya que la edición directa ya no estará disponible).
* Si se ha creado una **tarea o proyecto** a partir del memo, las discusiones posteriores deben continuar en el **chat correspondiente de la tarea o proyecto**.

---

## **Opciones adicionales**

Si el memo se creó originalmente a partir de un **deal** (oferta), aparecerá un botón **"Ver deal"**, que le permitirá navegar rápidamente al registro CRM asociado.

> Tema relacionado: [Trabajar con ofertas en el CRM](working-with-deals.md)

---

Al ofrecer permisos estructurados, un historial detallado de cambios e integración con tareas,
proyectos y chats, Django CRM garantiza que la gestión de memos siga siendo transparente y eficiente.

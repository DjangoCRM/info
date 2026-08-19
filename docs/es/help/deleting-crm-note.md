---
title: Eliminar memos del CRM
description: Aprende a eliminar memos del CRM en Django CRM, incluidos los permisos, los efectos de la eliminación y las mejores prácticas para mantener organizados los registros de comunicación.
---

# Eliminar un memo del CRM

Si un [**memo del CRM**](../features/tasks-app-features.md#enhance-your-workflow-with-memos-crm-notes) ya no es relevante, puede eliminarlo del sistema.
Eliminar el memo ayuda a mantener organizado el espacio de trabajo y garantiza que solo permanezcan
las comunicaciones actuales y activas en el CRM.

Sin embargo, antes de proceder con la eliminación, revise los siguientes puntos importantes.

---

## **Quién puede eliminar un memo**

Solo el **autor (propietario)** y el **destinatario** del memo pueden eliminarlo.

- Una vez que el destinatario revisa el memo y actualiza su estado
	(por ejemplo, lo marca como *considerado* o *aplazado*),
	el autor ya no podrá eliminarlo.
- Si el **destinatario** elimina el memo, se considera una mala práctica,
	ya que puede provocar inconsistencias en los registros de comunicación.

---

## Qué ocurre cuando se elimina un memo

Al eliminar un memo, Django CRM elimina cuidadosamente solo el memo,
sin afectar a los registros relacionados.

Tenga en cuenta lo siguiente:

- La lista de objetos que se eliminarán puede incluir vínculos entre objetos y usuarios,
	pero **los usuarios nunca se eliminan**.
- Las [**tareas**](../features/tasks-app-features.md) o [**proyectos**](../features/crm-and-project-management.md) creados a partir del memo permanecen en el sistema.
- Los **archivos** transferidos desde el memo a una tarea o proyecto **no se eliminan**.

En otras palabras, eliminar un memo no afectará a otros datos del CRM relacionados con él: solo elimina el memo.

---

## Información relacionada

* [Crear un memo](creating-crm-note.md)
* [Editar un memo](editing-updating-crm-note.md)
* [Trabajar con memos del CRM](notes-crm.md)

---

## Buenas prácticas

Antes de eliminar un memo, asegúrese de que ya no sea necesario para informes, consultas posteriores
o el seguimiento de las comunicaciones.
Si una nota contiene información valiosa relacionada con un proyecto o una tarea, considere conservarla
y marcarla como considerada en lugar de eliminarla.

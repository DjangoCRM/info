---
title: Crear un memo en el CRM
description: Aprende a crear y gestionar memos (notas del CRM) en Django CRM para mejorar la comunicación interna y la organización.
---

# **Crear un memo - Nota del CRM**

La **página de creación de memos** de Django CRM permite a los usuarios crear y enviar memos internos,
como notas personales, comunicados de oficina o notas de servicio,
para sí mismos, sus responsables o toda la empresa.
Esta función ayuda a organizar la comunicación dentro del CRM, registrar decisiones
y [iniciar una tarea](task-management.md) como resultado de la revisión del memo.

---

## **Quién puede crear un memo**

Cualquier usuario del CRM puede crear un memo. El autor de un memo es su **propietario** y tiene control total sobre su contenido hasta que se revise.
Una vez revisado el memo y cambiado su estado a *considerado*, el propietario ya no puede editarlo ni reemplazar los archivos adjuntos.

---

## **Roles del memo**

Al crear un memo, los usuarios definen sus participantes:

- **Propietario**: el usuario que crea el memo (se asigna automáticamente).
- **Destinatario**: el usuario para quien está destinado el memo (se selecciona de la lista disponible).
- **Suscriptores**: los usuarios que deben recibir información sobre el memo (reciben notificaciones y pueden verlo).

---

## **Estados y etapas de los memos**

Al crear un memo, primero puede guardarlo como **borrador**.
En este caso, solo usted (y los administradores del CRM) pueden verlo y no se envían notificaciones.

Después de compartir un memo con otros usuarios, pasa por varias **etapas**:

- **Pendiente**: el memo espera ser revisado.
- **Aplazado**: la revisión se ha retrasado.
- **Considerado**: el memo ha sido revisado. En esta etapa, su contenido queda bloqueado para la edición.

Todos los participantes reciben notificaciones del CRM y por correo electrónico cuando se crea el memo y cuando cambia su estado.

---

## **Cómo crear un memo**

Para crear un nuevo memo, vaya a la [**página de lista de memos**](notes-crm.md) y haga clic en **AÑADIR MEMO** o en el icono **Copiar nota**.
La segunda opción abre un formulario rellenado previamente con los datos del memo seleccionado.

Complete los campos del formulario de creación del memo:

1. **Título del memo**: introduzca un nombre breve y claro para el memo.
2. **Casilla Borrador**: selecciónela si desea guardar el memo como borrador (visible solo para usted).
3. **Destinatario**: elija el usuario al que va dirigido el memo.
4. **Propósito (opcional)**: elija uno de los propósitos predefinidos:

	- para información
	- para consideración
	- para aprobación
	- para dejar constancia
	- para tomar una decisión
	- pago de gastos habituales

5. **Descripción**: proporcione el contenido detallado del memo.
6. **Suscriptores**: seleccione los usuarios que deben recibir una notificación sobre el memo.
7. **Archivos adjuntos**: cargue los archivos relacionados con el memo.

Una vez que guarde la nota del CRM, aparecerá en su **lista de memos**
y será visible para todos los usuarios especificados en ella (destinatarios y suscriptores).
También recibirán notificaciones automáticas sobre su creación.

---

## **Páginas relacionadas**

- [Página de lista de memos](notes-crm.md): permite ver, buscar y gestionar sus memos.
- [Página de edición de memos](editing-updating-crm-note.md): permite actualizar un memo existente antes de que se revise.
- [Página de eliminación de memos](deleting-crm-note.md): permite confirmar y eliminar un memo si es necesario.

---

**Consejo:** Use los memos no solo como recordatorios, sino también como una forma formal de documentar decisiones, aprobaciones internas
y acciones que requieran tareas de seguimiento.

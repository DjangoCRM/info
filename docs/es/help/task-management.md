---
title: Gestionar tareas, subtareas y colaboración
description: Aprenda cómo usar la lista de tareas de CRM, crear tareas personales y de equipo, gestionar subtareas, actualizar
  estados, usar filtros y etiquetas, y colaborar mediante chat integrado y notificaciones.
---

# **Gestión de Tareas en Django CRM**

La lista de tareas en Django CRM ayuda a los usuarios y equipos a organizar el trabajo diario,
gestionar tareas personales y [de equipo](#working-with-team-task), hacer seguimiento del progreso con subtareas,
y comunicarse directamente en chats de tareas. Aquí aprenderá cómo crear tareas,
asignar roles, actualizar estados, usar filtros y etiquetas, y hacer que el trabajo en equipo sea más eficiente con
notificaciones automatizadas y herramientas de colaboración.  
Lea más sobre las características clave de [software de gestión de tareas](../features/tasks-app-features.md).

---

## **Crear tarea**

Para crear una [nueva tarea](creating-assigning-tasks.md), haga clic en el botón "**AGREGAR TAREA +**" en la esquina superior derecha.
Después de completar el formulario y guardar la tarea, podrá crear subtareas en ella.

### Quién Puede Crear Tarea

- Un **gerente** o **jefe de departamento** puede asignar tareas a su equipo.
- Los **usuarios** también pueden crear tareas para **sí mismos**. En este caso, el jefe de departamento se agrega automáticamente como copropietario.
- En tarea de equipo, los **ejecutores** pueden crear subtareas para **uno otro**.

---

![Captura de pantalla de filtros de tareas en CRM](../assets/img/screenshots/crm_task_filters_screenshot.webp){ loading=lazy align="right" }

## **Filtros de Tareas**

Use el **panel de filtros** en el lado derecho de la lista de tareas para encontrar rápidamente tareas.

- Los gerentes pueden filtrar por empleado para ver su carga de trabajo actual.
- Algunos filtros tienen valores predeterminados (por ejemplo, la lista predeterminada muestra solo tareas activas).

---

## **Ordenar Tareas**

- Por defecto, las tareas nuevas aparecen en la parte superior de la lista.
- Para un seguimiento más efectivo, especialmente con el tiempo, se recomienda ordenar tareas por la **fecha del Siguiente Paso**.
- El ordenamiento se puede cambiar con el botón de alternancia en la esquina superior derecha de la lista de tareas.

La mayoría de los títulos de la tabla de tareas están activos. Al hacer clic en ellos, también puede ordenar tareas.
<figure markdown="span">
    ![Captura de pantalla de encabezados de tabla de tareas en CRM](../assets/img/screenshots/task_table_headers_screenshot.webp){ loading=lazy }
    <figcaption>Ordenar tareas por prioridad</figcaption>
</figure>

---

## **Tipos de Tareas**

- **Tarea personal** – asignada a un único usuario.
- [**Tarea de equipo**](#working-with-team-task) – involucra a múltiples usuarios.
- **Subtarea** – puede crearse para cualquier tarea. Una tarea se convierte en una **tarea principal** si tiene al menos una subtarea.
- Las tareas también pueden pertenecer a un **proyecto** para una mejor organización.

---

## **Roles de Usuario**

Cada tarea puede tener diferentes participantes con roles específicos:

- **Propietario** – el usuario que creó y gestiona la tarea.
- **Copropietario** – usuario asignado automáticamente o manualmente (*opcional*).
- **Responsable (ejecutores)** – usuarios que realizan trabajo o lo delegan creando subtareas para otros y gestionándolas.
- **Suscriptores** – notificados sobre el progreso y resultados de la tarea.
- **Operadores de tarea (*opcional*)** – administradores con los mismos derechos que los propietarios.  
Este rol es similar al administrador de CRM pero tiene derechos solo en el módulo de gestión de tareas.
Para obtener este rol, comuníquese con su administrador de CRM.

---

## **Estados de Tarea**

Las tareas pasan por diferentes estados:

- **Pendiente**, **En progreso**, **Hecho**, **Pospuesto**, **Cancelado**.

El **ejecutor** generalmente actualiza el estado, pero los propietarios u operadores también pueden hacerlo.

- En tareas de equipo, los primeros tres estados se actualizan automáticamente.
- Los estados se pueden cambiar en cualquier momento. Por ejemplo, si una tarea completada aún requiere trabajo, el propietario puede agregar un "siguiente paso" y devolver el estado a *En progreso*.

---

## **Notificaciones**

Todos los participantes de la tarea reciben notificaciones de CRM y correo electrónico sobre:

- creación de tarea
- finalización de tarea
- mensajes de chat
- asignaciones:

    - copropietario de tarea
    - suscriptor de tarea

---

## **Chat de Tarea**

Cada tarea tiene un chat integrado para intercambiar mensajes y archivos.

- Los suscriptores también pueden unirse a discusiones sobre el progreso de la tarea.
- Para comenzar, haga clic en "**Mensaje +**", elija destinatarios y envíe su primer mensaje. Después, aparecerá un botón "**Chat**" para ver toda la conversación.

---

## **Etiquetas**

Puede crear etiquetas personalizadas para agrupar y hacer seguimiento de tareas.

- Ejemplo: Agregue una etiqueta "Reunión de producción" a todas las tareas que desee discutir en la próxima reunión.
- Las tareas se pueden filtrar por etiquetas.

---

## **Trabajar con Tarea de Equipo**

- El **usuario responsable** debe crear una subtarea para sí mismo. Todos los demás ejecutores de la tarea principal se agregarán como suscriptores.
- La subtarea copia el título y descripción de la tarea principal. El ejecutor debe ajustar estos detalles para aclarar su trabajo específico.
- Si el usuario responsable simplemente hace clic en **Hecho**, se creará automáticamente una subtarea completada y la tarea principal desaparecerá de su lista.
- Los ejecutores también pueden crear subtareas entre sí.
- Cuando se crea la primera subtarea, la tarea principal cambia automáticamente al estado "En progreso".
- La tarea principal se marca como hecha cuando todos los ejecutantes tienen al menos una subtarea completada y
no hay subtareas pendientes o en progreso.

---

✅ Con estas herramientas, Django CRM facilita la organización del trabajo, el seguimiento del progreso y la colaboración en tareas en todo su equipo.

---

---
title: Gestión de proyectos
description: Descripción general de la página Lista de proyectos en Django CRM, incluida la creación de proyectos, el filtrado, la ordenación, los roles de usuario y las etapas.
---

# **Gestión de proyectos**

La página **Lista de proyectos** de [Django CRM](../index.md) permite a los usuarios ver, filtrar y gestionar todos los proyectos creados en el sistema.
Un proyecto en el CRM es un grupo de [tareas](task-management.md) relacionadas y sus subtareas que, en conjunto, representan un objetivo o una actividad específicos.
Los proyectos ayudan a estructurar el trabajo, supervisar el progreso y coordinar las actividades entre los miembros del equipo.

Cualquier usuario del CRM puede crear y gestionar proyectos. Cada proyecto tiene los mismos atributos y funciones que una tarea:
puedes añadirle tareas, realizar un seguimiento de su finalización y supervisar el progreso general del proyecto en tiempo real.

---

## **Creación de proyectos**

Hay varias formas de crear un proyecto en Django CRM:

- **Creación directa**: haz clic en **Añadir proyecto** y completa el [formulario del proyecto](creating-assigning-projects.md).
- **Desde un memo**: crea un proyecto directamente a partir de una [nota de CRM](../features/tasks-app-features.md#enhance-your-workflow-with-memos-crm-notes) existente; el formulario se completará automáticamente con los datos del memo.
- **Desde una tarea**: convierte una tarea en un proyecto; el formulario del proyecto heredará los detalles de la tarea.

Estas opciones facilitan iniciar un proyecto a partir de registros de CRM existentes.

---

## **Filtrado de proyectos**

La página Lista de proyectos incluye un panel de filtros que permite limitar los proyectos visibles. Puedes filtrar por:

- **Propietario o copropietario**
- **Responsable** (usuario asignado)
- **Estado**: proyectos activos o inactivos (cerrados)
- **Fecha de creación**

Los filtros ayudan a encontrar rápidamente los proyectos relevantes sin tener que buscar manualmente en toda la lista.

---

## **Ordenación de proyectos**

Los proyectos se muestran en una tabla estructurada con columnas ordenables. Las columnas principales incluyen:

- **Nombre del proyecto**
- **Siguiente paso**: qué debe hacerse a continuación
- **Fecha del siguiente paso**: cuándo debe completarse
- **Fecha de finalización**: plazo general del proyecto
- **Prioridad**: alta, media o baja
- **Etapa**: pendiente, en progreso, completado, pospuesto o cancelado
- **Propietarios**: creadores del proyecto
- **Estado de actividad**: activo o inactivo
- **Fecha de finalización del proyecto**
- **ID del proyecto**

La mayoría de los encabezados de columna son interactivos y permiten ordenar los proyectos según parámetros específicos. Algunos campos utilizan iconos: pasa el cursor sobre un icono para ver una descripción de su significado.

---

## **Roles de usuario en los proyectos**

Cada proyecto de Django CRM incluye roles de usuario específicos:

- **Propietarios y copropietarios del proyecto**: usuarios que crean y gestionan los proyectos.
- **Usuarios responsables**: ejecutores o usuarios asignados para llevar a cabo el proyecto.
- **Suscriptores**: usuarios que reciben notificaciones sobre el progreso del proyecto.

Los proyectos solo son visibles para los usuarios que participan en ellos en alguno de estos roles, lo que garantiza la privacidad y la relevancia de los datos.

---

## **Etapas de los proyectos**

Las etapas de los proyectos en Django CRM ayudan a realizar un seguimiento del progreso y a mantener informados a todos los participantes. Las etapas disponibles son:

- **Pendiente**
- **En progreso**
- **Completado**
- **Pospuesto**
- **Cancelado**

Normalmente, el **usuario responsable** actualiza la etapa del proyecto, aunque los propietarios también pueden modificarla. En las tareas colectivas, las tres primeras etapas (pendiente, en progreso y completado) se establecen automáticamente. Las etapas se pueden actualizar en cualquier momento; por ejemplo, si un proyecto marcado como “completado” todavía requiere alguna acción, el propietario puede especificar un nuevo “siguiente paso” y cambiar la etapa de nuevo a “en progreso”.

---

### **Temas relacionados**

* [Gestión de tareas en Django CRM](../features/tasks-app-features.md)
* [Creación y asignación de tareas](creating-assigning-tasks.md)
* [Notas de CRM: trabajo con memos](notes-crm.md)

---

**Notas de CRM**: Django CRM proporciona herramientas integradas para gestionar proyectos, tareas y memos, ayudando a los equipos a organizar el trabajo de forma eficiente y a mantener el control total sobre las actividades en curso.

---

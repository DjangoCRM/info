---
title: Edición y actualización de tareas en el CRM
description: Aprende a editar y actualizar tareas en el CRM para mejorar la productividad y la colaboración del equipo.
---

# **Edición y actualización de tareas**

El formulario de edición de tareas de Django CRM te ayuda a actualizar los detalles de las tareas, realizar un seguimiento del progreso y colaborar con tus compañeros.
Puedes cambiar la etapa de la tarea, definir el siguiente paso con una fecha límite, configurar recordatorios y consultar el historial del flujo de trabajo.
Las opciones adicionales, como crear subtareas, chatear con los participantes, copiar tareas o consultar su historial, hacen que la gestión de tareas sea flexible y transparente tanto para usuarios individuales como para equipos.
A continuación se explican los nuevos campos y botones disponibles en el formulario de edición de tareas.
Para obtener una visión general de la organización de las tareas, consulta la sección [Gestión de tareas del CRM](../features/tasks-app-features.md).

---

## **Campos adicionales del formulario de edición de tareas**

- **Etapa**  
	Define el estado actual de la tarea. Los valores disponibles son:

		- **Pendiente** *(valor predeterminado)*: la tarea se ha creado, pero aún no se ha iniciado.
		- **En progreso**: la tarea se está realizando activamente.
		- **Completada**: la tarea ha finalizado.
		- **Pospuesta**: la tarea se ha retrasado para más adelante.
		- **Cancelada**: la tarea no se completará.

- **Siguiente paso**  
	Especifica la próxima acción necesaria para la tarea.
	El valor introducido aquí también se muestra en la lista de tareas del usuario, para ayudar a los participantes a saber qué deben hacer a continuación.

- **Fecha del siguiente paso**  
	Define la fecha prevista para el siguiente paso. Esta fecha se muestra en la lista de tareas para que los usuarios puedan consultar los próximos plazos.

- **Recordármelo** *(casilla de verificación)*  
	Cuando se activa, el CRM crea automáticamente un recordatorio y se lo envía al usuario en la **fecha del siguiente paso**.

- **Ocultar la tarea principal** *(casilla de verificación en las subtareas)*
	Permite ocultar la tarea principal en el [gestor de tareas del CRM](task-management.md) antes de que todos los responsables la completen.

- **Flujo de trabajo**  
	El CRM completa este campo automáticamente cada vez que cambia el campo **Siguiente paso**.
	Registra qué acciones se realizaron y cuándo, formando un historial del progreso de la tarea.

Los demás campos se describen detalladamente en la sección [Crear una nueva tarea](creating-assigning-tasks.md).

---

## **Nuevos botones del formulario de edición de tareas**

- **Crear subtarea**  
	Permite crear una subtarea vinculada a la tarea actual.

- **Añadir mensaje al chat de esta tarea**  
	Abre el chat de la tarea, donde todos sus participantes, responsables y operadores (si están asignados)
	pueden intercambiar mensajes y archivos. Cada tarea y subtarea tiene su propio chat independiente.

- **Chat**  
	Aparece cuando hay al menos un mensaje en el chat de la tarea. Úsalo para consultar todo el historial de la conversación y responder.
	Las tareas con mensajes de chat se marcan con un icono en el [gestor de tareas](task-management.md).
	El icono cambia de color cuando tienes mensajes sin leer en el chat.

- **Subtareas** *(con contador)*  
	Muestra una lista de todas las subtareas asociadas a la tarea principal, accesible para todos los participantes.

- **Ver tarea principal** *(en las subtareas)*  
	Aparece en el formulario de edición de una subtarea. Haz clic para volver a la tarea principal.

- **Copiar**  
	Crea una nueva tarea basada en la actual. El formulario de creación de tareas se abrirá con todos los campos rellenados con los datos
	de la tarea existente, que podrás ajustar antes de guardarla.

- **Crear recordatorio**  
	Permite a cualquier participante crear un recordatorio personal para la tarea. El botón cambia de color cuando existe al menos un recordatorio.

- **Historial**  
	Abre el registro del historial de la tarea, que muestra todos los cambios realizados, quién los realizó y cuándo.

---

## **Botón especial para tareas de equipo**

- **Completada**  
	Aparece en las tareas asignadas a un equipo. Al hacer clic, el CRM crea automáticamente una subtarea para el usuario
	y la marca inmediatamente como completada. Todos los miembros del equipo reciben una notificación de esta acción.

---

## **Resumen**

Al actualizar tareas en el [CRM con gestión de tareas](../features/tasks-app-features.md), los usuarios pueden establecer etapas claras, definir siguientes pasos con fechas límite,
utilizar recordatorios y comunicarse directamente en los chats de las tareas. Los botones adicionales facilitan la gestión de subtareas,
el seguimiento del historial y la copia de tareas existentes.
Esto garantiza que el trabajo en equipo sea transparente y esté organizado durante todas las etapas de ejecución de las tareas.

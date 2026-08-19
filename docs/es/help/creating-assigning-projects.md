---
title: Creación y asignación de proyectos
description: Aprende a crear y asignar proyectos en Django CRM, incluyendo la configuración de prioridades, fechas límite y usuarios responsables.
---

# **Creación de un proyecto en el CRM**

Al trabajar con proyectos en [**Django CRM**](../index.md), los usuarios pueden crear fácilmente nuevos proyectos
y asignar responsabilidades, prioridades y fechas límite. Cada proyecto agrupa las [tareas](task-management.md) relacionadas
y proporciona una forma estructurada de gestionar los flujos de trabajo entre departamentos o equipos.

---

## **Campos del formulario de creación de proyectos**

Cada campo del formulario ayuda a definir cómo se [gestionará](project-management.md) el proyecto y quién participará en él:

- **Nombre** — Introduce el título del proyecto.
	Este es un campo obligatorio y aparecerá en la lista de proyectos.

- **Fecha límite** *(opcional)* — Establece una fecha de finalización para el proyecto.
	Puedes seleccionar la fecha directamente en el calendario integrado.

- **Prioridad** — Elige el nivel de prioridad del proyecto:
	**Baja**, **Media** o **Alta**. El sistema sugiere **Media** de forma predeterminada.

- **Descripción** *(opcional)* — Añade una breve descripción del propósito,
	alcance u objetivos del proyecto.

- **Nota** *(opcional)* — Utiliza este campo para añadir comentarios adicionales u observaciones internas.

- **Responsables** — Especifica los usuarios responsables de ejecutar las tareas del proyecto.

- **Propietario** — El usuario que crea el proyecto se asigna automáticamente como su propietario.

- **Copropietario** *(opcional)* — Puedes añadir otro usuario como copropietario para compartir los derechos de gestión.

---

## **Secciones opcionales**

Debajo de los campos principales, el formulario contiene varias secciones desplegables
para configurar opciones adicionales:

- **Cambiar suscriptores** — Selecciona los usuarios que deben recibir notificaciones sobre las
	actualizaciones y el progreso del proyecto. Esto ayuda a mantener informados a los miembros relevantes del equipo
	sin asignarles tareas como ejecutores.

- **Añadir etiquetas** *(opcional)* — Las etiquetas facilitan la categorización de los proyectos y permiten
	filtrarlos rápidamente en la lista de proyectos.

- **Archivos** — Adjunta archivos directamente al proyecto. Pueden ser informes iniciales,
	especificaciones, informes o cualquier documentación de apoyo.

---

## **Guardar el proyecto**

Después de completar todos los campos obligatorios, haz clic en **Guardar** para crear el proyecto.
El nuevo proyecto aparecerá en tu **Lista de proyectos**. También puedes hacer clic en **Guardar y continuar**
para empezar a añadir tareas al proyecto.

> [Trabajar con tareas en Django CRM](../features/tasks-app-features.md)

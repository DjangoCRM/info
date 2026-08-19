---
title: Creación y asignación de tareas en el CRM
description: Aprende a crear, asignar y gestionar tareas en el CRM para mejorar la productividad y la colaboración del equipo.
---

# **Creación de una nueva tarea**

El formulario Nueva tarea de Django CRM te ayuda a crear y organizar tareas rápidamente con todos los detalles necesarios en un solo lugar.
Puedes establecer un título claro, añadir una fecha límite, asignar empleados responsables, definir la prioridad, adjuntar archivos
y notificar al equipo sobre el progreso. Las opciones flexibles, como los copropietarios, los suscriptores y las etiquetas,
facilitan la gestión de responsabilidades y mantienen informadas a las personas adecuadas.
A continuación se explica cada campo del formulario y su funcionamiento.

---

## **Detalles de la tarea**

- **Nombre**  
	Introduce el título de la tarea. Es un campo obligatorio y debe describir claramente su propósito.

- **Fecha límite** *(opcional)*  
	Si es necesario, selecciona una fecha límite mediante el calendario integrado.
	Puedes dejar este campo vacío si la tarea no tiene una fecha de finalización estricta.
	Si se produce un error al introducir la fecha manualmente, utiliza el calendario para consultar el formato correcto.

- **Prioridad**  
	Elige la importancia de la tarea:

		- **Baja**: trabajo no urgente o rutinario.
		- **Media**: prioridad estándar, seleccionada de forma predeterminada.
		- **Alta**: tarea urgente o crítica para la empresa.

- **Descripción** *(opcional)*  
	Añade información adicional sobre la tarea. Este campo puede utilizarse para explicar el alcance, los objetivos o los requisitos específicos.

- **Nota** *(opcional)*  
	Añade observaciones breves, comentarios internos o recordatorios relacionados con la tarea.

---

## **Asignación**

- **Responsables**  
	Son las personas que ejecutarán la tarea. De forma predeterminada, se te selecciona automáticamente.

		- Si eres responsable de un departamento, también puedes asignar la tarea a los miembros de tu equipo.
		- Si eres el responsable de la empresa, verás la lista completa de empleados añadidos al CRM.

- **Propietario**  
	Se te asigna automáticamente como propietario de la tarea. Este campo no se puede cambiar.

	- **Copropietario** *(opcional)*  
		Asigna un copropietario a la tarea. Esta persona compartirá la responsabilidad de supervisar el progreso y la finalización de la tarea.
		El copropietario tendrá permiso para modificarla.
		El sistema sugerirá automáticamente un copropietario:

		- Si eres un empleado común, se propondrá al responsable de tu departamento.
		- Si eres responsable de un departamento, se propondrá al responsable de la empresa.
		- Si eres el responsable de la empresa, no se sugerirá ningún copropietario.

	Puedes dejar este campo vacío si no deseas asignar un copropietario.

	- **Cambiar suscriptores** *(sección desplegable)*  
		Selecciona los usuarios que deben recibir notificaciones sobre la tarea y su progreso.
		Los suscriptores no realizan el trabajo, pero se mantienen informados sobre las actualizaciones y los resultados.
		Al crear una subtarea, el sistema selecciona automáticamente a los demás responsables de la tarea principal.
		Puedes eliminar a cualquiera de ellos si es necesario.

- **Añadir etiquetas** *(sección desplegable)*  
	Asigna una o más etiquetas a la tarea para facilitar su categorización y búsqueda posterior.

---

## **Archivos adjuntos**

- **Archivos**  
	Sube y adjunta archivos a la tarea. Pueden ser documentos, hojas de cálculo u otros materiales útiles para completarla.

---

## **Notificaciones y acceso**

Después de guardar una tarea, todos los usuarios seleccionados recibirán una notificación adecuada a su función.
La tarea estará disponible en su [gestor de tareas](task-management.md).
Los demás usuarios, excepto tus responsables y los administradores, no tendrán acceso a ella.

---

## **Recursos adicionales**

Para obtener más información sobre las funciones de gestión de tareas y las prácticas recomendadas, consulta los siguientes recursos:
- [Funciones de gestión de tareas](../features/tasks-app-features.md)
- Gestión de proyectos
- Memos en el CRM

---

## **Resumen**

Al completar el formulario **Nueva tarea**, puedes establecer fechas límite, asignar responsables, notificar a los compañeros adecuados
y proporcionar toda la información necesaria en un solo lugar. Esto garantiza que las tareas estén bien estructuradas
y que su progreso pueda seguirse eficazmente en el CRM.
El resultado es una mejor colaboración del equipo y una mayor productividad.

---
title: Gestión de transacciones
description: Aprende a gestionar transacciones en Django CRM, incluida su creación, los permisos de acceso, la vista general de la lista, la búsqueda, el filtrado y la exportación de datos.
---

# **Gestión de transacciones**

La **transacción** es el objeto principal del [CRM](../index.md) que utilizan los gerentes de ventas para realizar un seguimiento del trabajo comercial con clientes potenciales y actuales.
Almacena todo el historial de comunicación, negociación y toma de decisiones, desde la [solicitud](request-processing.md) inicial hasta el cierre exitoso (o el rechazo) de la transacción.

Esta página explica cómo trabajar con la lista de transacciones y utilizar las herramientas disponibles para organizar y analizar las actividades de ventas.

---

## **Creación de transacciones y permisos de acceso**

Para fines de análisis de marketing, una transacción solo se puede crear **a partir de una solicitud** recibida mediante un formulario del sitio web, un correo electrónico o creada manualmente en el CRM.

➡ Nota: los productos o servicios especificados en la solicitud pueden diferir de aquellos para los que finalmente se cierra la transacción.

El acceso a las transacciones está regulado por los roles de usuario y los departamentos:

| Rol | Nivel de acceso |
| --- | --- |
| Gerente de ventas | *Transacciones de su departamento* |
| Directivos de la empresa | *Todas las transacciones de todos los departamentos* |
| Otros usuarios | *No tienen acceso a las transacciones* |

En equipos de pequeñas empresas, el CRM permite combinar roles: operador, gerente de ventas e incluso gerente de la empresa.
Si necesitas cambiar roles o configurar permisos personalizados, ponte en contacto con tu **administrador del CRM**.

---

## **Vista general de la lista de transacciones**

La lista de transacciones se muestra como una tabla ordenable con encabezados de columna activos. Las columnas incluyen:

- **Nombre de la transacción**: se hereda de la solicitud, pero se puede editar.
- **Siguiente paso**: la próxima acción que debe realizarse.
- **Fecha del siguiente paso**: fecha límite de la acción planificada.
- **Etapa**: estado actual del progreso.
- **Nombre de la contraparte (prospecto o empresa)**: enlace a la página de la contraparte.
- **Contador**: número de transacciones de esta contraparte en la base de datos del CRM.
- **Gerente de ventas**: usuario responsable asignado.
- **Activa**: indica si la transacción se está gestionando actualmente.
- **Indicador de relevancia de la transacción**.
- **Fecha de creación**.
- **ID de la transacción**.

---

## **Iconos de estado de las transacciones**

Los iconos proporcionan información rápida sobre las condiciones de la transacción:

- Todavía no se ha enviado ninguna respuesta a la solicitud del cliente.
- Se ha recibido el pago.
- No hay productos ni servicios indicados en la transacción.
- Se ha recibido el pago, pero no se ha especificado la fecha de envío o prestación del servicio.
- La fecha límite de envío o prestación del servicio ha vencido.
- Hay archivos adjuntos a la transacción.

Pasa el cursor sobre cualquier icono para ver una descripción emergente con más información.

---

## **Búsqueda y filtrado de transacciones**

### Búsqueda

Utiliza la **barra de búsqueda** para encontrar transacciones por:

- Palabras clave
- ID de la transacción

### Filtros

Un **panel de filtros** permite reducir dinámicamente la lista. Entre los filtros disponibles se incluyen:

- Departamento (si el rol permite seleccionarlo)
- Nivel de importancia
- Gerente de ventas (propietario)
- Producto o servicio
- Socio (representante de ventas)
- Modificada por la dirección de la empresa
- Indicador de relevancia
- Fecha de creación
- Etapa de la transacción
- Motivo del cierre
- Sector del cliente
- Etiquetas

Los filtros se pueden combinar para ajustar aún más los resultados.
De forma predeterminada, en la lista solo se muestran las transacciones activas.

---

## **Exportación de datos de transacciones**

Con el menú desplegable **«Acción»**, puedes exportar las transacciones seleccionadas a un **archivo de Excel**.
Esto resulta especialmente útil para compartir datos o conciliarlos con socios comerciales.

---

## Temas relacionados

- [Trabajo con transacciones](working-with-deals.md)
- [Gestión de solicitudes comerciales](commercial-requests-management.md)
- [Descripción general del software CRM](../features/overview.md)

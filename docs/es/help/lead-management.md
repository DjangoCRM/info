---
title: Gestión de Leads
description: Aprende cómo gestionar leads en Django CRM, incluyendo creación de leads, permisos de acceso, descripción general de la lista de leads, búsqueda, filtrado, acciones en lote y exportación de datos.
---

# **Gestión de Leads**

El objeto **Lead** en Django [CRM](../index.md) representa un cliente potencial.
Un lead puede ser un individuo o un perfil de empresa/contacto parcialmente completado
que aún no se ha convertido en Empresa y Persona de Contacto.
La gestión efectiva de leads asegura que los equipos de ventas puedan calificar prospectos,
enriquecer sus datos y convertir leads relevantes en empresas y contactos.

Esta página explica cómo ver, gestionar, filtrar, ordenar y convertir leads dentro de Django CRM.

---

## **¿Qué es un Lead?**

Un lead contiene información básica sobre un cliente potencial. Los datos pueden provenir de:

- Solicitudes del sitio web
- Envíos de formularios
- Entradas agregadas manualmente
- Leads creados automáticamente cuando un gerente de ventas crea un **Trato**

Si se recibe información faltante sobre una empresa y persona de contacto durante el procesamiento de una solicitud de ventas,
el Lead puede ser convertido en objetos de Empresa y Persona de Contacto.

> Para obtener detalles sobre cómo trabajar con solicitudes, consulte
**[Gestión de Solicitudes Comerciales](../features/crm-app-features.md#commercial-requests-management)**.

---

## **Agregando Leads al CRM**

Los leads pueden ingresar al CRM de varias formas:

### 1. Creación Automática de Leads

Cuando se crea un trato a partir de una consulta entrante y el CRM
detecta datos de cliente insuficientes, se crea un Lead automáticamente.

### 2. Agregando un Lead Manualmente

Los usuarios pueden agregar leads manualmente:

- Haga clic en **Agregar Lead**.
- Complete los campos del formulario y guarde.

### 3. Importando Leads desde Excel

Puede cargar múltiples leads a la vez:

1. Haga clic en **Importar**.
2. Seleccione un archivo Excel preparado según el formato de importación del CRM.
3. Confirme la carga.

Para obtener opciones de exportación, consulte la sección **Exportando Leads** [abajo](#exporting-leads).

---

## **Permisos de Acceso**

La visibilidad del lead depende del rol del usuario en CRM y del departamento:

- **Gerentes de Ventas** y **Operadores** — pueden ver y gestionar leads asignados a *su propio departamento*.
- **Gerentes de Empresa** y **Super Operadores** — tienen acceso a *todos los leads en todos los departamentos*.

---

## **Tabla de Lista de Leads**

Los leads se muestran en una tabla ordenable. Cada encabezado de columna está activo, permitiéndole ordenar leads por el campo seleccionado.

### Columnas de la Tabla

- Nombre del Lead / Nombre Completo
- Dirección de Email
- Nombre de la Empresa (*si existe*)
- Gerente de Ventas Asignado
- País
- Estado de Boletín
- Fecha Agregada

### Iconos de Estado del Boletín

La posición del lead en su actividad de envío se indica por el color del icono del buzón:

- **Rojo** — El lead aún no ha recibido ningún boletín.
- **Turquesa** — El lead recibe boletines y no se ha desuscrito.
- **Gris** — El lead recibió boletines pero se desuscribió.

---

## **Buscando Leads**

Use la barra de búsqueda para encontrar leads por:

- Nombre
- Email
- Empresa
- Cualquier palabra clave
- ID del Lead

---

## **Filtrando Leads**

El CRM proporciona varios filtros para reducir la lista de leads:

- Estado de descalificación
- Gerente de ventas asignado
- País
- Estado de suscripción al boletín
- Estado VIP

Los filtros se pueden combinar para obtener resultados más precisos.

---

## **Acciones en Lote (*Menú de Acciones*)**

Seleccione uno o más leads para realizar operaciones en lote desde el menú desplegable **Acción**:

- Crear Envío Masivo
- Establecer Estado VIP
- Remover Estado VIP
- Exportar a Excel

Estas acciones ayudan a gestionar listas grandes de leads de manera eficiente.

---

## **Exportando Leads**

Puede exportar datos de leads en formato Excel:

### Exportar Leads Seleccionados

Elija leads usando las casillas de verificación de la tabla, luego seleccione **Exportar a Excel** del menú Acción.

### Exportar Todos los Leads

Use el botón **Exportar Todo** para descargar la base de datos completa de leads.

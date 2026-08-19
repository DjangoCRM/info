---
title: Gestión de Contactos Empresariales
description: Aprende cómo gestionar contactos empresariales en Django CRM, incluyendo creación de contactos, permisos de acceso,
  descripción general de la lista, búsqueda, filtrado, acciones masivas y exportación de datos.
---

# **Gestión de Contactos Empresariales en Django CRM**

La gestión de contactos empresariales es una de las características principales de [CRM](../index.md). La sección **Contactos** en CRM permite a los usuarios almacenar, organizar y trabajar con información sobre empleados y representantes de empresas cliente. Esta guía explica cómo aparecen los contactos en CRM, cómo gestionarlos, cómo utilizar filtros y acciones masivas, y cómo entender los estados de los contactos.

> Para temas relacionados, consulta **[Gestión de Empresas](company-management.md)**

---

## **¿Qué Representa un Contacto?**

Un **Contacto** es una persona individual — un empleado o representante de una empresa cliente. Los registros de contactos almacenan detalles clave de comunicación y se utilizan para procesos de ventas, soporte y campañas de correo electrónico masivo.
Cada contacto está vinculado a una empresa, asignado a un gerente de ventas e incluido en boletines o envíos masivos.

---

## **Cómo Se Agregan Contactos a CRM**

Django CRM admite varios métodos para agregar contactos al sistema:

### 1. Creación automática

Los contactos se pueden crear automáticamente cuando un usuario crea un **negocio**, basándose en datos de solicitud de ventas.

### 2. Creación manual

Los usuarios pueden agregar manualmente nuevos contactos:

1. Haz clic en **Agregar Contacto**.
2. Completa el formulario con la información personal y empresarial requerida.
3. Guarda el contacto.

### 3. Importación desde Excel

Si necesitas cargar contactos en masa:

1. Haz clic en el botón **Importar**.
2. Selecciona un archivo de Excel preparado según el formato de importación de CRM.
3. Cárgalo para agregar los contactos al sistema.

### 4. Conversión desde Lead

Cuando un **Lead** se convierte en una empresa y contacto, CRM crea automáticamente un registro de **Contacto**.

> Más información: **[Gestión de Leads](lead-management.md)**

---

## **Acceso del Usuario a Contactos**

El acceso a la base de datos de contactos depende del rol y departamento del usuario:

- **Gerentes de ventas y operadores**  —  acceden solo a los contactos pertenecientes a su propio departamento.

- **Gerentes de empresa y superoperadores**  — acceden a todos los contactos en todos los departamentos.

Esto asegura que los datos sensibles estén disponibles solo para miembros autorizados del equipo dentro de la organización.

---

## **Trabajar con la Lista de Contactos**

La lista de contactos aparece en una **tabla ordenable**, permitiendo a los usuarios organizar y localizar rápidamente la información necesaria. Al hacer clic en un encabezado de columna activo, se ordenarán los contactos por ese campo.

### Columnas de la Tabla

La tabla incluye los siguientes campos:

- Nombre del contacto
- Correo electrónico
- Número de teléfono
- Nombre de la empresa
- País
- Estado como destinatario del boletín
- Fecha de adición a CRM
- Gerente de ventas asignado

La clasificación y los datos estructurados mejoran la velocidad y eficiencia al trabajar con bases de datos de clientes grandes.

---

## **Indicadores de Estado de Suscripción del Boletín**

Al lado de cada contacto, un icono de buzón indica su estado de suscripción al boletín:

- **Rojo** — El contacto **aún no ha recibido ningún boletín**.
- **Turquesa** — El contacto **recibe boletines** y **no se ha dado de baja**.
- **Gris** — El contacto **ha recibido boletines** pero **se ha dado de baja**.

Estos marcadores visuales ayudan a identificar preferencias de correo de un vistazo.

---

## **Búsqueda y Filtrado de Contactos**

### Barra de búsqueda

Utiliza la barra de búsqueda para encontrar contactos por:

- Palabras clave (nombre, correo electrónico, empresa, etc.)
- ID de contacto

### Filtros disponibles

Puedes filtrar la lista de contactos por:

- Departamento (si el rol del usuario lo permite)
- Gerente de ventas asignado
- Industria de la empresa
- Tipo de empresa
- País
- Estado de suscripción al boletín
- Estado VIP
- Etiquetas

Estos filtros permiten una segmentación precisa para análisis de ventas y campañas de marketing.

---

## **Acciones Masivas para Contactos**

El menú desplegable **Acción** permite a los usuarios realizar operaciones masivas en contactos seleccionados:

- Crear un **envío masivo**
- Establecer estado **VIP**
- Eliminar estado **VIP**
- **Exportar** contactos seleccionados a Excel

Nota: Los usuarios pueden exportar solo los contactos asignados a ellos.

---

## **Opciones de Envío Masivo**

Hay dos formas de crear campañas de correo electrónico masivas desde la página de Contactos:

-  **1. Envío masivo para contactos seleccionados**

Utiliza la opción **Acción → Hacer envío masivo**.

- **2. Envío masivo para grupos grandes**

Utiliza el botón **Hacer envío masivo** en la parte superior para iniciar una campaña para muchos contactos a la vez.

---

## **Exportación de Contactos**

Puedes exportar datos de contactos de dos formas:

### Exportar contactos seleccionados

Utiliza la opción **Acción → Exportar**.
Los usuarios pueden exportar solo los contactos de los que son responsables.

### Exportar todos los contactos

Para descargar la lista completa (los usuarios solo pueden exportar contactos asignados a ellos), utiliza el botón **Exportar Todo**.

---

> Lectura recomendada: [Características de la aplicación CRM](../features/crm-app-features.md)  
> Para más información sobre envíos, consulta [Campañas de Correo Electrónico y Boletines](../features/massmail-app-features.md)

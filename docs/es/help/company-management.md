---
title: Gestión de Empresas
description: Aprende a gestionar empresas en Django CRM, incluida la creación de empresas, los permisos de acceso, la vista general de la lista, la búsqueda, el filtrado, las acciones masivas y la exportación de datos.
---

# **Gestión de Empresas en Django CRM**

El objeto **Empresa** del [CRM](../index.md) almacena información sobre empresas clientes existentes o potenciales.
Los datos precisos de las empresas son esenciales para las operaciones de ventas, la segmentación y las campañas de marketing.
Esta guía explica cómo crear empresas, importar sus datos, asignar gerentes
y filtrar la lista de empresas para trabajar de forma eficiente en ventas y marketing.

---

## **¿Qué es el objeto Empresa en Django CRM?**

Un registro de Empresa representa a un cliente o cliente potencial. Incluye datos empresariales importantes, como el nombre,
la dirección, los datos de contacto, el tipo, el número de registro, el gerente de ventas asignado, el estado de suscripción al boletín y el sector.
Mantener perfiles de empresa precisos ayuda a los equipos de ventas a segmentar los mercados y gestionar el embudo de ventas.

---

## **Cómo se añaden empresas al CRM**

Django CRM permite crear o importar empresas de varias formas:

### 1. Automáticamente al crear una transacción

Si la solicitud contiene información sobre una empresa y esta no se encuentra en el CRM,
al crear una [transacción](deals-management.md) también se creará automáticamente el registro de Empresa.

### 2. Creación manual

Puedes añadir una empresa manualmente haciendo clic en **Añadir empresa** y completando el formulario.
Antes de crear una empresa, comprueba si ya existe un **Cliente potencial** con el mismo nombre.

> Consulta también:  
> [Gestión de contactos de empresas](contact-management.md)  
> [Gestión de clientes potenciales en el CRM](lead-management.md).

### 3. Importación desde Excel

Para añadir varias empresas a la vez:

1. Haz clic en **Importar**.
2. Selecciona un archivo de Excel preparado según el formato de importación del CRM.
3. Súbelo para crear o actualizar los registros de empresas.

### 4. Conversión de un cliente potencial

Al convertir un cliente potencial en cliente, el CRM puede crear automáticamente el registro de Empresa correspondiente.

---

## **Permisos de acceso a las empresas**

El acceso a los registros de empresas depende de los roles de usuario y los departamentos:

- Los **gerentes de ventas** y los **operadores** solo ven las empresas de su propio departamento.
- Los **gerentes de empresa** y los **súper operadores** tienen acceso a las empresas de todos los departamentos.

Si no ves la empresa que esperabas, ponte en contacto con el administrador del CRM para revisar tus permisos.

---

## **Vista de la lista de empresas y campos de la tabla**

Todas las empresas se muestran en una tabla ordenable. La mayoría de los encabezados de columna permiten ordenar en sentido ascendente o descendente.

### **Columnas de la tabla**

- **Nombre de la empresa**
- **Tipo de empresa** *(distribuidor, concesionario, revendedor, cliente final, competidor)*
- **Fecha de incorporación**
- **Gerente de ventas asignado**
- **País**
- **Estado de destinatario del boletín**
- **ID de la empresa**
- **Número de registro**

Estos conjuntos de tipos y sectores se pueden adaptar a las necesidades específicas de tu empresa.
Ponte en contacto con el administrador del CRM si necesitas personalizarlos.

---

## **Indicadores del estado del boletín**

El estado de suscripción al boletín se muestra mediante un icono de buzón de color:

- **Rojo**: la empresa todavía no ha recibido ningún boletín.
- **Turquesa**: la empresa ha recibido boletines y no se ha dado de baja.
- **Gris**: la empresa se ha dado de baja de los boletines.

---

## **Búsqueda de empresas**

Utiliza la barra de búsqueda para encontrar empresas por:

- Nombre de la empresa
- Palabras clave
- ID de la empresa

Los resultados de búsqueda se actualizan al instante según lo que escribas.

---

## **Filtros para gestionar la base de datos de empresas**

Utiliza el panel de filtros para limitar la lista por:

- Departamento (según tu rol)
- Existencia de personas de contacto vinculadas
- Gerente de ventas asignado
- Fecha de la última actualización
- Sector
- Tipo de empresa
- País
- Estado de suscripción al boletín
- Estado VIP
- Etiquetas

Estos filtros te ayudan a segmentar empresas para marketing, seguimiento de ventas o elaboración de informes.

---

## **Acciones masivas**

Selecciona una o varias empresas y utiliza el menú desplegable **Acción** para realizar acciones en grupo:

- **Crear envío masivo** (campañas de correo electrónico)
- **Establecer o eliminar el estado VIP**
- **Exportar las empresas seleccionadas a Excel**
- **Reasignar empresas a otro gerente de ventas** (si el rol lo permite)

Los administradores también pueden transferir las empresas seleccionadas a otro gerente desde este menú.

Para transferir una sola empresa junto con sus contactos, cambia el campo **Propietario** en la página de la empresa.

---

## **Creación de envíos masivos**

Hay dos formas de iniciar un envío masivo:

- Desde el menú **Acción** (para empresas seleccionadas)
- Mediante el botón **Crear envío masivo** (para un grupo grande)

---

## **Exportación de empresas**

Puedes exportar los datos de las empresas mediante:

- **Exportar** (para las filas seleccionadas)
- **Exportar todo**: exporta toda la base de datos de empresas a Excel

Los usuarios solo pueden exportar las empresas que tienen asignadas.

---

## Temas relacionados

- [Gestión de solicitudes comerciales en el CRM](commercial-requests-management.md)  
- [Marketing por correo electrónico del CRM](../features/massmail-app-features.md)

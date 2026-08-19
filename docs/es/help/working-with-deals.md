---
title: Trabajar con Acuerdos en Django CRM
description: Aprenda cómo gestionar efectivamente acuerdos en Django CRM, incluida la comprensión del diseño de la página de acuerdos,
  el uso de acciones de interfaz y la utilización de datos de acuerdos para análisis de ventas e informes.
---

# **Trabajar con Acuerdos en Django CRM**

La página de Acuerdos en CRM es su espacio de trabajo central para gestionar todo el proceso de ventas —
desde la consulta inicial hasta el pago final. Esta página recopila información clave del cliente, historial de comunicación,
pasos de flujo de trabajo y datos financieros para ayudar a los equipos de ventas a trabajar eficientemente y mantener toda la información relacionada con acuerdos organizada.

A continuación se muestra una descripción detallada de cada sección y función disponible en la página de Acuerdos.

---

## **Acciones de Interfaz y Comportamiento del Sistema**

### Acciones de Botones Grises

**(No guardan ni modifican datos del acuerdo)**  
Algunos botones en la página de Acuerdos están diseñados para crear objetos relacionados sin alterar el acuerdo en sí:

- **Nota de Oficina** – Crea una nota interna vinculada al acuerdo actual. Cada nota incluye un atajo para usuarios con acceso para abrir rápidamente el acuerdo.
- **Mensaje** – Abre un formulario de mensaje de chat.

  - Si el chat ya contiene mensajes, aparece un botón *Ver chat*.
  - Si hay mensajes no leídos, el botón se vuelve **rojo**.

### Sincronización de Correo Electrónico

CRM sincroniza automáticamente el buzón del vendedor asignado utilizando tickets de acuerdos incrustados en correos electrónicos.  
En la parte inferior de la página de acuerdos, verá los **cuatro correos electrónicos más recientes**.
Use el **icono de dos sobres** para ver la lista completa de correspondencia de correo electrónico.  
Si un correo electrónico entrante no incluía un ticket de acuerdo, puede adjuntarlo manualmente usando el botón **Importar**.

### Herramientas Adicionales

- **Acuerdos** – Muestra el número de acuerdos asociados con el mismo cliente. Hacer clic abre la lista completa.
- **Recordatorio (icono de reloj)** – Crea un recordatorio relacionado con este acuerdo. Todos los recordatorios se pueden ver en la sección **Común**.
- **Historial** – Muestra el registro de auditoría completo: quién cambió qué, cuándo y cómo.

---

## **Sección 1: Información Principal**

Aquí puede gestionar los atributos básicos del acuerdo:

- **Nombre del acuerdo** – Editable en cualquier momento. Por defecto, heredado de la solicitud de origen.
- **Información de la solicitud** – Ver detalles clave de la solicitud. Haga clic en **Solicitud** para abrirla.
- **Bandera de importancia** – Resalte el acuerdo en el Administrador de Acuerdos y habilite el filtrado por importancia.
- **Cerrar el acuerdo** – Seleccione un motivo de cierre de la lista desplegable para cerrar el acuerdo.

*Tema relacionado* - [Gestionar Solicitudes](commercial-requests-management.md)

---

## **Sección 2: Información de Contacto**

Esta sección muestra con quién está trabajando y proporciona herramientas de comunicación rápida:

- **Contacto o Prospecto** – Ver a la persona involucrada en el acuerdo y navegar a su perfil.
- **Accesos directos de comunicación:**

  - Enviar un **correo electrónico**
  - Mensaje a través de **WhatsApp**
  - Mensaje a través de **Viber**
- **Sitio web de la empresa** – Abra el sitio web del cliente.
- **Perfil de la empresa** – Navegue a la página de la empresa del cliente.

*Temas relacionados:*

- [Gestionar Prospectos](lead-management.md)
- [Gestionar Contactos](contact-management.md)
- [Gestionar Empresas](company-management.md)

---

## **Sección 3: Progreso del Acuerdo y Flujo de Trabajo**

Esta sección apoya la gestión operativa del proceso de ventas:

### Gestión de Etapas

Seleccione la **etapa actual del acuerdo** de la lista predefinida. Estas etapas se utilizan para construir el informe del Embudo de Ventas.

### **Campos Financieros**

- **Cantidad total y moneda** – El valor general del acuerdo.
- Después de agregar pagos, CRM calcula automáticamente:

  - **Cantidad pagada**
  - **Cantidad esperada**

### Planificación del Próximo Paso

- **Próximo paso** – Describa brevemente la próxima acción.
- **Fecha del paso** – Seleccione la fecha límite.
- **Recordarme** – Crea automáticamente un recordatorio.

### Flujo de Trabajo e Historial

- **Flujo de trabajo** – Enumera las acciones completadas a medida que progresa el acuerdo.
- **Descripción** – Espacio para notas internas.
- **Fechas de etapa** – Lista de etapas completadas con fechas completadas automáticamente.

---

## **Sección 4: Datos Avanzados y Vínculos**

### Etiquetas

Adjunte etiquetas para categorizar y filtrar acuerdos de manera más eficiente.

### Conexiones de Acuerdos

El acuerdo muestra sus vínculos a:

- Persona de contacto y empresa (o prospecto)
- Representante del socio (si es aplicable)
- Solicitud

**Importante:**
Para un análisis de clientes preciso, siempre especifique el **cliente final** en los campos de contacto y empresa — incluso si la venta se realiza a través de un socio. Esto se puede ajustar más tarde si se conoce el cliente final.
Especificar un socio le permite ver todos los acuerdos con este socio en el administrador de Acuerdos usando el filtro de socio.

### Información Adicional

Esta área muestra:

- Propietario y copropietario del acuerdo (gerentes de ventas responsables)
- Información de última modificación (quién modificó por última vez el acuerdo y cuándo).
- Ticket de acuerdo

### Resultados (Productos / Servicios)

Aquí puede describir lo que está vendiendo:

- Cantidades y precios
- Fechas de contrato y envío real
- Números de serie (si es aplicable)
- Estado de envío

### Pagos

Agregue y realice un seguimiento de los detalles de pago:

- Monto del pago y moneda
- Fecha de pago real o esperada
- Estado del pago (recibido / garantizado / alta probabilidad / baja probabilidad)
- Números de contrato e factura
- Número de pedido
- Indicador de pagos a través de la oficina representante

### Archivos

Cargue contratos, especificaciones, facturas y otros archivos relacionados con acuerdos.

---

## **Por Qué los Datos de Acuerdos Precisos Son Importantes**

Django CRM utiliza información de acuerdos para generar poderosos informes de marketing y análisis:

### Informe de Motivos de Cierre

Ayuda a identificar por qué los acuerdos fracasan y revela patrones que impactan el desempeño de ventas.

### Informe del Embudo de Ventas

Basado en el campo **Etapa**. Muestra en qué etapa se pierden la mayoría de los acuerdos — por ejemplo, acuerdos que nunca progresaron más allá de la etapa de oferta de precio.

### Informe de Resumen de Ingresos

Utiliza estados de pago para construir pronósticos de ingresos para el mes actual y los próximos dos meses.

### Informe de Ventas

Muestra qué productos o servicios se vendieron, cuándo, por quién y a qué precio.

Si necesita actualizar valores preestablecidos para etapas de acuerdos o motivos de cierre, comuníquese con el administrador de CRM — estas listas se pueden personalizar para que coincidan con sus procesos comerciales.

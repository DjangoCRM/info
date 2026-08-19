---
title: Gestión de Mailings Masivos
description: Aprende a gestionar mailings masivos en el CRM de correo, incluyendo la creación de mailings, el seguimiento del progreso, la gestión de errores, la búsqueda, el filtrado y la combinación de mailings.
---

# **Gestión de Mailings Masivos en Django CRM**

El módulo de **Mailing masivo** de Django CRM ayuda a los equipos de ventas y marketing a gestionar [boletines](managing-newsletters.md) de empresas,
actualizaciones de productos y mensajes promocionales mediante las herramientas integradas del [**CRM de correo**](../index.md).
Esta sección explica cómo crear mailings, supervisar su progreso y optimizar las campañas de **mailing masivo**,
garantizando flujos de trabajo eficaces y conformes para el [**marketing por correo electrónico**](../features/massmail-app-features.md).

Los mailings masivos pueden enviarse a **empresas**, **contactos** o **leads**. Todos los destinatarios proceden directamente de la
base de datos del CRM, lo que garantiza una segmentación limpia y una selección precisa: elementos clave de un marketing por correo electrónico eficaz.

---

## **Funciones principales de la herramienta de Mailing Masivo del CRM**

El módulo de CRM de correo ofrece varias funciones integradas que permiten un envío eficaz y seguro:

- Los boletines se envían a través de las cuentas de correo electrónico de los gerentes de ventas.
- El sistema incluye un mecanismo integrado para cancelar la suscripción. Los destinatarios pueden **cancelar su suscripción** en cualquier momento.
- Las cuentas de correo electrónico están protegidas frente a los mecanismos de bloqueo de spam mediante límites de envío automáticos y reglas de programación.
- Cada cuenta de correo electrónico tiene un **límite de envío diario**, y los correos se envían **de forma uniforme durante el horario laboral**.
- Los mailings masivos se suspenden automáticamente los viernes, sábados y domingos.
- Las cuentas de correo electrónico principales de los gerentes de ventas envían boletines únicamente a **destinatarios VIP**, reduciendo el riesgo de spam.

Estas medidas protegen la reputación del remitente y mejoran el rendimiento general del marketing por correo electrónico.

Cada operación de mailing se guarda como un objeto Mailing, que contiene:

* Configuración inicial del mailing masivo
* Progreso del envío en curso
* Resultados finales cuando el mailing se completa

---

## **Creación de un nuevo Mailing Masivo**

Antes de crear un mailing, asegúrate de tener:

- Al menos **una cuenta de correo electrónico configurada** para enviar boletines.
- Una **plantilla de boletín** creada y lista para usar.
- Una **firma** de correo preparada (recomendado).

Puedes crear un nuevo mailing de varias formas:

1. En la página principal de **Mailing Masivo**, haciendo clic en **Crear Massmail**.
2. Desde las páginas de [**Lead**](lead-management.md), [**Empresa**](company-management.md)
   o [**Contacto**](contact-management.md); cada tipo de objeto tiene una opción para iniciar un Massmail.

Se crea un mailing independiente **para cada tipo de destinatario** (leads, empresas o contactos).
Los gerentes de ventas solo pueden crear mailings para los destinatarios que tienen asignados.

### Permisos de acceso

El acceso depende del rol y del departamento:

* Los **gerentes de ventas** solo ven los mailings de su propio departamento.
* Los **gerentes de empresa** ven los mailings de **todos** los departamentos.

<!-- Para obtener más información sobre los permisos, consulta: ➡️ *[Gestión de departamentos en el CRM](#)* ➡️ *[Roles de usuario y derechos de acceso](#)* -->

---

## **Descripción general de la lista de Mailings Masivos**

La lista de mailings masivos aparece en una tabla que se puede ordenar y filtrar, lo que permite a los equipos analizar rápidamente los datos de las campañas.

### Columnas de la tabla

- Nombre y vista previa del boletín
- Tipo de destinatario (leads, empresas, contactos)
- Estado
- Porcentaje de finalización
- Gerente de ventas asignado
- Correos enviados hoy
- Número de destinatarios
- Número de cuentas de correo electrónico disponibles
- Notificaciones y mensajes de error

Las cuentas de correo electrónico asignadas a un gerente de ventas se representan mediante estrellas verdes y rojas.
<?xml version="1.0" encoding="utf-8"?>
<svg width="15px" height="15px" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill="#379634" d="M10 15l-5.878 3.09 1.123-6.545L.489 6.91l6.572-.955L10 0l2.939 5.955 6.572.955-4.756 4.635 1.123 6.545z"/></svg><?xml version="1.0" encoding="utf-8"?>
<svg width="15px" height="15px" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill="#379634" d="M10 15l-5.878 3.09 1.123-6.545L.489 6.91l6.572-.955L10 0l2.939 5.955 6.572.955-4.756 4.635 1.123 6.545z"/></svg><?xml version="1.0" encoding="utf-8"?>
<svg width="15px" height="15px" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill="#e4572e" d="M10 15l-5.878 3.09 1.123-6.545L.489 6.91l6.572-.955L10 0l2.939 5.955 6.572.955-4.756 4.635 1.123 6.545z"/></svg>  
Un color verde indica que la cuenta puede utilizarse para enviar correos electrónicos.

### Estados del Mailing

Los mailings pueden tener los siguientes estados:

* **Activo**: el envío está en curso
* **Activo, pero con errores**: el envío continúa, pero se han producido problemas
* **En pausa**
* **Interrumpido**: el envío se detuvo debido a errores críticos
* **Completado**: el mailing terminó

Para mostrar los datos más recientes, actualiza la página. Al iniciar un nuevo mailing, los detalles del progreso aparecerán aproximadamente en **5 minutos**.

---

## **Gestión de errores durante un Mailing Masivo**

Si se produce un error:

- El estado cambia a **Activo, pero con errores**.
- En la columna **Notificaciones** aparece un mensaje detallado.
- Si se producen varios errores, el campo se vuelve desplazable.
- Los errores críticos detienen el boletín y le asignan el estado **Interrumpido**.

Si algunos destinatarios no recibieron el correo electrónico:

1. Resuelve los problemas indicados, como el límite de la cuenta de correo o las direcciones no válidas.
2. Reinicia el mailing únicamente para los destinatarios que no recibieron el mensaje desde la página de detalles del mailing.

---

## **Búsqueda y filtrado de Mailings Masivos**

Utiliza la barra de búsqueda para encontrar mailings por:

- Palabras clave, como el nombre del mailing
- ID del mailing

Los filtros disponibles incluyen:

- Departamento, si el rol del usuario lo permite
- Estado VIP
- Propietario: gerente de ventas asignado

Estos filtros permiten navegar rápidamente por un gran volumen de mailings.

---

## **Combinación de varios Mailings**

El menú **Acciones** permite combinar varios mailings masivos en uno solo.
Los mailings solo se pueden combinar cuando tienen:

- El mismo mensaje de boletín
- El mismo tipo de destinatario
- El mismo propietario del mailing (gerente de ventas)

Esta función ayuda a evitar campañas de marketing por correo electrónico duplicadas y simplifica la gestión del flujo de trabajo.

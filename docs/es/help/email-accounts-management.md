---
title: Gestión de cuentas de correo electrónico
description: Aprende a gestionar las cuentas de correo electrónico en Django CRM, incluyendo la consulta de los detalles de las cuentas,
	el seguimiento del estado de sincronización y la comprensión de la lógica de la cuenta principal para el envío de correos del CRM y las campañas de correo masivo.
---

# Página de cuentas de correo electrónico en Django CRM

La página de **Cuentas de correo electrónico** en Django CRM es el centro de control para configurar y supervisar todos los
canales de correo utilizados para la comunicación con clientes, el envío de correos del CRM y las campañas de marketing por correo electrónico del CRM.

Django CRM admite la integración con cualquier proveedor de correo electrónico que funcione mediante los protocolos SMTP e IMAP,
incluidos servicios como **Gmail**.
Esto permite una sincronización bidireccional fiable tanto para la correspondencia individual como para las operaciones de correo masivo.

---

## Qué se puede ver en la página de cuentas de correo electrónico

Todas las cuentas de correo electrónico conectadas y asignadas se muestran en una tabla estructurada.
Esta vista general proporciona transparencia operativa para las actividades de envío de correos del CRM y correo masivo.

La tabla permite identificar rápidamente:

- **Cuentas asignadas a ti**
	Una lista completa de las cuentas de correo electrónico que tienes autorización para utilizar.

- **Cuenta predeterminada para la comunicación con clientes**
	La cuenta que el CRM ha designado como principal para la correspondencia saliente.

- **Estado de sincronización automática**
	Indica qué cuentas tienen habilitada la sincronización IMAP.
	Esto es especialmente importante para importar correos entrantes que contienen solicitudes y vincularlos automáticamente con los registros del CRM.

- **Actividad diaria de envío**

		- Marca de tiempo del último correo enviado
		- Número total de correos enviados ese día a través de cada cuenta
			Esto te ayuda a supervisar la distribución de la carga de trabajo y detectar actividades inusuales durante las campañas de correo masivo.

- **Notificaciones del sistema**
	El CRM muestra notificaciones relacionadas con:

		- Errores durante un envío masivo o una campaña de marketing por correo electrónico del CRM
		- Finalización correcta de una campaña de envío

Esta visibilidad operativa permite evaluar el rendimiento y la fiabilidad de cada cuenta utilizada para el envío de correos del CRM.

---

## Consulta de información detallada de la cuenta

Para acceder a información ampliada, haz clic en una cuenta de correo electrónico concreta de la lista.

La vista detallada puede incluir:

- Credenciales de acceso (visibles según los permisos)
- Parámetros de configuración SMTP e IMAP
- Configuración de sincronización
- Estadísticas de uso de la cuenta

Esta sección resulta especialmente útil para solucionar problemas relacionados con el correo masivo,
las campañas de marketing por correo electrónico del CRM o los errores de importación de correos.

---

## Notas importantes de configuración

### 1. Se requiere acceso administrativo

La configuración correcta de los parámetros SMTP e IMAP requiere conocimientos técnicos.
Si necesitas modificar la configuración de una cuenta de correo electrónico, ponte en contacto con el administrador del CRM.

Una configuración incorrecta puede provocar:

- Fallos en las campañas de envío de correos del CRM
- Interrupciones de la sincronización
- Errores en la entrega de correos electrónicos
- Importaciones incompletas de solicitudes

---

### 2. Lógica de la cuenta principal y de los clientes VIP

Django CRM aplica una regla específica para la **cuenta de correo electrónico principal**:

- La cuenta principal se utiliza para enviar correos **solo a destinatarios marcados como VIP**.
- Si la audiencia seleccionada para un envío masivo no contiene contactos VIP, los correos **no se enviarán** a través de la cuenta principal, incluso si está autorizada para utilizarse en marketing por correo electrónico del CRM.

Esta regla garantiza una gestión prioritaria de los clientes estratégicos y evita el uso indebido de los canales principales de comunicación.

---

## Prácticas recomendadas para el envío de correos del CRM y el correo masivo

Para garantizar operaciones estables de marketing por correo electrónico del CRM:

- Supervisa periódicamente las estadísticas de envío de cada cuenta.
- Comprueba el estado de sincronización de las cuentas responsables del procesamiento de solicitudes.
- Revisa las notificaciones del CRM después de cada campaña de correo masivo.
- Coordínate con el administrador antes de modificar la configuración de una cuenta.
- Confirma las etiquetas VIP antes de iniciar una campaña que dependa de la cuenta principal.

---

## Temas relacionados

Para obtener más información, consulta:

- [Gestión del correo masivo](managing-mass-mailings.md): cómo crear e iniciar una campaña de correo masivo en el CRM
- [Gestión de contactos de empresas](contact-management.md): cómo afecta el estado VIP a la lógica de envío de correos del CRM

---

La página de cuentas de correo electrónico es un módulo operativo fundamental de Django CRM.
Las cuentas configuradas correctamente garantizan un envío de correos fiable, una sincronización precisa de las solicitudes
y un rendimiento eficaz del marketing por correo electrónico del CRM.

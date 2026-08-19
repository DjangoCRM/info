---
title: Correo en CRM
description: Usa Correo en CRM para enviar, recibir y gestionar correos de clientes en un solo lugar. Mejora la comunicación con la gestión de correo del CRM y una solución integral de CRM con integración de correo.
---

# Correo en CRM

La página de **Correo en CRM** ofrece un espacio centralizado para gestionar la comunicación con clientes y socios dentro de la interfaz del CRM. En lugar de cambiar entre varias herramientas, los usuarios pueden gestionar las conversaciones directamente dentro del sistema, convirtiendo Django CRM en una solución práctica de **CRM con integración de correo**.

Con esta función, los equipos pueden **enviar**, **recibir** y **hacer seguimiento** de los **correos electrónicos** mientras mantienen una visibilidad completa del historial de comunicación con el cliente. Este enfoque mejora la colaboración, garantiza una comunicación constante y proporciona un flujo de trabajo estructurado de correo CRM para las interacciones con los clientes.

---

## Resumen de las funciones de correo

El sistema de correo integrado permite a los equipos gestionar la correspondencia del cliente sin salir del entorno del CRM.
Combina herramientas de comunicación con la gestión de clientes y acuerdos, convirtiendo la plataforma en un espacio de **CRM y correo**.

Las capacidades clave incluyen:

- Enviar y recibir correos directamente desde la interfaz del CRM
- Mantener un historial centralizado de correspondencia
- Vincular automáticamente los correos a objetos del CRM, como solicitudes y ofertas
- Permitir la visibilidad a nivel de departamento para facilitar la colaboración

Este enfoque integrado simplifica la gestión de correo del CRM y garantiza que toda la comunicación permanezca accesible y organizada.

---

## Integración y sincronización del correo

Django CRM admite la integración con proveedores de correo ampliamente utilizados,
permitiendo a las empresas conectar sus buzones existentes con el sistema del CRM.

### Proveedores de correo compatibles

La plataforma funciona con servicios populares que admiten SMTP, incluidos:

- **Gmail**
- **Outlook**
- **Yahoo**
- Otros proveedores compatibles

Esto hace que la plataforma sea un CRM flexible con capacidades de correo que se adapta a la mayoría de las infraestructuras de correo existentes.

### Sincronización con clientes de correo externos

Los usuarios no tienen que abandonar sus clientes de correo preferidos. El CRM puede sincronizar mensajes con herramientas externas como:

- Thunderbird
- Outlook
- Otros clientes de correo

Los correos intercambiados a través de esas herramientas se sincronizan con el CRM mediante el sistema de tickets.

**Importante:**

- Para **activar** la sincronización bidireccional entre el CRM y el buzón conectado, primero debe enviarse al menos un correo desde la interfaz del CRM.
  Después de la activación, la correspondencia aparecerá automáticamente en ambos sistemas, garantizando registros de comunicación consistentes.
- La sincronización de correos **no incluye la eliminación** de mensajes. No se preocupe: si elimina correos de su buzón conectado (por ejemplo, debido al límite de almacenamiento del proveedor de correo), esos correos seguirán existiendo en su CRM.
  El historial de conversaciones se conservará intacto.

---

## Vinculación automática a objetos del CRM

Una de las ventajas más valiosas del sistema de correo del CRM es la vinculación automática de contexto.

Cada correo intercambiado con un cliente se conecta a registros relacionados del CRM, incluidos:

- [Solicitudes](request-processing.md)
- [Ofertas](deals-management.md)

Esto significa que, cuando los usuarios abren una solicitud o una oferta, pueden ver de inmediato todo el historial de correos relacionado con esa interacción.

Los beneficios incluyen:

- Mejor comprensión del historial de comunicación con el cliente
- Resolución más rápida de problemas
- Mayor continuidad cuando varios empleados trabajan con el mismo cliente

---

## Visualización de correos en la página Correo en CRM

La página de **Correo en CRM** ofrece una lista centralizada de todos los mensajes asociados con su cuenta del CRM.

### Correspondencia personal

Los usuarios pueden ver y gestionar todos los correos que han intercambiado con clientes. Esto incluye mensajes enviados y recibidos,
creando una línea de tiempo completa de comunicación.

### Correspondencia del departamento

Según los permisos del usuario, los empleados también pueden ver la comunicación por correo de sus compañeros del mismo departamento.

- Estos correos están disponibles en modo de **solo lectura**
- Esta función ayuda a los miembros del equipo a entender conversaciones en curso
- También favorece el intercambio de conocimientos y un servicio al cliente coherente

Esta transparencia es especialmente valiosa en equipos de **ventas** o soporte colaborativo.

---

## Interfaz, clasificación y navegación

La lista de correos se muestra en una tabla estructurada diseñada para una navegación rápida y una gestión eficiente de la comunicación.

Los usuarios pueden organizar los mensajes haciendo clic en los encabezados de las columnas para ordenar los correos según:

- **Asunto**
- **Remitente o destinatario**
- **Usuario responsable (Propietario)**
- **Fecha de envío o recepción**

La clasificación ayuda a los usuarios a localizar rápidamente los mensajes más recientes o revisar la correspondencia relacionada con un cliente concreto.

---

## Búsqueda y filtrado de correos

Para simplificar la navegación en grandes volúmenes de correo, Django CRM ofrece potentes herramientas de búsqueda y filtrado.

### Búsqueda

Utiliza la barra de búsqueda para encontrar correos introduciendo palabras clave relacionadas con:

- Líneas de asunto
- Contenido del mensaje
- Direcciones de correo electrónico
- Nombres de clientes

Esta función permite localizar mensajes concretos en cuestión de segundos.

### Filtros

Los filtros ayudan a reducir los resultados de correo según criterios específicos.

Dependiendo de los permisos de acceso del usuario, los filtros pueden incluir:

- Buzones
- Propietarios de mensajes
- Departamentos

Estas opciones de filtrado son especialmente útiles para equipos que manejan un gran volumen de correspondencia en un entorno compartido de gestión de correo del CRM.

---

## Creación de un nuevo correo

Para redactar un nuevo mensaje desde la interfaz del CRM:

1. Abre la página de **Correo en CRM**.
2. Haz clic en el botón **Agregar correo**.
3. Introduce el destinatario, el asunto y el contenido del mensaje.
4. Si es necesario, puedes vincular el correo a los objetos correspondientes.
5. Envía el correo directamente desde el CRM.

Una vez enviado, el correo se almacenará en el CRM.

---

## Beneficios de usar el correo dentro del CRM

Usar el correo directamente dentro del CRM ofrece varias ventajas operativas:

- Historial de comunicación centralizado
- Mejor colaboración entre miembros del equipo
- Vinculación automática de mensajes a clientes, solicitudes y ofertas
- Menor riesgo de comunicación perdida o fragmentada
- Gestión eficiente del correo del CRM para las relaciones con los clientes

Al integrar herramientas de comunicación con los datos del cliente, Django CRM se convierte en una plataforma completa de **CRM con integración de correo** que soporta flujos de trabajo de ventas, soporte y atención al cliente.

---

## Temas relacionados

Para obtener información adicional sobre funciones de correo y comunicación en Django CRM, consulta:

- [Gestión de cuentas de correo electrónico](email-accounts-management.md): conexión de tu buzón al CRM
- [Campañas de correo CRM](../features/massmail-app-features.md): envío de boletines y anuncios

Estas guías te ayudarán a aprovechar al máximo Django CRM como una potente plataforma de comunicación CRM y correo.

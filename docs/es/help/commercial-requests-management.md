---
title: Gestión de Solicitudes Comerciales
description: Aprende a gestionar solicitudes comerciales en Django CRM, incluidos los roles de usuario, los derechos de acceso, la creación de solicitudes y las prácticas recomendadas.
---

# **Gestión de Solicitudes Comerciales**

Las solicitudes comerciales en [Django CRM](../index.md) ayudan a los equipos de ventas a realizar un seguimiento de clientes potenciales que buscan productos o servicios específicos. Una solicitud suele ser el primer paso para crear una transacción e iniciar el proceso de ventas.

Esta página explica cómo los usuarios del CRM gestionan las solicitudes comerciales, qué derechos de acceso se aplican y cómo trabajar eficazmente con la lista de solicitudes.

> Temas relacionados:  
> [Gestión de transacciones en Django CRM](deals-management.md)  
> [Explorar la aplicación CRM](../features/crm-app-features.md)

---

## **¿Qué son las solicitudes comerciales?**

Una solicitud incluye [datos esenciales](request-processing.md) sobre la consulta de un cliente: qué quiere comprar, a quién representa y sus datos de contacto. Estos registros pueden aparecer en el CRM de varias formas:

- **Automáticamente**, desde un formulario web
- **Automáticamente**, desde determinados correos electrónicos entrantes (si está configurado)
- **Manualmente**, añadidos por un usuario del CRM
- **Copiados** de una solicitud existente (para ahorrar tiempo con consultas recurrentes)

Es importante mantener las solicitudes completas y precisas: los datos de contacto correctos permiten al CRM relacionar empresas, prospectos y contactos que ya están en la base de datos.

---

## **Roles de usuario que trabajan con solicitudes**

Hay **tres roles** directamente involucrados en la gestión de solicitudes:

| Rol | Responsabilidades | Nivel de acceso |
| --- | --- | --- |
| **Operador** | Procesa solicitudes, crea transacciones y asigna el gerente de ventas | Solo dentro del departamento asignado |
| **Súper operador** | Gestiona solicitudes de todos los departamentos | Todas las solicitudes de la empresa |
| **Gerente de ventas** | Crea solicitudes y transacciones | Solo dentro del departamento asignado |

Si el CRM se utiliza en una pequeña empresa, la misma persona puede actuar como operador **y** gerente de ventas.

Los gerentes de ventas trabajan principalmente con **transacciones**, no con solicitudes. Los operadores convierten las solicitudes calificadas en transacciones y las asignan para continuar el trabajo. Cuando las solicitudes llegan directamente a los gerentes de ventas, ellos mismos las crean.

Para cambiar de rol o solicitar acceso adicional, ponte en contacto con tu **administrador del CRM**.

---

## **¿Cuándo se debe crear una transacción?**

Una transacción representa el **flujo de trabajo de ventas activo**, no el contrato cerrado. Para la mayoría de las solicitudes válidas, **se debe crear una transacción**.

**No se crea una transacción** únicamente cuando la solicitud está marcada como:

* **Duplicada**
* **Caso/incidente** (solicitud de soporte sin potencial comercial)
* **Irrelevante** (el campo está oculto de forma predeterminada)

---

## **Cómo añadir solicitudes**

Los usuarios con los permisos adecuados pueden añadir solicitudes:

| Método | Cómo funciona |
| --- | --- |
| Botón **Añadir solicitud** | Abre un formulario vacío; completa todos los datos obligatorios |
| **Importar solicitud desde el correo electrónico** | Crea una solicitud a partir de un correo entrante (primero se debe configurar la cuenta de correo en el CRM) |
| Botón **Copiar** | Crea un borrador duplicado con datos editables |

Las solicitudes procedentes de formularios de contacto del sitio web aparecen automáticamente en el sistema.

---

## **Gestión de la lista de solicitudes**

Todas las solicitudes se muestran en una tabla ordenable. Los encabezados de las columnas incluyen:

- **Nombre de la solicitud**
- **Etiqueta de fidelidad**  
	• *Principal*: generada por marketing  
	• *Posterior*: contacto directo de un cliente conocido o de una empresa conocida
- **Nombre de la contraparte** (prospecto o empresa)
- **País**
- **Persona de contacto**
- **Fecha de la solicitud**
- **Operador o gerente de ventas asignado**
- **Estado de la solicitud**: *pendiente* o *procesada*

### **Búsqueda y filtrado**

Puedes encontrar rápidamente las solicitudes necesarias mediante:

✅ **Barra de búsqueda**: busca por ID *(id123)* o palabras clave  
✅ **Panel de filtros**: filtra por:

- Departamento (si el rol lo permite)
- Estado de la solicitud
- Operador o gerente de ventas asignado
- Fecha de recepción
- Producto o servicio
- Fidelidad
- País

---

## **Resumen de las reglas de acceso**

| Tipo de usuario | Qué puede consultar |
| --- | --- |
| Operador | Solicitudes de su propio departamento |
| Gerente de ventas | Solicitudes de su propio departamento (asignadas a esa persona) |
| Súper operador | Solicitudes de todos los departamentos |
| Gerente de la empresa | Visibilidad completa en todo el CRM |

---

## **Prácticas recomendadas**

* Revisa cada solicitud nueva lo antes posible
* Verifica los datos de contacto del cliente
* Marca los duplicados para evitar confusiones en el embudo de ventas
* Convierte las solicitudes calificadas en transacciones de inmediato

> Lectura recomendada:
>
> * [Explorar la aplicación CRM en la suite Django CRM](../features/crm-app-features.md)

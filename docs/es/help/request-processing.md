---
title: Procesamiento de Solicitudes
description: Aprenda cómo procesar efectivamente solicitudes comerciales en Django CRM, incluida la verificación de detalles de solicitudes,
  enriquecimiento de información faltante, vinculación con entidades de CRM existentes y creación de tratos o casos.
---

# **Procesamiento de Solicitudes en Django CRM**

El procesamiento de solicitudes garantiza que toda consulta de cliente entrante se convierta en datos de CRM precisos, completos
y accionables. Esta página guía a los usuarios a través de la verificación de detalles de solicitudes, enriquecimiento de información faltante,
vinculación de la solicitud con entidades de CRM existentes y, finalmente, creación de un trato o cierre de la solicitud como caso.
El procesamiento efectivo de solicitudes fortalece la calidad de los datos, reduce duplicados y mejora la velocidad de seguimiento.

---

## **Propósito del procesamiento de solicitudes**

El procesamiento de solicitudes se enfoca en **verificar** y **enriquecer** la información de contacto del cliente antes de pasar la consulta al pipeline de ventas.
El manejo preciso de solicitudes garantiza la verificación e integridad de los datos del cliente.
Esto cumple dos funciones críticas:

1. Asegurar que el equipo de ventas pueda contactar al cliente.
2. Coincidir la consulta con registros existentes de CRM para evitar [leads](lead-management.md),
  [contactos](contact-management.md) o [empresas](company-management.md) duplicados.

La mayoría de [solicitudes](commercial-requests-management.md) de clientes se generan automáticamente cuando un visitante envía un formulario del sitio web o envía un correo electrónico.
Antes de que la solicitud se convierta en un trato, toda la información debe verificarse en cuanto a precisión e integridad.

Una vez **validada**, se debe crear un trato. Para los usuarios con rol de operador,
el propietario de la solicitud debe reasignarse a un gerente de ventas antes de crear el trato.
Tenga en cuenta que los tratos no se pueden crear a partir de solicitudes marcadas como duplicadas o como casos/incidentes.

---

## **Contador de solicitudes y flujo de trabajo de asignación**

El panel izquierdo incluye un **contador** de solicitudes que ayuda a los usuarios de CRM a realizar un seguimiento de la carga de trabajo entrante.

- El valor verde muestra la cantidad de nuevas solicitudes pendientes que necesitan procesamiento.
- El valor rojo indica solicitudes con más de 24 horas que aún no se asignan a un gerente de ventas.

Una solicitud desaparece del contador una vez que se asigna un gerente de ventas como propietario.

---

## **Manejo de casos e incidentes**

Si una solicitud no requiere seguimiento de pagos o ventas, debe marcarse como **caso/incidente**.
Esto reemplaza el botón Crear Trato con un botón Cerrar.
Los casos aparecen en verde en la lista de solicitudes y se vuelven grises después de cerrarse. Estos elementos se excluyen del flujo de trabajo de ventas
pero permanecen disponibles para el seguimiento de soporte.

---

## **Trabajar con los botones de acción**

Cuando abre una solicitud, aparece un conjunto de botones de acción grises en la parte superior.
Estas acciones no modifican ni guardan datos de solicitud. Le permiten:

- Crear un correo electrónico vinculado a la solicitud
- Ver toda la correspondencia por correo electrónico
- Importar un correo electrónico manualmente desde su bandeja de entrada (los correos electrónicos con el ticket de solicitud se importan automáticamente)
- Imprimir la solicitud
- Copiar la solicitud para crear una nueva usando los mismos datos
- Ver el historial de cambios

Pasar el mouse sobre cualquier botón muestra una **información sobre herramientas** que explica su función.

---

## **Cómo rellenar correctamente los campos de nombre de contacto**
Para mantener la precisión de los registros, CRM proporciona tres campos separados para nombres:

- Nombre
- Segundo nombre
- Apellido

Solo se permite **una palabra** en los campos de nombre y apellido. Si un nombre completo contiene más de tres palabras,
todas las palabras adicionales deben colocarse en el campo Segundo nombre.
Esto ayuda a prevenir inconsistencias de datos y mejora la precisión de coincidencia.

---

## **Cómo evitar registros de empresas duplicados**

Preste **atención** cuidadosa al campo Nombre de empresa. Los clientes a menudo proporcionan nombres de empresas abreviados o acortados,
lo que puede causar entradas de empresas duplicadas.
Si la empresa ya existe en el CRM, ingrese abreviaturas y variaciones ortográficas en el campo "**Nombres Alternativos**"
del perfil de la empresa en lugar de crear una empresa nueva.

---

## **Traducción, observaciones y selección de productos**

- Si una solicitud llega en un idioma extranjero, use el campo Traducción para proporcionar una versión traducida.
- Esta traducción también aparecerá en el trato.
- Ingrese comentarios internos o aclaraciones en el campo Observación.
- Use el campo Productos para seleccionar los productos o servicios solicitados.
  Esto mejora la calidad de los informes de CRM y permite el filtrado basado en productos en la lista de solicitudes.

---

## **Validación de relaciones y vinculación automática**

Al crear una solicitud, Django CRM intenta encontrar clientes **coincidentes** en la base de datos.
Si se encuentra una coincidencia, el sistema vincula la solicitud a un lead, contacto y empresa existentes.
Estos enlaces aparecen en la sección Relaciones, acompañados de una casilla de verificación que indica que las relaciones necesitan verificación.
Revise y confirme estos enlaces, y luego desmarque la casilla una vez que la validación sea completa.

Si no se encuentra ninguna coincidencia, el CRM creará un **nuevo lead**, contacto y empresa (dependiendo de los datos disponibles) durante la creación del trato
y los vinculará automáticamente a la solicitud.

---

## **Ver conversaciones de correo electrónico**

La parte inferior de la página de solicitud muestra los últimos cuatro correos electrónicos intercambiados en la conversación.
Esto proporciona a los usuarios contexto inmediato sin tener que alejarse de la solicitud.

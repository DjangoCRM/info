---
hide:
  - toc
title: Gestión de Relaciones con Clientes de Código Abierto
description: CRM con integración de correo electrónico para administrar ventas, soporte y flujos de trabajo con clientes. Realiza seguimiento de consultas, automatiza la conversión de prospectos y aprovecha análisis para mejorar el rendimiento

---

# Explore la Aplicación CRM en el Suite Django CRM

La aplicación CRM en el núcleo del paquete de software Django CRM proporciona a equipos de ventas, personal de soporte y propietarios de negocios una plataforma centralizada para manejar consultas de clientes, solicitudes comerciales y flujos de trabajo de transacciones. Asegura tu CRM asignando permisos granulares. Controla quién puede ver, añadir, editar o eliminar cada tipo de registro, y mantén el cumplimiento de políticas internas. Con control de acceso basado en roles, cada usuario ve solo los datos que necesita.  
Los datos de la aplicación CRM fluyen hacia el módulo de Analytics para reportes profundos sobre embudos de ventas, desglose de ingresos y métricas de conversión—ayudando a los equipos a refinar tácticas y mejorar el rendimiento.

<figure markdown="span">
  ![Captura de pantalla de lista de solicitudes de CRM](../assets/img/screenshots/request_list_screenshot.png){ loading=lazy width="680"}
  <figcaption>Captura de pantalla de la página de Solicitudes en el Software CRM</figcaption>
</figure>

---

## Gestión de Solicitudes Comerciales

* **Captura de consultas entrantes**  
  Las consultas entrantes pueden capturarse desde formularios web, correos electrónicos o ingresarse manualmente. Cada solicitud se etiqueta como "pendiente" hasta ser validada.

* **Vinculación de Entidades**  
  Al guardar, el sistema busca coincidencias en registros de Empresas, Personas de Contacto o Prospectos y adjunta la solicitud a registros existentes cuando es posible.
  Si una nueva solicitud no coincide con ninguna entidad existente, el sistema genera automáticamente un registro de Prospecto.

* **Verificación y Filtrado**

    * Las solicitudes válidas avanzan hacia la configuración de transacciones.
    * Las solicitudes irrelevantes o imposibles de cumplir se marcan como tales o se eliminan.
    * Los contadores en tiempo real muestran el número de solicitudes recibidas de cada cliente.

* **Información de Geolocalización**  
  La búsqueda basada en IP detecta el país y la ciudad de cada corresponsal, ayudando a los equipos a asignar seguimientos basados en territorios.

* **Protección contra Spam**  
  Los administradores pueden añadir nombres de empresas prohibidas y frases de bloqueo para filtrar presentaciones repetitivas o no solicitadas.

> **Nota:** Para una descripción detallada de la gestión de Solicitudes Comerciales, por favor consulta la [documentación de Gestión de Solicitudes Comerciales](../help/commercial-requests-management.md).

---

## Gestión de Empresas, Contactos y Prospectos

* **Creación Inteligente de Registros**  
  Mantén un directorio estructurado de organizaciones y contactos asociados. Visualiza perfiles de empresas junto con todos los transacciones relacionados, comunicaciones y actividades.

* **Flujo de Trabajo de Conversión de Prospectos**  
  Los Prospectos validados pueden elevarse a registros de Clientes completos con un solo clic, reteniendo todos los datos históricos de solicitudes.

* **Prevención de Duplicados**  
  Antes de convertir un Prospecto a una Empresa y Contacto formales, el CRM realiza una verificación cruzada de entradas existentes para evitar duplicados.

---

## Procesamiento de Transacciones

* **Objetos de Transacción**  
  Crea una Oportunidad (Transacción) directamente desde una solicitud verificada. Cada Transacción sirve como un espacio de trabajo para realizar seguimiento del progreso hacia el cierre.

* **Tuberías Personalizables**  
  Define tus propias etapas de ventas como propuesta, negociación, cierre y monitorea cada Transacción visualmente mientras avanza.

* **Indicadores de Estado**  
  Los iconos señalan la próxima acción requerida, fechas de vencimiento y la salud general de cada etapa de la tubería.

* **Ordenamiento y Filtrado**  
  Las nuevas Transacciones aparecen en la parte superior de forma predeterminada; los equipos pueden reordenar por fecha de próximo paso, prioridad o campos personalizados.

* **Cierre de Transacciones**  
  Cuando una Transacción concluye, selecciona un motivo de "Ganada" o "Perdida" del menú desplegable. Las Transacciones cerradas se ocultan de las listas activas pero permanecen buscables en la base de datos.

---

## Manejo de Moneda y Pagos

* **Compatibilidad Multi-Moneda**  
  Administra transacciones internacionales con múltiples monedas. Especifica una moneda nacional y una moneda separada para reportes de marketing si es necesario.

* **Actualizaciones de Tipos de Cambio**  
  Los tipos pueden ingresarse manualmente u obtenerse a través de servicios externos, asegurando que los datos financieros se mantengan precisos.

* **Registro de Pagos**  
  Registra pagos directamente en la página de Transacción o desde la vista de Pagos centralizada. Todas las entradas se incluyen en reportes analíticos para análisis de ingresos.

---

## Integración y Extensibilidad

* **Formularios Web**

    * reCAPTCHA integrado y captura de IP.
    * Diseño personalizable para coincidir con directrices de marca.
    * Validación de campos protege contra entradas incompletas o inválidas.

* **Integración de Correo Electrónico**

    * Envía y recibe mensajes dentro del CRM usando **SMTP/IMAP**.
    * Numeración de **boletos** automática mantiene la correspondencia organizada.
    * Posibilidad de importación manual de cartas históricas y vinculación a Transacciones.

* **Importación/Exportación de Datos**  
  La compatibilidad con Excel para el manejo masivo de Empresas, Contactos, Prospectos y Transacciones hace que las migraciones y copias de seguridad sean sencillas.

---

## Rastreo de Envíos

* **Fechas de Envío Contratadas**  
  Asigna fechas de envío esperadas a cada Transacción.

* **Estado en Tiempo Real**  
  El progreso del envío se muestra dentro del registro de Transacción, asegurando que los equipos de ventas y operaciones se mantengan alineados en los cronogramas de entrega.

---

> [Instalación de CRM](https://django-crm-admin.readthedocs.io/en/latest/installation/)

Al consolidar consultas, datos de clientes y tuberías de transacciones en una sola aplicación, la aplicación CRM permite a los equipos administrar su ciclo de vida de ventas con mayor visibilidad y control—respaldado por análisis profundos y flujos de trabajo personalizables.

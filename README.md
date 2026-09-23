# SERKONT

Asistente digital para contadores que centraliza la gestión de clientes, obligaciones tributarias, servicios, tareas, confirmaciones, pagos, agendas, comunicaciones y seguimiento operativo.

## Descripción

SERKONT es una plataforma de software diseñada para apoyar a los contadores en la gestión de sus actividades operativas diarias y en la relación con sus clientes.

A diferencia de un sistema contable tradicional, SERKONT no busca reemplazar las herramientas utilizadas para llevar la contabilidad. Su objetivo es facilitar la gestión de las actividades que ocurren alrededor de los servicios contables: organizar clientes, obligaciones, servicios y tareas, detectar vencimientos, solicitar confirmaciones a los clientes, gestionar pagos, organizar agendas, realizar seguimiento de pendientes, gestionar recordatorios y mantener la información operativa centralizada.

SERKONT busca convertirse en un asistente digital que permita al contador tener mayor control sobre sus clientes y sobre el estado de los servicios que debe gestionar, reduciendo progresivamente la intervención manual en procesos repetitivos.

Los clientes de los contadores no tendrán acceso directo a SERKONT ni necesitarán una cuenta dentro de la plataforma. La interacción con ellos se realizará principalmente mediante WhatsApp y, cuando este canal no esté disponible, mediante correo electrónico.

---

## Objetivos

- Centralizar la información operativa de los clientes.
- Gestionar las obligaciones tributarias asociadas a los clientes.
- Incorporar información tributaria proveniente de la DIAN.
- Permitir la incorporación automática o manual de información tributaria.
- Identificar automáticamente obligaciones próximas a vencer.
- Generar servicios automáticamente a partir de las obligaciones detectadas.
- Organizar los servicios y tareas asociados a cada cliente.
- Facilitar la comunicación y solicitud de confirmaciones.
- Gestionar los pagos asociados a los servicios.
- Automatizar el proceso posterior a la aprobación del pago.
- Gestionar la disponibilidad y agenda del contador.
- Permitir el seguimiento del estado de los servicios.
- Reducir el trabajo manual relacionado con seguimientos y recordatorios.
- Mantener trazabilidad sobre comunicaciones, pagos, agendas y servicios.
- Mantener documentos y soportes relacionados con los servicios organizados.
- Proteger la información de los contadores y sus clientes.
- Sentar las bases para futuras automatizaciones y funcionalidades asistidas por inteligencia artificial.

---

## Flujo principal

El flujo principal de SERKONT se basa en la siguiente secuencia:

```text
Cliente del contador
        ↓
Información tributaria
        ↓
Obligación tributaria
        ↓
Período
        ↓
Fecha de vencimiento
        ↓
Detección de vencimiento
        ↓
Aplicación de reglas
        ↓
Generación automática del servicio
        ↓
Comunicación con el cliente
        ↓
Confirmación
        ↓
Pago
        ↓
Validación del pago
        ↓
Agendamiento
        ↓
Ejecución del servicio
        ↓
Seguimiento
```

La relación fundamental de la información tributaria es:

```text
Cliente del contador
        ↓
Obligación
        ↓
Período
        ↓
Vencimiento
```

La información tributaria utilizada por SERKONT tendrá como fuente la DIAN.

La incorporación de esta información podrá realizarse mediante un mecanismo automatizado cuando exista una alternativa técnicamente viable, o mediante ingreso o carga manual por parte del contador cuando la automatización no esté disponible, no sea viable o no sea conveniente.

---

## Usuarios

### Contador

El contador es el usuario principal de SERKONT.

Desde la plataforma podrá:

- Registrar y gestionar clientes.
- Consultar información tributaria.
- Consultar obligaciones y vencimientos.
- Gestionar servicios.
- Gestionar tareas.
- Consultar confirmaciones.
- Consultar pagos.
- Gestionar agendas.
- Consultar notificaciones.
- Consultar comunicaciones.
- Realizar seguimiento de servicios.
- Consultar el historial operativo.
- Anular servicios cuando sea necesario.
- Gestionar su perfil y configuración.

### Cliente del contador

El cliente no tendrá acceso directo a SERKONT.

No necesitará:

- Crear una cuenta.
- Iniciar sesión.
- Instalar la aplicación móvil.

La interacción con SERKONT se realizará mediante:

- WhatsApp como canal principal.
- Correo electrónico como alternativa cuando WhatsApp no esté disponible.

El cliente podrá:

- Recibir información de servicios.
- Confirmar o rechazar servicios.
- Recibir enlaces de pago.
- Recibir información de agenda.
- Recibir recordatorios.
- Recibir otras comunicaciones operativas.

---

# Funcionalidades principales

## Gestión de clientes

- Registro y administración de clientes.
- Información general.
- Datos de contacto.
- Información necesaria para comunicaciones.
- Asociación con obligaciones tributarias.
- Asociación con servicios.
- Consulta de información relacionada con cada cliente.
- Seguimiento de actividades y servicios.
- Control de acceso a la información de cada contador.

Cada contador deberá poder gestionar únicamente sus propios clientes.

---

## Gestión de obligaciones tributarias

SERKONT incorporará la información tributaria necesaria para determinar cuándo debe iniciar la gestión de un servicio.

La información se organizará mediante:

```text
Cliente
   ↓
Obligación
   ↓
Período
   ↓
Fecha de vencimiento
```

La información podrá incorporarse mediante:

- Mecanismos automatizados.
- Ingreso manual.
- Carga manual de información.
- Información obtenida desde la DIAN.

La información incorporada deberá:

- Ser validada.
- Asociarse con el cliente correspondiente.
- Identificar la obligación.
- Identificar el período.
- Registrar la fecha de vencimiento.
- Mantener información sobre su origen.
- Mantener trazabilidad de actualización.
- Evitar duplicados.
- Mantener consistencia con la información disponible.

---

## Incorporación de información de la DIAN

SERKONT utilizará la DIAN como fuente de información tributaria.

El proyecto contempla investigar y determinar los mecanismos técnicamente disponibles para incorporar dicha información.

Entre las alternativas a evaluar se encuentran:

- Mecanismos oficiales de integración.
- APIs.
- Web Services.
- Servicios de interoperabilidad.
- Información pública.
- Open Data cuando corresponda.
- Otros mecanismos técnicamente disponibles.
- Ingreso o carga manual por parte del contador.

La incorporación automática no será una dependencia obligatoria del sistema.

SERKONT deberá poder continuar funcionando mediante mecanismos manuales cuando una integración automática no esté disponible o no sea viable.

---

## Actualización de información tributaria

La información tributaria deberá mantenerse actualizada.

El sistema deberá contemplar:

- Actualización automática cuando exista un mecanismo viable.
- Actualización manual por parte del contador.
- Detección de nuevas obligaciones.
- Detección de nuevos períodos.
- Detección de cambios en fechas de vencimiento.
- Validación de cambios.
- Control de duplicados.
- Registro del origen de la información.
- Registro de fechas de actualización.
- Trazabilidad de cambios.

---

## Detección de vencimientos

SERKONT contará con un motor encargado de identificar obligaciones próximas a vencer.

El motor utilizará las reglas de generación de servicios configuradas en el sistema.

Entre sus responsabilidades se encuentran:

- Evaluar obligaciones válidas.
- Evaluar períodos.
- Evaluar fechas de vencimiento.
- Aplicar reglas de anticipación.
- Identificar obligaciones próximas a vencer.
- Ignorar obligaciones que no cumplan las condiciones.
- Evitar detecciones duplicadas.
- Detectar nuevos períodos.
- Considerar cambios en fechas de vencimiento.
- Generar la información necesaria para iniciar la gestión del servicio.

El motor funcionará independientemente de si la información tributaria fue incorporada automáticamente o ingresada manualmente por el contador.

---

## Reglas de generación de servicios

SERKONT permitirá definir las reglas que determinan cuándo debe iniciar la gestión de un servicio.

Las reglas deberán relacionar:

```text
Obligación
     +
Fecha de vencimiento
     +
Período de anticipación
     ↓
Inicio de gestión
```

El objetivo es evitar que los criterios operativos dependan directamente del código de la aplicación.

Las reglas configuradas serán utilizadas por el motor de detección de vencimientos para determinar qué obligaciones requieren iniciar una gestión.

---

## Gestión de servicios

- Generación automática de servicios.
- Asociación de servicios con clientes.
- Asociación de servicios con obligaciones tributarias.
- Definición de estados.
- Consulta de servicios.
- Actualización de servicios.
- Seguimiento del ciclo de vida.
- Control de actividades pendientes.
- Gestión de confirmaciones.
- Gestión de pagos.
- Gestión de agendas.
- Gestión de cancelaciones.

Los servicios derivados de obligaciones tributarias podrán generarse automáticamente sin que el contador tenga que crearlos manualmente uno por uno.

---

## Gestión de tareas

- Crear tareas.
- Consultar tareas.
- Actualizar tareas.
- Asociar tareas con clientes.
- Asociar tareas con servicios.
- Definir estados.
- Gestionar fechas.
- Gestionar vencimientos.
- Identificar tareas pendientes.
- Registrar actividades realizadas.

Las tareas estarán orientadas principalmente a la gestión operativa del contador.

---

## Confirmaciones

SERKONT permitirá solicitar al cliente la confirmación de los servicios generados.

El sistema deberá:

- Generar solicitudes de confirmación.
- Enviar la solicitud al cliente.
- Recibir la respuesta.
- Identificar respuestas afirmativas.
- Identificar respuestas negativas.
- Identificar respuestas pendientes.
- Actualizar el estado correspondiente.
- Registrar el historial de confirmaciones.

La interacción no requerirá que el cliente tenga una cuenta en SERKONT.

---

## Comunicaciones

SERKONT utilizará una estrategia de comunicación centralizada.

### Canal principal

```text
WhatsApp
```

### Canal alternativo

```text
Correo electrónico
```

La selección del canal será gestionada por una regla común de comunicación.

Los módulos del sistema no deberán implementar de manera independiente la selección del canal.

Las comunicaciones podrán incluir:

- Solicitudes de confirmación.
- Avisos de servicios.
- Enlaces de pago.
- Recordatorios.
- Información de servicios.
- Información de agenda.
- Cambios de agenda.
- Cancelaciones.
- Notificaciones operativas.

---

## Integración con WhatsApp

WhatsApp será el canal principal de interacción entre SERKONT y los clientes de los contadores.

La integración deberá permitir:

- Enviar mensajes.
- Recibir mensajes.
- Procesar respuestas.
- Asociar mensajes con clientes.
- Asociar mensajes con servicios.
- Procesar confirmaciones.
- Enviar enlaces de pago.
- Enviar recordatorios.
- Comunicar información de agenda.
- Mantener trazabilidad de las comunicaciones.

La integración deberá funcionar como infraestructura común para los diferentes módulos de SERKONT.

Los clientes no necesitarán una cuenta ni autenticación en SERKONT.

---

## Integración de correo electrónico

El correo electrónico funcionará como canal alternativo de comunicación.

La integración deberá permitir:

- Enviar correos.
- Utilizar plantillas.
- Asociar mensajes con clientes.
- Asociar mensajes con servicios.
- Registrar resultados de envío.
- Gestionar errores.
- Mantener trazabilidad.

La integración será utilizada por los diferentes módulos que necesiten comunicarse con los clientes.

---

## Historial de comunicaciones

SERKONT permitirá al contador consultar el historial de comunicaciones relacionadas con sus clientes y servicios.

El historial podrá incluir información proveniente de:

- WhatsApp.
- Correo electrónico.

La consulta deberá permitir conocer:

- Cliente.
- Servicio relacionado.
- Canal utilizado.
- Tipo de comunicación.
- Fecha.
- Estado.
- Resultado.
- Eventos relacionados.

Esta funcionalidad estará orientada al seguimiento operativo y no será responsable de implementar el envío de mensajes.

---

## Seguimiento y recordatorios

SERKONT permitirá realizar seguimiento sobre el estado de los servicios y las actividades pendientes.

Se contemplan:

- Seguimiento de servicios.
- Seguimiento de tareas.
- Recordatorios.
- Seguimiento de vencimientos.
- Notificaciones.
- Identificación de pendientes.
- Registro de eventos relevantes.

Los recordatorios podrán ejecutarse automáticamente de acuerdo con las reglas definidas.

El sistema deberá evitar comunicaciones innecesarias o duplicadas.

---

## Notificaciones

SERKONT contará con un sistema de notificaciones para informar sobre eventos relevantes.

Las notificaciones podrán estar relacionadas con:

- Nuevos servicios.
- Confirmaciones recibidas.
- Pagos aprobados.
- Cambios de agenda.
- Recordatorios.
- Cancelaciones.
- Tareas pendientes.
- Otros eventos operativos.

Las notificaciones dirigidas al cliente utilizarán los canales externos definidos.

Las notificaciones internas permitirán al contador conocer situaciones que requieren atención.

---

# Pagos

## Modelo de pagos

SERKONT permitirá gestionar pagos asociados a los servicios confirmados por los clientes.

Cada pago deberá poder relacionarse con:

```text
Cliente
   ↓
Servicio
   ↓
Pago
   ↓
Transacción
```

El sistema deberá mantener:

- Estado del pago.
- Identificación de la transacción.
- Asociación con el servicio.
- Asociación con el cliente.
- Trazabilidad.
- Eventos provenientes de la pasarela.

---

## Pasarela de pagos

El pago será realizado mediante una pasarela externa.

El flujo será:

```text
Servicio confirmado
        ↓
Enlace de pago
        ↓
Cliente realiza el pago
        ↓
Pasarela de pagos
        ↓
Webhook
        ↓
Validación
        ↓
Pago aprobado
        ↓
Agendamiento
```

SERKONT no procesará directamente la transacción financiera.

El sistema deberá utilizar la información proporcionada por la pasarela para determinar el estado de cada pago.

---

## Webhooks de pagos

Los webhooks permitirán recibir eventos enviados por la pasarela de pagos.

SERKONT deberá:

- Recibir eventos.
- Validar su autenticidad.
- Identificar la transacción.
- Asociar el evento con el pago.
- Actualizar el estado.
- Mantener trazabilidad.
- Evitar procesamiento duplicado.
- Continuar el flujo cuando el pago sea aprobado.

---

## Estados de pagos

SERKONT gestionará el ciclo de vida de los pagos.

Los cambios de estado deberán:

- Corresponder a eventos válidos.
- Respetar las transiciones permitidas.
- Mantener trazabilidad.
- Evitar cambios inconsistentes.

Un servicio solo podrá avanzar hacia el agendamiento cuando el pago haya sido validado correctamente como aprobado.

---

# Agendamiento

## Agendamiento de servicios

Los servicios confirmados y con pago aprobado podrán avanzar hacia el proceso de agendamiento.

SERKONT deberá:

- Consultar disponibilidad.
- Identificar espacios disponibles.
- Evitar conflictos.
- Crear agendas.
- Asociar la agenda con el servicio.
- Mantener el estado de la agenda.
- Notificar la programación.

---

## Disponibilidad y conflictos

El sistema deberá considerar:

- Disponibilidad del contador.
- Servicios ya agendados.
- Duración del servicio.
- Modificaciones.
- Cancelaciones.
- Reprogramaciones.

Antes de crear o modificar una agenda deberá verificarse que no exista conflicto.

---

## Ciclo de vida de las agendas

Las agendas tendrán un ciclo de vida controlado.

Se deberán contemplar estados relacionados con:

- Creación.
- Confirmación.
- Modificación.
- Reprogramación.
- Ejecución.
- Finalización.
- Cancelación.

Cada transición deberá ser válida según el estado actual de la agenda y del servicio asociado.

---

## Historial de agendas

SERKONT mantendrá trazabilidad sobre los cambios realizados en las agendas.

El historial permitirá consultar eventos como:

- Creación.
- Confirmación.
- Modificación.
- Reprogramación.
- Cancelación.
- Finalización.

---

## Confirmación de agenda

Una vez cumplidas las condiciones necesarias para agendar un servicio, SERKONT podrá comunicar al cliente:

- Fecha.
- Hora.
- Información del servicio.
- Cambios posteriores.

La comunicación se realizará mediante WhatsApp o correo electrónico según la regla de canal establecida.

---

## Notificaciones de agenda

Las comunicaciones relacionadas con agenda incluirán:

- Confirmación de programación.
- Cambios.
- Reprogramaciones.
- Cancelaciones.
- Próximos servicios.

La información enviada deberá corresponder al estado real de la agenda.

---

## Cancelación de servicios

La cancelación de servicios será gestionada por el contador.

El cliente no podrá cancelar directamente un servicio dentro de SERKONT.

Si el cliente desea cancelar:

```text
Cliente
   ↓
Contacta al contador
   ↓
Contador registra la cancelación
   ↓
SERKONT actualiza el servicio
   ↓
SERKONT actualiza la agenda
   ↓
Se libera la disponibilidad
   ↓
Se gestionan los estados relacionados
```

Cuando corresponda, también deberán gestionarse los estados relacionados con el pago.

Toda cancelación deberá mantener trazabilidad.

---

# Aplicación móvil

La aplicación móvil de SERKONT estará destinada exclusivamente a los contadores.

Los clientes de los contadores no tendrán acceso ni autenticación dentro de la aplicación.

## Módulos principales

La aplicación contempla:

- Autenticación.
- Navegación principal.
- Dashboard.
- Clientes.
- Servicios.
- Tareas.
- Seguimiento.
- Agenda.
- Notificaciones.
- Perfil.
- Configuración.

---

## Autenticación móvil

La aplicación utilizará los mecanismos de autenticación definidos por el backend.

Se contempla:

- Inicio de sesión.
- JWT.
- Gestión de sesión.
- Cierre de sesión.
- Manejo de errores.
- Roles y permisos.
- Protección de rutas.

---

## Dashboard

El dashboard permitirá al contador obtener una visión general de su operación.

Podrá presentar información como:

- Servicios pendientes.
- Próximos vencimientos.
- Tareas pendientes.
- Confirmaciones pendientes.
- Pagos aprobados pendientes de agendamiento.
- Próximas agendas.
- Notificaciones relevantes.

La lógica de negocio permanecerá en el backend.

---

## Módulo de clientes

Permitirá al contador:

- Consultar clientes.
- Registrar clientes.
- Actualizar clientes.
- Buscar clientes.
- Consultar información asociada.

Los clientes no tendrán acceso a este módulo.

---

## Módulo de servicios

Permitirá al contador:

- Consultar servicios.
- Consultar estados.
- Consultar servicios generados automáticamente.
- Consultar información asociada.
- Realizar las acciones autorizadas.

---

## Módulo de tareas

Permitirá consultar y gestionar:

- Tareas pendientes.
- Tareas realizadas.
- Fechas.
- Estados.
- Relaciones con clientes.
- Relaciones con servicios.

---

## Módulo de seguimiento

Permitirá consultar:

- Estado de los servicios.
- Eventos relevantes.
- Cambios.
- Trazabilidad operativa.
- Situaciones pendientes.

---

## Módulo de agenda

Permitirá consultar:

- Servicios programados.
- Disponibilidad.
- Estado de agendas.
- Cambios.
- Información relacionada con los servicios agendados.

---

## Módulo de notificaciones

Permitirá al contador consultar:

- Nuevos servicios.
- Confirmaciones.
- Pagos aprobados.
- Cambios de agenda.
- Recordatorios.
- Cancelaciones.
- Otros eventos relevantes.

La generación de las notificaciones continuará siendo responsabilidad del backend.

---

## Perfil y configuración

El contador podrá consultar y gestionar la información y configuraciones permitidas para su propia cuenta.

El acceso estará controlado mediante autenticación, autorización y permisos.

---

## Conectividad

La aplicación móvil deberá manejar correctamente los diferentes estados de conectividad.

Se contempla:

- Detectar pérdida de conexión.
- Informar al contador.
- Controlar operaciones dependientes de la API.
- Evitar estados inconsistentes.
- Evitar pérdida de información.

La aplicación no será inicialmente una aplicación completamente offline.

---

# Procesamiento asíncrono

SERKONT utilizará un enfoque híbrido de procesamiento.

## Procesamiento síncrono

Se utilizará para operaciones que requieren una respuesta inmediata de la API, como:

- Inicio de sesión.
- Registro de clientes.
- Consultas.
- Actualizaciones.
- Operaciones CRUD.
- Acciones realizadas directamente por el contador.

## Procesamiento asíncrono

Se utilizará para procesos que no deben bloquear la API.

Entre ellos:

- Detección periódica de vencimientos.
- Actualización automática de información tributaria.
- Generación automática de servicios.
- Recordatorios.
- Notificaciones.
- Procesamiento de mensajes.
- Webhooks.
- Procesamiento posterior a eventos externos.
- Procesamiento de múltiples clientes.
- Procesos de larga duración.

El objetivo es evitar que procesos pesados bloqueen las solicitudes realizadas directamente por el contador.

---

# Seguridad y protección de datos

SERKONT maneja información relacionada con:

- Contadores.
- Clientes.
- Información tributaria.
- Servicios.
- Pagos.
- Comunicaciones.
- Agendas.
- Tareas.
- Registros de actividad.

El sistema deberá implementar controles sobre:

- Autenticación.
- Autorización.
- Roles.
- Permisos.
- Aislamiento de información entre contadores.
- Protección de credenciales.
- Protección de tokens.
- Validación de datos.
- Protección de endpoints.
- Seguridad de webhooks.
- Integraciones externas.
- Información sensible.
- Logs.
- Trazabilidad.

Cada contador deberá poder acceder únicamente a la información correspondiente a sus propios clientes.

La información sensible no deberá exponerse innecesariamente mediante respuestas de API, logs, comunicaciones o interfaces.

---

# Arquitectura tecnológica

SERKONT utiliza una arquitectura modular orientada a facilitar su evolución, mantenimiento y escalabilidad progresiva.

## Tecnologías principales

- **Aplicación móvil:** React Native + TypeScript + Expo
- **Backend:** Python + Flask
- **ORM:** SQLAlchemy
- **Base de datos:** PostgreSQL
- **Contenedores:** Docker
- **Infraestructura:** AWS
- **Control de versiones:** Git + GitHub
- **CI/CD:** GitHub Actions

---

# Arquitectura general

```text
                         ┌─────────────────────┐
                         │      CONTADOR       │
                         │ React Native + Expo │
                         └──────────┬──────────┘
                                    │
                                    │ HTTPS / API
                                    ▼
                         ┌─────────────────────┐
                         │      Flask API      │
                         │       Backend       │
                         └──────────┬──────────┘
                                    │
              ┌─────────────────────┼─────────────────────┐
              │                     │                     │
              ▼                     ▼                     ▼
       ┌─────────────┐      ┌─────────────┐      ┌──────────────┐
       │ PostgreSQL  │      │ Procesamiento│      │ Integraciones│
       │             │      │ asíncrono    │      │ externas     │
       └─────────────┘      └─────────────┘      └───────┬──────┘
                                                         │
                        ┌────────────────────────────────┼──────────────────┐
                        │                                │                  │
                        ▼                                ▼                  ▼
                      DIAN                            WhatsApp            Pagos
                                                         │
                                                         ▼
                                                       Email
```

---

# Estructura del proyecto

```text
serkont/
├── backend/
├── mobile/
├── infra/
└── docs/
```

### Backend

Contendrá:

- API.
- Lógica de negocio.
- Modelos.
- Autenticación.
- Autorización.
- Servicios.
- Integraciones.
- Procesamiento asíncrono.

### Mobile

Contendrá la aplicación móvil utilizada por los contadores.

### Infra

Contendrá:

- Configuración de Docker.
- Infraestructura.
- Despliegue.
- Configuración de servicios.
- Componentes necesarios para los diferentes entornos.

### Docs

Contendrá:

- Documentación técnica.
- Documentación funcional.
- Arquitectura.
- Operación.
- Integraciones.
- Procedimientos.

La estructura definitiva podrá evolucionar durante el desarrollo.

---

# Entorno de desarrollo

El entorno de desarrollo está basado en:

- Windows
- WSL2
- Ubuntu
- Docker Engine
- Docker Compose
- Git
- GitHub
- Visual Studio Code

El desarrollo se realiza dentro de Ubuntu mediante WSL2, utilizando Docker Engine para la ejecución de servicios y contenedores.

El proyecto busca evitar el uso de privilegios de root para las actividades habituales de desarrollo.

---

# Pruebas y calidad

SERKONT contempla diferentes niveles de pruebas.

## Pruebas del backend

Se deberán cubrir los principales componentes:

- Autenticación.
- Usuarios.
- Clientes.
- Obligaciones tributarias.
- Actualización tributaria.
- Detección de vencimientos.
- Generación de servicios.
- Confirmaciones.
- Pagos.
- Webhooks.
- Agendamiento.
- Cancelaciones.
- Notificaciones.
- Manejo de errores.
- Procesamiento asíncrono.

Las integraciones externas podrán utilizar mocks o entornos de prueba.

---

## Pruebas móviles

Se contemplan pruebas sobre:

- Autenticación.
- Gestión de clientes.
- Navegación.
- Servicios.
- Tareas.
- Agenda.
- Notificaciones.
- Manejo de conectividad.

---

## Pruebas de integración

Se validará el flujo principal:

```text
Información tributaria
        ↓
Detección de vencimiento
        ↓
Generación automática
        ↓
Comunicación
        ↓
Confirmación
        ↓
Pago
        ↓
Webhook
        ↓
Pago aprobado
        ↓
Agendamiento
        ↓
Ejecución
        ↓
Seguimiento
```

También deberán contemplarse escenarios como:

- Rechazo del servicio.
- Pago rechazado.
- Pago pendiente.
- Error de comunicación.
- Conflicto de agenda.
- Cancelación.
- Error de integración.
- Pérdida de conectividad.

---

# Infraestructura y despliegue

SERKONT será preparado para ejecutarse en AWS.

La infraestructura deberá contemplar:

- Backend mediante Docker.
- PostgreSQL.
- Servicios necesarios para procesamiento asíncrono.
- Gestión de secretos.
- HTTPS.
- Control de acceso.
- Separación entre entornos.
- Monitoreo.
- Logs.
- Respaldos.
- Recuperación.

Los entornos de desarrollo y producción deberán mantener separados sus recursos y credenciales.

---

# CI/CD

El proyecto utilizará GitHub Actions para automatizar procesos de integración y despliegue.

El pipeline deberá permitir progresivamente:

- Validar código.
- Ejecutar pruebas.
- Validar dependencias.
- Construir imágenes Docker.
- Detectar errores antes de integrar cambios.
- Preparar despliegues.
- Separar procesos de desarrollo y producción.

---

# Monitoreo y observabilidad

SERKONT contará con mecanismos de monitoreo y observabilidad para conocer el estado de:

- API.
- Contenedores.
- Base de datos.
- Procesamiento asíncrono.
- Integraciones externas.
- Webhooks.

El objetivo será facilitar:

- Detección de errores.
- Diagnóstico.
- Seguimiento de incidentes.
- Identificación de fallos.
- Mantenimiento del sistema.

---

# Respaldos y recuperación

La base de datos PostgreSQL deberá contar con mecanismos de respaldo y recuperación.

Los respaldos deberán:

- Ejecutarse de forma controlada.
- Almacenarse de forma segura.
- Contar con una estrategia de conservación.
- Permitir restauración.
- Ser verificados periódicamente.

La recuperación deberá contar con procedimientos documentados.

Los respaldos técnicos y la gestión de conservación de información operativa son conceptos independientes.

---

# Documentación y operación

SERKONT deberá contar con documentación suficiente para:

- Configurar el entorno.
- Ejecutar el proyecto.
- Comprender la arquitectura.
- Comprender el modelo de datos.
- Configurar integraciones.
- Ejecutar pruebas.
- Realizar despliegues.
- Operar el sistema.
- Gestionar incidentes.
- Recuperar servicios.
- Mantener la infraestructura.

La documentación deberá mantenerse alineada con la implementación real.

---

# Gestión del proyecto

El desarrollo de SERKONT se gestiona mediante GitHub Projects utilizando un flujo Kanban.

## Flujo de trabajo

```text
Backlog → Ready → In Progress → In Review → Done
```

Las actividades se gestionan mediante Issues y se organizan utilizando:

- **Milestones:** representan etapas importantes del proyecto.
- **Etiquetas:** identifican áreas y tipos de trabajo.
- **Issues:** representan actividades concretas.
- **Checklists:** permiten dividir actividades en tareas más pequeñas.
- **Git y GitHub:** gestionan el control de versiones.
- **GitHub Projects:** permite visualizar y gestionar el flujo de trabajo.

La planificación detallada y el estado de las actividades se mantienen en GitHub.

---

# Progreso del proyecto

## Milestone 1 — Entorno de desarrollo

- [ ] Configurar Docker.
- [ ] Configurar Git y GitHub.
- [ ] Configurar Visual Studio Code para WSL.
- [ ] Preparar entorno Python.
- [ ] Verificar herramientas de desarrollo.

## Milestone 2 — Arquitectura inicial

- [ ] Crear estructura inicial de SERKONT.
- [ ] Definir arquitectura del backend.
- [ ] Definir arquitectura móvil.
- [ ] Definir estructura de infraestructura.
- [ ] Preparar documentación técnica inicial.

## Milestone 3 — Backend base

- [ ] Crear proyecto Flask.
- [ ] Configurar dependencias.
- [ ] Implementar manejo de errores.
- [ ] Estandarizar respuestas.
- [ ] Implementar validación de datos.
- [ ] Implementar logging.
- [ ] Configurar CORS.
- [ ] Preparar estructura para procesamiento asíncrono.

## Milestone 4 — Base de datos

- [ ] Configurar PostgreSQL.
- [ ] Conectar Flask con PostgreSQL.
- [ ] Diseñar modelo de datos.
- [ ] Implementar modelos mediante SQLAlchemy.
- [ ] Configurar migraciones.
- [ ] Modelar clientes.
- [ ] Modelar obligaciones tributarias.
- [ ] Modelar servicios.
- [ ] Modelar tareas.
- [ ] Modelar confirmaciones.
- [ ] Modelar pagos.
- [ ] Modelar agendas.
- [ ] Modelar trazabilidad.

## Milestone 5 — Autenticación y usuarios

- [ ] Implementar JWT.
- [ ] Implementar registro.
- [ ] Implementar inicio de sesión.
- [ ] Implementar autorización.
- [ ] Implementar roles y permisos.
- [ ] Implementar recuperación de contraseña.
- [ ] Implementar gestión de sesiones.

## Milestone 6 — Gestión de clientes

- [ ] Registrar clientes.
- [ ] Consultar clientes.
- [ ] Actualizar clientes.
- [ ] Desactivar clientes.
- [ ] Gestionar datos de contacto.
- [ ] Asociar clientes con obligaciones.
- [ ] Asociar clientes con servicios.

## Milestone 7 — Gestión de servicios

- [ ] Diseñar obligaciones tributarias.
- [ ] Investigar mecanismos de incorporación de información de la DIAN.
- [ ] Implementar incorporación de información tributaria.
- [ ] Implementar actualización de información tributaria.
- [ ] Configurar reglas de generación de servicios.
- [ ] Implementar motor de detección de vencimientos.
- [ ] Implementar generación automática de servicios.
- [ ] Gestionar estados de servicio.

## Milestone 8 — Gestión de tareas

- [ ] Crear tareas.
- [ ] Asociar tareas con servicios.
- [ ] Asociar tareas con clientes.
- [ ] Definir estados.
- [ ] Gestionar fechas y vencimientos.
- [ ] Gestionar pendientes.

## Milestone 9 — Confirmaciones

- [ ] Crear solicitudes de confirmación.
- [ ] Integrar confirmaciones con WhatsApp.
- [ ] Integrar confirmaciones con correo electrónico.
- [ ] Registrar respuestas.
- [ ] Gestionar estados.
- [ ] Registrar historial.

## Milestone 10 — Seguimiento y recordatorios

- [ ] Implementar seguimiento de servicios.
- [ ] Implementar recordatorios.
- [ ] Implementar notificaciones.
- [ ] Diseñar procesamiento asíncrono.
- [ ] Integrar procesamiento asíncrono.
- [ ] Implementar historial de comunicaciones.
- [ ] Implementar cancelación de servicios.

## Milestone 11 — Aplicación móvil

- [ ] Configurar React Native + Expo.
- [ ] Configurar TypeScript.
- [ ] Implementar autenticación.
- [ ] Implementar navegación.
- [ ] Implementar dashboard.
- [ ] Implementar módulo de clientes.
- [ ] Implementar módulo de servicios.
- [ ] Implementar módulo de tareas.
- [ ] Implementar módulo de seguimiento.
- [ ] Implementar módulo de agenda.
- [ ] Implementar módulo de notificaciones.
- [ ] Implementar perfil y configuración.
- [ ] Implementar manejo de conectividad.
- [ ] Implementar actualización de datos.
- [ ] Integrar aplicación con la API.

## Milestone 12 — Pruebas y calidad

- [ ] Configurar entorno de pruebas móvil.
- [ ] Implementar pruebas de autenticación móvil.
- [ ] Implementar pruebas del módulo de clientes móvil.
- [ ] Implementar pruebas del backend.
- [ ] Implementar pruebas unitarias.
- [ ] Implementar mocks.
- [ ] Implementar pruebas de integración.
- [ ] Validar flujo principal.
- [ ] Realizar revisión de seguridad.

## Milestone 13 — Infraestructura y despliegue

- [ ] Implementar CI/CD.
- [ ] Preparar infraestructura AWS.
- [ ] Preparar entornos.
- [ ] Configurar secretos.
- [ ] Configurar HTTPS.
- [ ] Configurar producción.
- [ ] Implementar monitoreo.
- [ ] Implementar observabilidad.
- [ ] Implementar respaldos PostgreSQL.
- [ ] Implementar recuperación.
- [ ] Documentar operación.

## Pagos y agendamiento

- [ ] Diseñar modelo de pagos.
- [ ] Integrar pasarela de pagos.
- [ ] Implementar webhooks.
- [ ] Gestionar estados de pagos.
- [ ] Implementar agendamiento.
- [ ] Gestionar disponibilidad.
- [ ] Gestionar conflictos.
- [ ] Gestionar ciclo de vida de agendas.
- [ ] Implementar historial de agendas.
- [ ] Implementar confirmación de agenda.
- [ ] Implementar notificaciones de agenda.

## Integración con WhatsApp

- [ ] Diseñar integración con WhatsApp.
- [ ] Implementar integración técnica.
- [ ] Definir canal estándar.
- [ ] Integrar confirmaciones.
- [ ] Integrar recordatorios.
- [ ] Integrar notificaciones.
- [ ] Integrar pagos.
- [ ] Integrar comunicaciones de agenda.

## Protección de datos y operación

- [ ] Implementar controles de tratamiento y protección de datos.
- [ ] Garantizar aislamiento de información entre contadores.
- [ ] Proteger información tributaria.
- [ ] Proteger información de clientes.
- [ ] Revisar exposición de información sensible.
- [ ] Documentar procedimientos de operación.
- [ ] Preparar soporte del MVP.

## MVP

- [ ] Integrar funcionalidades principales.
- [ ] Validar flujo completo.
- [ ] Validar integraciones externas.
- [ ] Validar pagos.
- [ ] Validar agendamiento.
- [ ] Validar comunicaciones.
- [ ] Validar seguridad.
- [ ] Validar infraestructura.
- [ ] Corregir errores críticos.
- [ ] Validar el MVP en producción.
- [ ] Preparar operación y soporte.

---

# Filosofía del proyecto

SERKONT busca mantener una arquitectura simple, modular y mantenible.

Las decisiones técnicas estarán orientadas principalmente a:

- Separación de responsabilidades.
- Código mantenible.
- Seguridad.
- Escalabilidad progresiva.
- Facilidad de despliegue.
- Automatización.
- Buenas prácticas de desarrollo.
- Pruebas automatizadas.
- Documentación clara.
- Trazabilidad.
- Bajo acoplamiento entre componentes.

El proyecto priorizará la construcción de una base sólida antes de incorporar funcionalidades complejas.

La lógica de negocio deberá permanecer principalmente en el backend, mientras que la aplicación móvil funcionará como cliente de la API.

Los procesos que requieran ejecución en segundo plano deberán utilizar procesamiento asíncrono cuando sea necesario, evitando convertir innecesariamente todas las operaciones en procesos asíncronos.

---

# Estado del proyecto

🚧 **En desarrollo**

SERKONT se encuentra actualmente en fase de construcción.

El proyecto está evolucionando desde la preparación del entorno y la arquitectura base hacia la implementación progresiva de:

- Backend.
- Base de datos.
- Autenticación.
- Gestión de clientes.
- Información tributaria.
- Detección de vencimientos.
- Generación automática de servicios.
- Comunicaciones.
- Confirmaciones.
- Pagos.
- Agendamiento.
- Seguimiento.
- Aplicación móvil.
- Pruebas.
- Seguridad.
- Infraestructura.
- Despliegue.

El estado detallado de cada actividad se mantiene en GitHub mediante Issues, Milestones y GitHub Projects.

---

# Contribución

Actualmente SERKONT se encuentra en desarrollo.

La estructura, arquitectura y procesos de contribución se definirán y documentarán a medida que el proyecto avance.

Las modificaciones deberán mantener las responsabilidades definidas para cada componente y respetar la arquitectura establecida del proyecto.

---

# Licencia

Licencia por definir.

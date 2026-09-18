# SERKONT

Asistente digital para contadores que centraliza la gestión de clientes, servicios, tareas, confirmaciones y seguimiento operativo.

## Descripción

SERKONT es una plataforma de software diseñada para apoyar a los contadores en la gestión de sus actividades operativas diarias y en la relación con sus clientes.

A diferencia de un sistema contable tradicional, SERKONT no busca reemplazar las herramientas utilizadas para llevar la contabilidad. Su objetivo es facilitar la gestión de las actividades que ocurren alrededor de los servicios contables: organizar servicios y tareas, solicitar confirmaciones a los clientes, realizar seguimiento de pendientes, gestionar recordatorios y mantener la información operativa centralizada.

SERKONT busca convertirse en un asistente digital que permita al contador tener mayor control sobre sus clientes y sobre el estado de los servicios que debe gestionar.

## Objetivos

- Centralizar la información operativa de los clientes.
- Organizar los servicios y tareas asociados a cada cliente.
- Facilitar la comunicación y solicitud de confirmaciones.
- Permitir el seguimiento del estado de los servicios.
- Reducir el trabajo manual relacionado con seguimientos y recordatorios.
- Mantener documentos y soportes relacionados con los servicios organizados.
- Sentar las bases para futuras automatizaciones y funcionalidades asistidas por inteligencia artificial.

## Funcionalidades principales

### Gestión de clientes

- Registro y administración de clientes.
- Información general y datos de contacto.
- Consulta del historial de actividades.
- Organización de información relacionada con cada cliente.

### Gestión de servicios

- Creación y administración de servicios.
- Asociación de servicios con clientes.
- Definición de tareas y actividades.
- Seguimiento del estado de cada servicio.
- Control de actividades pendientes.

### Confirmaciones

- Solicitud de confirmación de servicios o actividades.
- Registro de respuestas de los clientes.
- Identificación de servicios confirmados, rechazados o pendientes.
- Seguimiento de las confirmaciones pendientes.

### Seguimiento y recordatorios

- Gestión de actividades pendientes.
- Recordatorios para el contador.
- Seguimiento de fechas y vencimientos.
- Identificación de tareas que requieren atención.

### Documentos y soportes

- Organización de documentos relacionados con clientes y servicios.
- Asociación de archivos con actividades específicas.
- Gestión centralizada de soportes necesarios para la prestación de los servicios.

### Automatización

SERKONT está diseñado para permitir la incorporación progresiva de automatizaciones, incluyendo:

- Recordatorios automáticos.
- Notificaciones.
- Flujos de seguimiento.
- Automatización de tareas repetitivas.
- Integraciones con servicios externos.

### Inteligencia artificial

Como parte de su evolución, SERKONT podrá incorporar funcionalidades basadas en inteligencia artificial para asistir al contador en determinadas tareas operativas y de gestión.

Estas funcionalidades serán desarrolladas progresivamente de acuerdo con las necesidades identificadas durante la evolución del proyecto.

## Arquitectura tecnológica

SERKONT utiliza una arquitectura modular orientada a facilitar su evolución, mantenimiento y escalabilidad progresiva.

### Tecnologías principales

- **Aplicación móvil:** React Native + TypeScript + Expo
- **Backend:** Python + Flask
- **Base de datos:** PostgreSQL
- **Contenedores:** Docker
- **Infraestructura:** AWS
- **Control de versiones:** Git + GitHub

## Estructura del proyecto

```text
serkont/
├── backend/
├── mobile/
├── infra/
└── docs/
```

### Backend

Contendrá la API y la lógica de negocio de SERKONT.

### Mobile

Contendrá la aplicación móvil utilizada por los usuarios.

### Infra

Contendrá los archivos y configuraciones relacionados con la infraestructura, despliegue y servicios utilizados por SERKONT.

### Docs

Contendrá la documentación técnica y funcional del proyecto.

## Entorno de desarrollo

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

## Gestión del proyecto

El desarrollo de SERKONT se gestiona mediante GitHub Projects utilizando un flujo Kanban.

### Flujo de trabajo

```text
Backlog → Ready → In Progress → In Review → Done
```

Las actividades se gestionan mediante Issues y se organizan utilizando:

- **Milestones:** representan etapas importantes del proyecto.
- **Etiquetas:** identifican áreas y tipos de trabajo.
- **Issues:** representan actividades concretas.
- **Checklists:** permiten dividir actividades en tareas más pequeñas.
- **Git y GitHub:** gestionan el control de versiones del proyecto.

## Progreso del proyecto

### Milestone 1 — Entorno de desarrollo

- [ ] Preparar WSL2
- [ ] Instalar Ubuntu
- [ ] Configurar usuario de desarrollo
- [ ] Actualizar Ubuntu
- [ ] Configurar repositorio oficial de Docker
- [ ] Instalar Docker Engine
- [ ] Instalar Docker Compose
- [ ] Verificar funcionamiento de Docker
- [ ] Configurar Docker para ejecución sin privilegios de root
- [ ] Configurar Git y GitHub
- [ ] Configurar Visual Studio Code para WSL

### Milestone 2 — Arquitectura inicial

- [ ] Crear estructura inicial de SERKONT
- [ ] Definir arquitectura del backend
- [ ] Definir arquitectura de la aplicación móvil
- [ ] Definir estructura de infraestructura
- [ ] Crear documentación técnica inicial

### Milestone 3 — Backend base

- [ ] Inicializar proyecto Flask
- [ ] Configurar dependencias
- [ ] Configurar PostgreSQL
- [ ] Configurar SQLAlchemy
- [ ] Configurar migraciones
- [ ] Crear estructura de módulos
- [ ] Crear endpoint de prueba

### Milestone 4 — Base de datos

- [ ] Diseñar modelo inicial
- [ ] Crear modelo de usuarios
- [ ] Crear modelo de clientes
- [ ] Crear modelo de servicios
- [ ] Crear modelo de tareas
- [ ] Crear migraciones iniciales

### Milestone 5 — Autenticación y usuarios

- [ ] Implementar registro
- [ ] Implementar inicio de sesión
- [ ] Implementar autenticación mediante JWT
- [ ] Implementar autorización
- [ ] Implementar roles y permisos
- [ ] Crear pruebas de autenticación

### Milestone 6 — Gestión de clientes

- [ ] Crear clientes
- [ ] Consultar clientes
- [ ] Actualizar clientes
- [ ] Eliminar o desactivar clientes
- [ ] Consultar información e historial del cliente

### Milestone 7 — Gestión de servicios

- [ ] Crear servicios
- [ ] Asociar servicios con clientes
- [ ] Definir estados de servicio
- [ ] Consultar servicios
- [ ] Actualizar servicios

### Milestone 8 — Gestión de tareas

- [ ] Crear tareas
- [ ] Asociar tareas con servicios
- [ ] Definir estados
- [ ] Gestionar fechas y vencimientos
- [ ] Gestionar tareas pendientes

### Milestone 9 — Confirmaciones

- [ ] Crear solicitud de confirmación
- [ ] Registrar respuesta del cliente
- [ ] Gestionar estados de confirmación
- [ ] Registrar historial de confirmaciones

### Milestone 10 — Seguimiento y recordatorios

- [ ] Crear recordatorios
- [ ] Gestionar vencimientos
- [ ] Implementar seguimiento de pendientes
- [ ] Implementar notificaciones

### Milestone 11 — Aplicación móvil

- [ ] Inicializar React Native + Expo
- [ ] Configurar TypeScript
- [ ] Crear estructura de navegación
- [ ] Implementar autenticación
- [ ] Implementar gestión de clientes
- [ ] Implementar gestión de servicios
- [ ] Implementar gestión de tareas
- [ ] Integrar aplicación con la API

### Milestone 12 — Pruebas y calidad

- [ ] Configurar framework de pruebas
- [ ] Crear pruebas unitarias
- [ ] Crear pruebas de integración
- [ ] Implementar mocks
- [ ] Validar endpoints
- [ ] Revisar cobertura de pruebas

### Milestone 13 — Infraestructura y despliegue

- [ ] Preparar Docker para SERKONT
- [ ] Configurar entornos
- [ ] Preparar infraestructura AWS
- [ ] Configurar despliegue
- [ ] Configurar variables y secretos
- [ ] Configurar monitoreo

### Milestone 14 — MVP

- [ ] Integrar funcionalidades principales
- [ ] Validar flujo completo contador → cliente
- [ ] Realizar pruebas funcionales
- [ ] Corregir errores críticos
- [ ] Preparar primera versión funcional

## Filosofía del proyecto

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

El proyecto priorizará la construcción de una base sólida antes de incorporar funcionalidades complejas.

## Estado del proyecto

🚧 **En desarrollo**

Actualmente SERKONT se encuentra en la fase inicial de preparación del entorno de desarrollo y construcción de la arquitectura base del proyecto.

## Contribución

Actualmente SERKONT se encuentra en desarrollo.

La estructura, arquitectura y procesos de contribución se definirán y documentarán a medida que el proyecto avance.

## Licencia

Licencia por definir.

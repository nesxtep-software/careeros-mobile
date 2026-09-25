# CareerOS MVP Roadmap

## Overview

Este documento define las fases de desarrollo del MVP de CareerOS, enfocado en la aplicación móvil como punto de entrada principal.

## Fase 1: MVP Core

### Módulo 1: Transición y Estructuración de CV

**Función:** Interfaz de importación y mapeo de perfiles profesionales para reemplazar el formato tradicional en PDF por una estructura digital limpia.

**Alcance:**
- Campos estandarizados de historial laboral
- Roles y responsabilidades
- Tecnologías y herramientas utilizadas
- Período de tiempo en cada posición
- Validación de campos obligatorios

**Features Mínimas:**
- Importación de CV en PDF/Word
- Extracción de datos estructurados
- Interfaz de edición manual
- Validación de datos
- Exportación en formato JSON

**Requerimientos para careeros-core:**
- API de procesamiento de documentos
- Parser de CV (PDF/Word → JSON)
- Validación de estructura de datos
- Normalización de formatos

### Módulo 2: Registro de Tareas Atómicas

**Función:** Bitácora operativa de entrada rápida para registrar actividades diarias, tareas ejecutadas y entregables específicos en tiempo real.

**Alcance:**
- CRUD básico de tareas
- Vinculación al perfil del usuario
- Categorización de tareas
- Registro de fecha y hora
- Estado de completitud

**Features Mínimas:**
- Formulario de entrada rápida
- Lista de tareas recientes
- Edición y eliminación de tareas
- Filtrado por categoría
- Búsqueda de tareas

**Requerimientos para careeros-core:**
- API de gestión de tareas
- Almacenamiento local de datos
- Búsqueda y filtrado
- Sincronización con perfil de usuario

## Fase 2: Post-MVP

### Consolidación Analítica

**Función:** Motor de agrupación de tareas atómicas en logros cuantificables e indicadores de rendimiento métrico.

**Alcance:**
- Agrupación automática de tareas
- Cálculo de métricas de rendimiento
- Identificación de patrones
- Generación de insights
- Visualización de progreso

**Features:**
- Dashboard analítico
- Métricas de productividad
- Tendencias temporales
- Comparativas de rendimiento
- Exportación de reportes

**Requerimientos para careeros-core:**
- Motor de análisis de datos
- Algoritmos de agrupación
- Cálculo de métricas
- Generación de insights
- APIs de análisis

### Capa de Certificación

**Función:** Mecanismo de validación y certificación de ejecuciones laborales históricas por parte de actores autorizados.

**Alcance:**
- Validación de logros
- Certificación por terceros
- Registro de certificaciones
- Verificación de autenticidad
- Permisos y roles

**Features:**
- Sistema de certificación
- Validación de logros
- Firmas digitales
- Registro de audit trail
- Gestión de permisos

**Requerimientos para careeros-core:**
- Sistema de autenticación
- Gestión de permisos
- Almacenamiento de certificaciones
- Validación de firmas
- APIs de certificación

## Priorización

**Fase 1 (MVP):**
1. Módulo 1: Transición y Estructuración de CV
2. Módulo 2: Registro de Tareas Atómicas

**Fase 2 (Post-MVP):**
1. Consolidación Analítica
2. Capa de Certificación

## Notas de Implementación

- La aplicación móvil define los requerimientos de UI/UX
- careeros-core implementa la lógica de negocio y APIs
- Integración entre mobile y core vía APIs o shared packages
- Local-first data storage en todas las fases
- Privacidad y soberanía de datos como principio fundamental

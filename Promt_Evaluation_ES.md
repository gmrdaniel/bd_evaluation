# Prompt para Análisis Comparativo de Bases de Datos de Proyectos

## Contexto y Rol
Actúa como **consultor experto en arquitectura de bases de datos** y **auditor de proyectos de software** con especialización en TypeScript y Supabase. Tu objetivo es realizar un análisis exhaustivo y comparativo de dos proyectos en desarrollo por equipos diferentes.

## Archivos a Analizar
En la carpeta del proyecto encontrarás:
- **Código fuente** de ambos proyectos
- **Diagramas ERD** de las bases de datos
- **Esquemas de base de datos** de ambos proyectos

## Objetivos Principales

### 1. Análisis Comparativo de Bases de Datos
Compara ambos esquemas evaluando:
- **Estructura y normalización**
- **Relaciones entre entidades**
- **Índices y optimizaciones**
- **Escalabilidad y mantenibilidad**
- **Seguridad y control de acceso**

### 2. Análisis FOMO (Fear of Missing Out)
Identifica para cada proyecto:
- **Características críticas ausentes** en comparación con el otro
- **Funcionalidades que podrían comprometer el éxito** del proyecto
- **Oportunidades perdidas** en el diseño actual
- **Riesgos de obsolescencia** técnica

### 3. Evaluación de Componentes Críticos

#### Tablas de Usuarios, Roles y Permisos
- **Expansibilidad**: Capacidad de agregar nuevos roles sin modificar estructura
- **Mantenibilidad**: Facilidad para gestionar permisos y actualizaciones
- **Flexibilidad**: Soporte para roles jerárquicos y permisos granulares
- **Seguridad**: Implementación de principios de menor privilegio

#### Tablas de Campañas
- **Instalabilidad**: Facilidad de configuración en diferentes entornos
- **Funcionalidad**: Completitud de características para gestión de campañas
- **Integrabilidad**: Capacidad de conectar con otros módulos
- **Rendimiento**: Optimización para operaciones frecuentes

## Criterios de Evaluación (Best Practices)

### Desarrollo TypeScript
- **Tipado fuerte** y uso de interfaces
- **Generics** para reutilización de código
- **Decoradores** apropiados para validación
- **Manejo de errores** robusto
- **Patterns** de diseño implementados
- **Testing** y cobertura de código

### Implementación Supabase
**Evaluación basada en mejores prácticas para aplicaciones escalables:**
- **Row Level Security (RLS)** configurado correctamente con policies granulares
- **Policies** de seguridad bien definidas para cada tabla crítica
- **Real-time subscriptions** optimizadas y filtradas apropiadamente
- **Triggers y funciones** de base de datos para lógica de negocio
- **Migraciones** versionadas y reversibles con rollback strategy
- **Edge Functions** cuando sea apropiado para processing distribuido
- **Auth integration** seamless con sistema de roles personalizado
- **Performance monitoring** y optimización de queries
- **Connection pooling** configurado para alta concurrencia

### Arquitectura de Base de Datos
- **Normalización** apropiada (3NF mínimo)
- **Índices** estratégicos para consultas frecuentes
- **Constrains** y validaciones a nivel de BD
- **Auditoría** y logging de cambios
- **Soft deletes** vs hard deletes
- **Particionado** para tablas grandes

## Salida Requerida

### Formato de Entrega
* Tu respuesta debe ser un archivo **`.md`** (Markdown)
* Inicia con un veredicto claro: **¿Cuál de las dos bases de datos es la mejor y por qué?**
* Organiza tu análisis en secciones claras con encabezados (por ejemplo, "Análisis de Normalización", "Revisión de Seguridad y Auditoría", "Compatibilidad con Supabase y TypeScript")
* Utiliza listas y tablas para presentar la información de manera concisa y fácil de digerir

## Estructura de Salida Requerida

### Análisis Individual por Proyecto

#### Proyecto A
**Fortalezas:**
- [Lista detallada de puntos fuertes]

**Debilidades del Modelo de BD:**
- [Identificación específica de problemas estructurales]
- [Limitaciones de escalabilidad]
- [Issues de rendimiento potenciales]
- [Problemas de mantenibilidad]

**Análisis FOMO:**
- [Características ausentes críticas]
- [Riesgos competitivos]

#### Proyecto B
**Fortalezas:**
- [Lista detallada de puntos fuertes]

**Debilidades del Modelo de BD:**
- [Identificación específica de problemas estructurales]
- [Limitaciones de escalabilidad]
- [Issues de rendimiento potenciales]
- [Problemas de mantenibilidad]

**Análisis FOMO:**
- [Características ausentes críticas]
- [Riesgos competitivos]

### Comparación Directa

#### Matriz de Comparación
| Criterio | Proyecto A | Proyecto B | Ganador | Justificación |
|----------|------------|------------|---------|---------------|
| Usuarios/Roles | | | | |
| Campañas | | | | |
| Escalabilidad | | | | |
| Mantenibilidad | | | | |
| Seguridad | | | | |
| Performance | | | | |

### Recomendación Final

#### Proyecto Recomendado: [A/B]
**Justificación:**
- [Razones técnicas específicas]
- [Consideraciones de negocio]
- [Evaluación de riesgos]

#### Plan de Mejoras para el Proyecto Elegido
1. **Mejoras Inmediatas** (Sprint actual)
2. **Mejoras a Mediano Plazo** (Próximos 2-3 sprints)
3. **Mejoras a Largo Plazo** (Roadmap futuro)

#### Lecciones para el Proyecto No Elegido
- [Elementos rescatables para implementación futura]
- [Approach alternativo sugerido]

## Instrucciones de Análisis

1. **Examina** el código fuente de ambos proyectos línea por línea
2. **Analiza** los diagramas ERD en detalle
3. **Evalúa** la implementación de TypeScript y Supabase
4. **Identifica** patrones de diseño utilizados
5. **Compara** métricas de complejidad y mantenibilidad
6. **Valida** la adherencia a best practices
7. **Documenta** todas las observaciones con ejemplos específicos de código
8. **Proporciona** recomendaciones accionables y priorizadas

## Consideraciones Especiales

- **Prioriza la claridad** sobre la brevedad en las explicaciones
- **Incluye fragmentos de código** como evidencia cuando sea relevante
- **Considera el contexto de negocio** además de los aspectos técnicos
- **Evalúa la curva de aprendizaje** para nuevos desarrolladores
- **Analiza el impacto en el time-to-market** de cada approach

---

**Formato de salida:** Documento Markdown (.md) estructurado y bien formateado para fácil lectura y referencia futura.

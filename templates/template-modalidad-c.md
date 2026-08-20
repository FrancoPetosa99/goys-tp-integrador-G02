# Título del Informe

**Grupo:** [Nombre del grupo]
**Integrantes:** [Nombre1, Nombre2, Nombre3, Nombre4]
**Modalidad:** C — Trabajo de Campo
**Fecha:** [Fecha de entrega]

---

## 1. Resumen ejecutivo

[2-3 párrafos describiendo la organización relevada, el alcance del análisis, los hallazgos principales y las mejoras propuestas. Debe poder leerse de forma independiente.]

## 2. Relevamiento de la situación actual

### 2.1. Descripción de la organización

[Tipo de organización (PYME, facultad, organismo público, etc.), tamaño aproximado, sector, cantidad de usuarios/dispositivos en la red. Describir el contexto sin revelar información sensible.]

### 2.2. Topología actual

[Diagrama de la red existente: equipos, conexiones, segmentos, servicios. Incluir como imagen. Si no se pudo acceder a la topología real, describir la topología inferida o la del caso de estudio.]

### 2.3. Inventario de equipamiento

| Equipo | Modelo | Función | Cantidad |
|--------|--------|---------|:--------:|
| Router | [modelo] | [función] | [cantidad] |
| Switch | [modelo] | [función] | [cantidad] |
| Servidor | [modelo] | [función] | [cantidad] |
| Access Point | [modelo] | [función] | [cantidad] |
| [Otro] | [...] | [...] | [...] |

### 2.4. Servicios actuales

[Listar los servicios que presta la red hoy: DHCP, DNS, web, correo, archivos compartidos, VPN, etc. Indicar cómo se implementan actualmente (servidor dedicado, VM, container, etc.).]

## 3. Diagnóstico

### 3.1. Problemas identificados

[Problemas de rendimiento, seguridad, gestión, documentación. Ser específicos: "no hay segmentación entre la red de administración y la red de usuarios" en vez de "la red es insegura".]

### 3.2. Análisis de tráfico (opcional)

[Si se realizaron capturas con Wireshark o similar, incluir hallazgos. Análisis de ancho de banda, protocolos más usados, latencias, pérdida de paquetes. Si no aplica, marcar como "No realizado".]

### 3.3. Evaluación de herramientas actuales

[¿Cómo se gestiona la red hoy? ¿Hay automatización? ¿Hay monitoreo? ¿La documentación está actualizada? ¿Qué herramientas se usan y qué limitaciones tienen?]

## 4. Propuesta de mejora

### 4.1. Diagrama propuesto

[Topología objetivo con los cambios marcados (puede usarse un diagrama con elementos en color diferente para indicar lo nuevo). Incluir como imagen.]

### 4.2. Mejoras de red

[Segmentación propuesta (VLANs, VXLANs), routing (BGP, OSPF), redundancia, mejoras de seguridad. Justificar cada cambio.]

### 4.3. Automatización

[Propuesta de automatización: Ansible, scripts, GitOps. Qué tareas se automatizarían y por qué.]

### 4.4. Monitoreo

[Propuesta de monitoreo: Prometheus, Grafana, alertas. Qué métricas tendría sentido recolectar.]

### 4.5. Plan de implementación

| Fase | Actividades | Duración estimada |
|:----:|-------------|:-----------------:|
| 1 | [actividades] | [días/semanas] |
| 2 | [actividades] | [días/semanas] |
| 3 | [actividades] | [días/semanas] |

## 5. Justificación

[Beneficios esperados de implementar las mejoras. Estimación de costos si es posible. ROI cualitativo: ¿cuánto tiempo se ahorra, qué riesgos se reducen, qué capacidades se ganan?]

## 6. Limitaciones

[Qué no se pudo relevar por falta de acceso, información no disponible, restricciones de la organización. Qué harían diferente si tuvieran más acceso o tiempo.]

## 7. Conclusiones

[Principales aprendizajes del trabajo de campo, relación entre la teoría de la materia y la realidad de la organización relevada.]

## 8. Referencias

- [Documentación técnica consultada]
- [Estándares y RFCs]
- [Referencias de herramientas propuestas]

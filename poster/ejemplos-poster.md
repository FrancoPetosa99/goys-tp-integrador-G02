# Ejemplos de pósters técnico-científicos

## 📌 Pósters IEEE — Formato Conferencia

IEEE tiene un template oficial de póster. Estos son los mejores para entender estructura y densidad de contenido para un póster técnico:

| Ejemplo | Descripción |
|---------|-------------|
| [IEEE Poster Template](https://www.ieee.org/conferences/publishing/templates.html) | Template oficial con estructura de conferencia: introducción, metodología, resultados, conclusiones. Similar a lo que pedimos en GOYS. |
| [NTU IEEE Poster Sample](https://www.ntu.edu.sg/eee/students/current-students/undergraduate-students/fyp/poster) | Ejemplo real de póster de proyecto final. Buena referencia de cómo distribuir diagramas + texto. |

**Qué aprender:** Separación clara entre metodología y resultados. Uso moderado de color (2 colores + fondo).

---

## 📌 NetDev Conference Posters

NetDev es la conferencia de referencia en redes y operación. Sus pósters son los más relevantes para GOYS:

| Ejemplo | Link |
|---------|------|
| [NetDev 0x13 Posters](https://netdevconf.info/0x13/posters.html) | Pósters de la edición 0x13 — temas: XDP, eBPF, routing, VXLAN, SONiC |
| [NetDev 0x14 Posters](https://netdevconf.info/0x14/posters.html) | Pósters con topics de data center, segment routing, network automation |
| [NetDev 0x15 Posters](https://netdevconf.info/0x15/posters.html) | Última edición disponible |

**Qué aprender:** Estos pósters son el estándar de la industria. Mirá cómo presentan topologías de red complejas en espacio limitado. Usan diagramas técnicos densos pero bien etiquetados.

---

## 📌 Ejemplo de la facultad (UTN — GOYS)

### Estructura típica de póster GOYS (nota ≥ 8)

```
┌──────────────────────────────────────────┐
│  IMPLEMENTACIÓN DE UNDERLAY VXLAN CON    │
│  EVPN EN GNS3 + ANSIBLE                  │  ← Título 48pt
│  Grupo 4 — Pérez, García, López          │
├──────────────────────────────────────────┤
│  💡 Contexto: Red de data center con     │
│  alta escalabilidad y segregación de      │
│  tráfico usando VXLAN sobre EVPN.        │
│  Objetivo: 3 tenants aislados con         │
│  movilidad de VM entre spines.            │
├───────────────┬──────────────────────────┤
│               │                           │
│  🌐 Topología │  ⚙️ Implementación       │
│  (3 spines,   │  - Ansible playbooks      │
│   4 leaves,   │  - Roles por dispositivo  │
│   3 tenants)  │  - Jinja2 templates       │
│               │  - Validación con         │
│               │    bats + pytest          │
├───────────────┴──────────────────────────┤
│  📊 Resultados                           │
│  ┌─────────────────┐  ┌───────────────┐  │
│  │ Captura: BGP EVPN│  │ Ping inter-   │  │
│  │ route exchange   │  │ tenant: ✅ OK │  │
│  └─────────────────┘  └───────────────┘  │
│  Convergencia: < 2s ante fallo de leaf    │
├──────────────────────────────────────────┤
│  Conclusión: VXLAN+EVPN funciona en      │
│  entornos multi-tenant con ANSIBLE        │
├──────────────────────────────────────────┤
│  📎 github.com/grupo4-goys              │
│  [QR code]                                │
└──────────────────────────────────────────┘
```

**Elementos clave:**
- Título específico (no "Trabajo de redes" — decí qué hiciste)
- Diagrama de red con nombres/números de dispositivos
- Resultados con capturas reales
- QR funcional

Lo que separa un 8 de un 10: claridad del diagrama, calidad de las capturas, conclusiones con métricas concretas.

---

## 📌 Antes vs. Después

### ❌ Póster malo

```
┌──────────────────────────────────────────┐
│          Redes y Gestión                 │  ← 24pt, no se lee
│          Grupo 7                         │
├──────────────────────────────────────────┤
│  En este trabajo realizamos una          │
│  investigación exhaustiva sobre          │  ← Párrafo de 15 líneas
│  diferentes tecnologías de redes         │     nadie lo va a leer
│  entre las cuales se encuentran          │
│  VXLAN, EVPN, BGP, OSPF, etc.           │
│  El objetivo fue analizar... (sigue)     │
├──────────────────────────────────────────┤
│  [texto] │ [más texto] │ [más texto]    │  ← 3 columnas iguales
│  ...      │  ...        │  ...           │     sin estructura
│  [texto] │ [más texto] │ [más texto]    │
├──────────────────────────────────────────┤
│  Conclusión: aprendimos mucho.           │  ← Sin métricas
└──────────────────────────────────────────┘
```

**Problemas:**
- Título genérico
- Pared de texto
- Sin diagrama de red
- Sin resultados concretos
- 3 columnas sin jerarquía
- Conclusión vacía

### ✅ Póster bueno

```
┌──────────────────────────────────────────┐
│  AUTOMATIZACIÓN DE FABRIC VXLAN/EVPN     │  ← 48pt
│  CON ANSIBLE EN ESCENARIO MULTI-TENANT   │
│  Grupo 7 — Rodríguez, Suárez, Medina     │
├──────────────────────────────────────────┤
│  💡 Problema: Configurar manualmente     │  ← 2 líneas
│  12 leaves + 4 spines es propenso a      │
│  errores. Solución: Ansible + VXLAN.      │
├────────────────┬─────────────────────────┤
│  🌐 Topología  │  ⚙️ Stack               │
│  [diagrama con │  - GNS3: 16 nodos        │  ← Bullet points
│   spines,      │  - Ansible: 12 playbooks  │
│   leaves,      │  - Wireshark: capturas    │
│   servers]     │  - Python: validador     │
├────────────────┴─────────────────────────┤
│  📊 Resultados                           │
│  ┌──────────┐  ┌──────────┐  ┌────────┐ │
│  │ Antes:   │  │ Después: │  │ Mejora │ │
│  │ 45 min   │  │ 3 min    │  │ 15x    │ │
│  │ manual   │  │ ansible  │  │        │ │
│  └──────────┘  └──────────┘  └────────┘ │
├──────────────────────────────────────────┤
│  🎯 Conclusión: Automatizar VXLAN/EVPN   │
│  reduce errores en 90% y tiempo en 15x.   │
├──────────────────────────────────────────┤
│  [QR]  github.com/grupo7-goys            │
└──────────────────────────────────────────┘
```

**Por qué funciona:**
- Título que dice exactamente qué hicieron
- Problema → Solución en 2 líneas
- Diagrama de red + stack tecnológico
- Resultados con **comparativa antes/después** (métrica concreta)
- Conclusión con número (`15x`, `90%`)

---

## 📌 Referencias adicionales

| Recurso | Link | Para qué sirve |
|---------|------|----------------|
| Better Posters blog | https://betterposters.blogspot.com | Todo sobre diseño de pósters académicos (en inglés) |
| Colin Purrington's guide | https://colinpurrington.com/tips/poster-design | La guía más completa sobre diseño de pósters científicos |
| Canva Poster Templates | https://www.canva.com/posters/templates | Templates editables (buscá "academic poster" o "scientific") |
| Overleaf Poster Templates | https://www.overleaf.com/gallery/tagged/poster | Templates LaTeX para póster científico |
| draw.io network shapes | https://app.diagrams.net | Diagramas de red profesionales |

# Título del Proyecto

**Grupo:** [Nombre del grupo]
**Integrantes:** [Nombre1, Nombre2, Nombre3, Nombre4]
**Modalidad:** A — Proyecto de Desarrollo
**Fecha:** [Fecha de entrega]

---

## 1. Resumen ejecutivo

[2-3 párrafos que describan qué hicieron, por qué, y qué resultados obtuvieron. Incluir el problema que resolvieron, la solución implementada y los principales hallazgos o métricas.]

## 2. Arquitectura de la solución

### 2.1. Diagrama de red

[Incluir diagrama de la topología: equipos, conexiones, direcciones IP, VLANs, VXLANs, segmentos. Puede ser generado con draw.io, excalidraw, o similar. Incluir como imagen.]

### 2.2. Componentes

| Componente | Tecnología | Función |
|------------|------------|---------|
| Router | MikroTik RouterOS | Gateway BGP, NAT, routing |
| Spine-Leaf | GNS3 + Alpine Linux | Conectividad del data center |
| VXLAN | Linux VTEPs | Segmentación L2 sobre L3 |
| Containers | Docker / K3s | Servicios y aplicaciones |
| Automatización | Ansible | Gestión de configuraciones |
| Monitoreo | Prometheus + Grafana | Métricas y alertas |
| Seguridad | Network Policies / Cilium / mTLS | Segmentación y aislamiento del tráfico |
| [Otro] | [...] | [...] |

### 2.3. Flujo de datos

[Explicar cómo viaja un paquete desde un cliente externo hasta el servicio final, pasando por cada componente de la arquitectura. Incluir protocolos involucrados en cada salto.]

## 3. Implementación

### 3.1. Configuración de red

[Detalle de direcciones IP, VLANs, VXLANs, BGP, OSPF. Incluir fragmentos de configuración relevantes.]

### 3.2. Container networking

[Deployments, services, network policies. Explicar cómo se segmentó el tráfico y cómo se aislaron los servicios.]

### 3.3. Automatización

[Playbooks de Ansible, templates, variables, inventarios. Mostrar cómo se automatizó la configuración de los equipos de red.]

### 3.4. Monitoreo

[Dashboards creados, métricas recolectadas, alertas configuradas. Incluir capturas de pantalla de Grafana.]

## 4. Verificación

### 4.1. Pruebas de conectividad

[Pings, traceroutes, capturas de Wireshark que demuestren que la red funciona según lo diseñado.]

### 4.2. Pruebas de segmentación

[Demostrar qué tráfico está permitido y qué tráfico está bloqueado entre los diferentes segmentos/namespaces.]

### 4.3. Pruebas de automatización

[Mostrar que los playbooks de Ansible se ejecutan correctamente, que los backups se realizan, que las configuraciones son idempotentes.]

## 5. Limitaciones y trabajo futuro

[Qué no pudieron hacer por tiempo, recursos o complejidad. Qué harían diferente si volvieran a empezar. Qué mejoras le harían al proyecto.]

## 6. Conclusiones

[Qué aprendieron, qué fue lo más difícil, qué fue lo más interesante, cómo se distribuyó el trabajo en el grupo.]

## 7. Referencias

- [Bibliografía]
- [RFCs consultados]
- [Documentación técnica]
- [Tutoriales o guías utilizadas]

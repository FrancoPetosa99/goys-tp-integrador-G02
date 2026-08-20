# Cómo armar el póster A1 en PowerPoint / Google Slides

## 1. Configurar tamaño A1

### PowerPoint
1. **Diseño → Tamaño de diapositiva → Tamaño personalizado**
2. Ancho: **594 mm** | Alto: **841 mm**
3. Orientación: **Vertical**
4. Aceptar → "Ajustar" (no "Maximizar")

### Google Slides
1. **Archivo → Configurar página**
2. Personalizado → **1122,5 × 1587,5 px** (es el equivalente a 594×841mm a 48ppp)
   - Si tu slide está en cm: **59,4 × 84,1 cm**
3. Aplicar

> ⚠️ **Tip:** Si vas a imprimir, configurá el tamaño en **mm**, no en px. PowerPoint y Slides redondean, pero se acerca.

---

## 2. Guías de diseño

Una vez configurado el tamaño A1, agregá guías visuales para mantener el margen:

| Elemento | Margen / Tamaño |
|----------|----------------|
| Margen general | **25-35 mm** en cada borde |
| Título (header) | Ocupa el **15-20%** superior |
| Contenido | El **65-70%** central |
| Footer | El **8-10%** inferior |

**Pasos:**
1. Insertá un rectángulo del tamaño del slide
2. Sin relleno, borde punteado gris claro
3. Ajustale un margen interno de 30 mm
4. Usalo como guía para todo el contenido

---

## 3. Estructura del slide (vertical)

| Zona | Altura aprox. | Contenido |
|------|:-------------:|-----------|
| **Header** | 180 mm | Título grande (48-60pt), grupo, integrantes. Fondo oscuro con texto blanco. |
| **Introducción** | 120 mm | 2-3 líneas de contexto + objetivo. Fondo claro o borde lateral. |
| **Diagrama + Metodología** | 280 mm | Dos columnas: izquierda → diagrama de red; derecha → bullet points de herramientas y proceso. |
| **Resultados** | 200 mm | Ancho completo. Capturas, tablas, gráficos. Podés poner 2-3 columnas. |
| **Footer** | 60 mm | QR al repo, mail del grupo, datos de la cátedra. Fondo oscuro. |

---

## 4. Insertar diagramas

### Draw.io
1. Hacé el diagrama en draw.io
2. **Archivo → Exportar → PNG**
3. Configurá: escala **300 ppp**, fondo transparente o blanco
4. Insertalo en la diapositiva

### Excalidraw
1. Hacé el diagrama
2. **Export → PNG** con fondo blanco
3. Insertar en el slide

### Screenshots de laboratorio
- Capturá con **ventanas limpias** (sin barras de herramientas, sin otras apps abiertas)
- Si es un terminal: usá `script` o `tmux capture-pane` para captura limpia
- Preferí **dark mode** en los terminals (se ve más profesional)

---

## 5. QR al repositorio

1. Andá a [qrcode-monkey.com](https://www.qrcode-monkey.com) o usá `qrencode`:
   ```bash
   qrencode -s 10 -o qr-repo.png "https://github.com/tu-org/tu-repo"
   ```
2. Tamaño en el póster: **30-40 mm** de lado
3. Ponelo en el footer, abajo a la derecha

---

## 6. Texto: tamaño mínimos

| Elemento | Tamaño mínimo |
|----------|:-------------:|
| Título del proyecto | **48 pt** |
| Subtítulos de sección | **36 pt** |
| Cuerpo de texto | **24 pt** |
| Footer / referencias | **20 pt** |

Regla de oro: si no se lee desde 1 metro, es muy chico.

---

## 7. Exportar a PDF

### PowerPoint
1. **Archivo → Exportar → Crear PDF**
2. Opciones: "Calidad de impresión" (no "Mínima")
3. Asegurate de que esté en **A1**

### Google Slides
1. **Archivo → Descargar → Documento PDF (.pdf)**
2. Verificá que la escala sea 1:1

### Verificación
- Abrí el PDF y hacé zoom al 100%
- Si se ve borroso o pixelado, las imágenes están a baja resolución
- Las imágenes deben tener al menos **200-300 ppp**

---

## 8. Impresión

### Centro de copiado / Plotter
- Pedí **A1 vertical** (594 × 841 mm)
- Papel recomendado: **fotográfico satinado** o **bond 120-150 g**
- No uses papel común de 80g — se transparenta
- Color: **full color**

### Antes de imprimir
- [ ] Revisé que no haya bordes blancos raros
- [ ] Verificá que las imágenes no estén pixeladas
- [ ] Comprobá que el QR escanee bien desde 30 cm
- [ ] Pedí **una sola copia de prueba** en A3 primero
- [ ] Si todo bien, mandá a imprimir en A1

### Margen de corte
Si usás servicio de impresión con sangría:
- Dejá **5 mm extra** en cada borde para sangría
- Los elementos importantes (texto, QR) adentro de los **30 mm** de margen seguro

---

## 9. Checklist final

- [ ] Tamaño configurado como **594 × 841 mm** (A1)
- [ ] Orientación **vertical**
- [ ] Título visible desde 3 m (≥ 48pt)
- [ ] Mínimo de texto, máximo de diagramas
- [ ] QR al repositorio insertado y escaneable
- [ ] Exportado a **PDF**
- [ ] Impresión de prueba en A3 antes del A1 final
- [ ] Las imágenes tienen alta resolución (≥ 200 ppp)
- [ ] El poster se entiende sin que alguien lo explique

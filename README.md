# Be Held — landing page

Landing de *Be Held*, círculo grupal de sanación en agua con Rocío Navarro (tres horas, 4 a 8 personas, agua a temperatura corporal).
Copy tomado del documento `BE HELD LANDIG PAGE COPY.docx`. Proyecto hermano de `submerge-in-silence`.

---

## 1. Cómo verlo

**Opción A — Live Server (VS Code)**
1. Abre la carpeta `be-held` en VS Code.
2. Con la extensión *Live Server*, clic derecho en `index.html` → **Open with Live Server**.

**Opción B — servidor estático**

```bash
python -m http.server 5513
```

Luego abre `http://localhost:5513`.

---

## 2. Estructura

```
be-held/
├── index.html          — hero + franja de datos + 7 secciones + cierre + barra de reserva fija
├── css/styles.css      — sistema de diseño (idéntico al de submerge) + bloque "Nervous"
├── js/water.js         — hero WebGL (Three.js), paleta cálida
├── js/main.js          — loader, smooth scroll, GSAP, menú, contador del carrusel
├── assets/img/         — springs-sunset.webp, springs-day.webp, placeholder-water.svg
└── README.md
```

Dependencias por CDN (sin build): GSAP 3.12 + ScrollTrigger, Three.js r128, Lenis 1.1, Marcellus + PT Serif.

---

## 3. Sistema de diseño

Hereda el sistema de **rocionavarro.org** (mismos tokens y tipografías que `submerge-in-silence`).
La única diferencia visual es el shader del hero, que usa una paleta cálida (agua a temperatura corporal):
`#211C19` (profundo) · `#4A4038` (medio) · `#C9B49C` (luz).

---

## 4. Pendientes

1. **Testimonio (SECTION 7 del docx).** Sigue en `[FALTA]`. La banda de cita usa provisionalmente una línea del propio copy
   («No one in this circle is only a spectator.») y está marcada con un comentario `PENDIENTE` en `index.html`.
2. **Fotos.** No hay fotos propias de Be Held. Se reutilizan dos imágenes de agua del otro proyecto
   (`springs-sunset.webp`, `springs-day.webp`); conviene sustituirlas por fotos de un círculo en piscina, con los mismos nombres de archivo.
3. **SECTION 3 duplicada.** El docx traía la sección «Why this happens in a group» dos veces (borrador y versión ampliada). Se usó la versión ampliada.
4. **Precio del círculo privado.** Hoy dice «On request». Confirmar si debe llevar una cifra.

# Navegante — Sitio web

Sitio web de **Navegante Publicidad**, agencia digital en Monterrey, N.L.
Hecho a mano (HTML/CSS/JS), sin WordPress, para que sea rápido y fácil de mantener.

Concepto de diseño: **carta de navegación digital / chartplotter**. La página es una
travesía: el negocio del cliente zarpa y lo llevamos "a buen puerto" pasando por
web → publicidad → IA.

---

## Cómo abrirlo y editarlo

1. Abre esta carpeta en **Visual Studio Code** (Archivo → Abrir carpeta).
2. Para verlo en el navegador mientras editas, lo más cómodo es la extensión
   **Live Server** (instálala en VS Code, luego clic derecho sobre `index.html` →
   "Open with Live Server"). También puedes solo hacer doble clic en `index.html`.
3. Todo el sitio está en un único archivo `index.html` (HTML, CSS y JS juntos).
   - El **CSS** está dentro de la etiqueta `<style>` arriba.
   - El **JavaScript** está dentro de `<script>` hasta abajo.

> Tip: si más adelante quieres separar el CSS y el JS en archivos aparte
> (`styles.css`, `script.js`), se puede hacer fácil. Por ahora un solo archivo
> es lo más simple para arrancar.

---

## Estructura del archivo (secciones)

| Sección | id | Qué es |
|---|---|---|
| Menú (nav) | — | Barra fija; transparente sobre el hero, se vuelve clara al hacer scroll |
| Hero | — | Titular + chartplotter animado (SVG) |
| Servicios | `#servicios` | 6 tarjetas (la de IA es la destacada) |
| Por qué Navegante | `#porque` | Sección oscura con el diferenciador (IA) |
| Travesía / Proceso | `#proceso` | 4 tramos del proceso |
| Para quién | — | Tipos de negocio (chips) |
| Contacto | `#contacto` | Formulario que abre WhatsApp + datos directos |
| Footer | — | Logo, redes, contacto |

---

## Datos de contacto (ya están puestos en el sitio)

- **WhatsApp:** 81 8690 4286  → en el código se usa el formato `528186904286`
  (variable `WHATSAPP` en el `<script>`).
- **Correo:** luis.corona@navegantepublicidad.com
- **Ubicación:** Monterrey, Nuevo León.

El formulario de contacto NO envía correos: arma un mensaje y abre WhatsApp con
el texto listo para enviar.

---

## Pendientes (lo que falta)

- [ ] **Redes sociales:** los enlaces de Instagram, Facebook, TikTok y LinkedIn
      están en `#` (vacíos). Buscar en `index.html` los `aria-label="Instagram"`,
      etc., y poner la URL real. Quitar las que no se usen.
- [ ] **Ubicación / mapa:** el renglón de "Ubicación" en contacto está en `#`.
      Si quieres, poner liga a Google Maps.
- [ ] Revisar/afinar textos a tu estilo.
- [ ] (Opcional) Dominio + hosting para publicarlo.
- [ ] (Opcional) Separar CSS y JS en archivos propios.

---

## Notas técnicas

- **Tipografías** (Google Fonts, se cargan por internet): Space Grotesk (títulos),
  Hanken Grotesk (texto), Space Mono (etiquetas tipo coordenadas).
- **Iconos:** Tabler Icons vía CDN (jsdelivr).
- El logo del menú y del footer es **vectorial** (SVG dibujado en el HTML: olas +
  "Navegante"), así se adapta solo a fondo claro u oscuro. No usa imagen PNG.
- Responsive (celular, tablet, escritorio) y respeta `prefers-reduced-motion`.
- La paleta y el sistema de diseño completos están en `marca.md`.

---

_Última actualización: junio 2026._

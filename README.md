# match-aniversario

Landing page del 10° aniversario de Match, agencia digital chilena.

## Concepto
"10 años orquestando el futuro digital" — Estructura no convencional donde el diagnóstico interactivo ES el hero: el usuario identifica su propio problema antes de que Match se presente como la solución.

## Stack
- Next.js
- Tailwind CSS
- Deploy: Vercel

## Identidad Visual

### Paleta de colores
| Token | Valor | Uso |
|---|---|---|
| Background primary | `#0A0F1E` / `#0D1B2A` | Fondo principal dark navy |
| Background secondary | `#111827` | Fondo secundario |
| Accent / CTA | `#00B4D8` / `#0EA5E9` | Botones, selecciones, highlights |
| Text primary | `#FFFFFF` | Títulos y texto principal |
| Text secondary | `#94A3B8` | Subtítulos y texto de apoyo |
| Surface cards | `#1E293B` | Fondo de tarjetas |
| Border / dividers | `#1E3A5F` | Bordes sutiles |

### Tipografía
- Fuente: **Inter** (headings y body)
- H1: 56-64px / H2: 40px / H3: 28px / Body: 16-18px
- Heading weight: 700-800 | Body weight: 400-500
- Letter spacing headings: `-0.02em`
- Line height: 1.4 headings / 1.6 body
- All caps solo para labels/badges pequeños

### Estilo visual
- Dark mode throughout
- Minimal, mucho espacio en blanco
- Gradientes sutiles dark blue → black
- Sin texturas pesadas
- Border radius cards y botones: 8-12px
- Botones CTA: solid electric blue con hover glow
- Iconos: line icons monocromáticos o en accent blue

## Estructura de Secciones

### Section 1 — Hero
- Headline: *"¿Tu empresa tiene todo lo digital... pero no funciona como un todo?"*
- Subheadline: *"Responde 3 preguntas. Te mostramos exactamente dónde está el problema."*
- CTA: "Comenzar diagnóstico" (electric blue, centrado)
- Badge: "10 años | +40 empresas | Copec · Zurich y más"
- Sin nav, sin logo clutter

### Section 2 — Quiz (3 pasos, fullscreen)
- Progress bar animada (electric blue, 2px)
- Transición fade entre preguntas
- Cards auto-avanzan al seleccionar

**Step 1/3** — Industria:
Retail/E-commerce · Servicios financieros · Salud · Educación · Energía · Tecnología/SaaS · Otra

**Step 2/3** — Mayor desafío digital:
Sitio no convierte · Canales no integrados · Sin visibilidad de datos · Incorporar IA

**Step 3/3** — Tamaño empresa:
50-200 · 200-500 · 500+

### Section 3 — Resultado personalizado
Lógica de personalización según respuestas:
- Energía/Infraestructura → Caso Copec: +4M usuarios, migración headless, TOP 2 Chile
- Financiero/Seguros → Caso Zurich: orquestación completa de experiencia digital
- Tecnología + dolor IA → Caso 6i.AI: IA integrada en cada fase
- Default → +40 empresas transformadas en 10 años

### Section 4 — Credibility bar
"10 años · +40 empresas · Una metodología" + 6 placeholders de logos clientes

### Section 5 — Formulario + CTA
- Headline: *"Tu diagnóstico ya empezó. Ahora lo completamos juntos."*
- Badge escasez: "Solo 10 cupos disponibles este mes"
- Campos: Nombre · Empresa · Cargo · Email corporativo · Teléfono
- CTA: "Completar mi diagnóstico"
- Microcopy: *"Sin compromiso. Un estratega de Match te contacta en menos de 24 horas."*

### Section 6 — Confirmación post-submit
- Checkmark animado SVG (draw-in, electric blue)
- Headline: "Listo."
- Subtext: *"Un estratega de Match revisó tus respuestas antes de llamarte."*

## Responsive
- Mobile first
- Quiz cards: 1 columna mobile / 2 columnas desktop
- Hero H1: 36px mobile / 56px desktop
- Form: full width mobile

## Animaciones
- Smooth scroll entre secciones
- Fade-in on section entry
- Quiz card: scale hover + blue glow on selection
- Progress bar animada por step
- Confirmación: SVG draw-in checkmark

## Notas técnicas
- Sin dependencias de imágenes externas (CSS/SVG only)
- Todo el texto en español
- **Sin localStorage ni sessionStorage**
- Estado del quiz manejado con React useState
- Respuestas del quiz en memoria para personalizar resultado

---
name: Clínica Dental Serena
description: Vidriera dental ficticia, luminosa y serena.
colors:
  bg: "#F7FAFA"
  ink: "#123B4F"
  blue: "#2A7AB0"
  mint: "#9AD1C8"
  paper: "#fff"
  soft: "#EAF4F3"
typography:
  display:
    fontFamily: "Sora, sans-serif"
    fontSize: "66px"
    fontWeight: 500
    lineHeight: 1.09
    letterSpacing: "-.025em"
  headline:
    fontFamily: "Sora, sans-serif"
    fontSize: "40px"
    fontWeight: 500
    lineHeight: 1.16
    letterSpacing: "-.025em"
  title:
    fontFamily: "Sora, sans-serif"
    fontSize: "24px"
    fontWeight: 500
    lineHeight: 1.16
    letterSpacing: "-.025em"
  body:
    fontFamily: "Manrope, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.65
  label:
    fontFamily: "Manrope, sans-serif"
    fontSize: "14px"
    fontWeight: 600
    lineHeight: 1.5
rounded:
  surface: "16px"
  comparison: "24px"
  comparison-mobile: "18px"
  hero: "24px 6px 24px 6px"
  pill: "999px"
  circle: "50%"
spacing:
  inset-mobile: "24px"
  inset-desktop: "32px"
  gutter-desktop: "40px"
  gutter-tablet: "28px"
  gutter-mobile: "22px"
  section-desktop: "100px"
  section-mobile: "70px"
components:
  button-primary:
    backgroundColor: "{colors.blue}"
    textColor: "{colors.paper}"
    rounded: "{rounded.pill}"
    padding: "14px 23px"
  button-primary-hover:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.paper}"
  button-secondary:
    backgroundColor: "{colors.soft}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "14px 23px"
  button-secondary-hover:
    backgroundColor: "{colors.mint}"
    textColor: "{colors.ink}"
  filter:
    backgroundColor: "{colors.soft}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "10px 19px"
  filter-selected:
    backgroundColor: "{colors.blue}"
    textColor: "{colors.paper}"
  treatment:
    backgroundColor: "{colors.paper}"
    rounded: "{rounded.surface}"
    padding: "27px 30px 30px"
  price-list:
    backgroundColor: "{colors.paper}"
    rounded: "{rounded.surface}"
    padding: "{spacing.inset-desktop}"
---

# Design System: Clínica Dental Serena

## Overview

**Creative North Star: "Serena"**

Una identidad familiar, luminosa y serena. La tinta petróleo sostiene la
lectura sobre fondos claros; azul y menta acompañan fotografías de consultorio
y atención clínica. Los titulares geométricos se combinan con texto espacioso.

Las superficies planas se separan por tono y espacio. Los controles redondos
ofrecen acciones claras y las fotografías conservan protagonismo sin efectos
de vidrio, gradientes ni sombras decorativas.

**Key Characteristics:**

- Fotografías luminosas y lectura en tinta petróleo.
- Titulares Sora y texto Manrope.
- Superficies planas y controles redondos.
- Foco visible y alternativa de movimiento reducido.

Este documento se escribió inicialmente **antes de index.html**, por pedido
explícito del usuario. Esta revisión conserva esa intención y reconcilia
los valores provisionales con el código final y las capturas de escritorio
y celular. La implementación fue dirigida desde código; no hay composición
visual aprobada ni QUALITYBAR externo al que atribuir sus decisiones.

## Colors

Las claves y valores normativos están en el frontmatter y corresponden a las
variables de index.html.

### Primary

- **Azul sereno** (`blue`): acciones, filtros seleccionados, foco,
  manija del comparador y sección de cierre.
- **Menta** (`mint`): franja de datos, selección de texto y estados suaves;
  también créditos sobre el footer oscuro.

### Neutral

- **Fondo Serena** (`bg`): página y header sólido.
- **Tinta petróleo** (`ink`): texto, marca, etiquetas oscuras y footer.
- **Papel** (`paper`): tarjetas, lista de precios y texto sobre azul.
- **Bruma menta** (`soft`): secciones de apoyo y controles secundarios.

**The Ink Reading Rule.** El texto corrido usa tinta sobre fondos claros;
las superficies menta no reciben texto azul de bajo contraste.

## Typography

**Display Font:** Sora (con sans-serif de respaldo).
**Body Font:** Manrope (con sans-serif de respaldo).

Los titulares usan peso medio y tracking compacto; Manrope reserva pesos
más altos para navegación y controles. Los roles base están en el frontmatter.

### Hierarchy

- **Display:** H1 final de 66 px en escritorio; hasta 1100 px mide 50 px y
  hasta 900 px, 43 px. Hasta 600 px cambia su interlínea de 1.09 a 1.12.
  Estos valores reemplazan el H1 provisional del documento inicial.
- **Headline:** H2 base del frontmatter; hasta 600 px mide 32 px con
  interlínea 1.18. El cierre tiene un ajuste propio de 52 px, interlínea 1.1,
  y 36 px en celular.
- **Title:** H3 base del frontmatter. Tratamientos pasa a 23 px en celular;
  equipo y precios tienen ajustes locales y no constituyen otra escala general.
- **Body:** párrafos con límite general de 65ch. Hero usa 17 px en escritorio
  y 16 px desde 900 px. Tratamientos, visita, FAQ y condición de precios
  mantienen 16 px.
- **Label:** navegación y filtros; metadatos y ayudas pueden usar 13 px.
  Botones con peso 700.

## Layout

Marco común de hasta 1220 px con los gutters del frontmatter: escritorio,
tablet hasta 900 px y celular hasta 600 px. Header pegajoso de 80 px, luego
76 px desde 900 px; separación de anclas de 104 px.

Las secciones regulares usan los espacios de sección del frontmatter.
Hero, FAQ, cierre y footer tienen ajustes propios. Tratamientos tiene dos
columnas; equipo, tres; pasos de visita, dos. Se apilan hasta 600 px.
Comparador, visita, precios y FAQ se apilan desde 900 px.

El hero implementado distribuye texto y fotografía en dos columnas; en
celular texto y acciones preceden a la foto. Los filtros tienen desplazamiento
horizontal propio. Las fotos varían en tamaño dentro del marco común.
Footer reserva 6rem inferiores para despejar el acceso flotante.

Sin JS, el menú móvil permanece visible en filas legibles y las anclas
reciben mayor separación para ese header expandido.

## Elevation & Depth

No hay sombras. La profundidad procede de papel sobre el fondo tenue,
secciones de bruma menta y bloques de tinta o azul. El header es sólido.

**The Flat Surface Rule.** Separar por tono, espacio y jerarquía antes que
añadir sombra.

## Shapes

El radio de superficie del frontmatter se aplica a tratamientos, fotos de
equipo y **una única lista de precios**. La evaluación sin cargo es su primera
fila: sin tarjeta interior, fondo propio ni radio anidado.

Hero combina esquinas amplias y cortas alternadas; el comparador tiene radio
propio y variante móvil. Botones, filtros y etiquetas son píldoras; manija
y acceso flotante son círculos. Los iconos de acciones son SVG de línea.
WhatsApp usa el símbolo de marca de Bootstrap Icons, relleno en currentColor
y sin trazo agregado; en el flotante su caja es de 27 × 27 px sin encogimiento.
Fuente y licencia MIT: THIRD-PARTY-LICENSES.txt.

## Components

### Buttons

Estados principal, secundario y hover en el frontmatter. Alto mínimo de
52 px; hasta 600 px, 49 px, texto 13 px y padding horizontal 19 px.
Una sola línea. Hover desplaza 2 px hacia arriba durante 0.2 s; active vuelve
a su posición. Foco común: contorno azul de 3 px con separación de 5 px.

En el cierre, botón principal papel/tinta y secundario tinta/papel.
Hay tres accesos de WhatsApp: hero, cierre y flotante, todos al placeholder
5491100000000.

### Chips

Cinco filtros: Todos, Prevención, Estética, Ortodoncia, Implantes y prótesis.
Alto mínimo 44 px; selección por `aria-pressed`, azul/papel; hover menta.
Actualizan ocho tarjetas sin recarga y anuncian el conteo. Sin JS se muestran
las ocho tarjetas y se ocultan los filtros.

### Cards / Containers

Ocho tratamientos: dos fotográficos y seis de lectura. Nombre, explicación,
«Para vos si…» y grupo. El padding de cuerpo pasa a 24 px en celular;
fotos de 235 px de alto en escritorio y 220 px en celular.

La lista de precios tiene una sola superficie papel con radio de superficie,
padding 32 px en escritorio y 24 px en celular. Primera fila: evaluación
sin cargo. Luego limpieza desde $45.000 y blanqueamiento desde $180.000.
La condición del presupuesto por escrito permanece visible a 16 px.
Son importes ficticios de la demostración, sin checkout ni integración de pagos.

**The Single Price Surface Rule.** Evaluación e importes comparten una
superficie plana; la primera fila no se convierte en una segunda tarjeta.

### Navigation

Serena con descriptor Clínica dental y cuatro anclas. El header muestra
la S de marca sobre menta; el favicon es una S geométrica vectorial blanca
sobre azul en assets/favicon.svg. Navegación: 14 px, peso 600, subrayado al
hover. Desde 900 px, control de menú de 44 × 44 px con estado expandido.
Escape cierra y devuelve el foco cuando corresponde; un ancla también cierra.
La alternativa sin JS permanece legible.

### Comparador de simulación

Misma foto en ambos lados, proporción 4:3, etiquetas fijas Antes/Después,
divisor de 4 px y manija de 60 px con flechas SVG. Recorte por posición,
arrastre con captura de puntero y slider ARIA: rango 0–100, inicio 50,
flechas en pasos de 4, Home/End y valor ARIA actualizado.
La descripción accesible enlaza la aclaración visible de simulación.

### Equipo, visita y FAQ

Tres perfiles ficticios y nota ilustrativa visible. Cuatro pasos numerados
en grilla, luego lista vertical móvil. Seis FAQ con details/summary nativos,
SVG más que gira al abrir y respuestas de 16 px.

### Movimiento

Una entrada coordinada del hero, sin ocultar contenido posterior: foto
con escala 1.035 y opacidad 0.8 durante 1.05 s; título desde 12 px durante
0.7 s; acciones desde 7 px durante 0.5 s. Easing power2.out.
GSAP 3.12.5 y ScrollTrigger más Lenis 1.1.14 por CDN; Lenis usa duración 0.9.
Menú, filtros y comparador no dependen de esas librerías.
Movimiento reducido evita entradas y scroll suavizado, y elimina transiciones.
Sin autoplay ni video de fondo.

## Do's and Don'ts

### Do:

- **Do** mantener Sora en titulares y Manrope en lectura.
- **Do** separar superficies planas con espacio y diferencias de tono.
- **Do** conservar foco visible, teclado y movimiento reducido.
- **Do** mantener la evaluación como primera fila de la única lista de precios.
- **Do** rotular el comparador como simulación de la misma foto y conservar su crédito.

### Don't:

- **Don't** añadir gradientes, vidrio, sombras decorativas ni iconos de emoji.
- **Don't** usar azul para texto corrido sobre menta.
- **Don't** presentar fotografías, personas o datos ficticios como evidencia clínica real.
- **Don't** describir la simulación digital como resultado clínico o promesa de tratamiento.

## Fotografías y procedencia

Fotos libres de Pexels, descargadas y optimizadas a WebP en assets/.
Licencia: https://www.pexels.com/license/ . No se presentan como instalaciones,
equipo ni resultados propios reales de Serena. Son material ilustrativo de
una marca ficticia. Se revisan marcas, letras ajenas y caras frontales.

| Archivo | Uso | Autor y fuente |
|---|---|---|
| hero-consultorio.webp | Hero luminoso, reencuadre hacia sillón azul | Tima Miroshnichenko — https://www.pexels.com/photo/a-clinic-with-dental-equipment-5355920/ |
| tratamiento-control.webp | Tarjeta Limpieza y control, atención de perfil | Cedric Fauntleroy — https://www.pexels.com/photo/a-dentist-checking-the-woman-s-teeth-4270362/ |
| tratamiento-estetica.webp | Tarjeta Blanqueamiento, sonrisa | Kindel Media — https://www.pexels.com/photo/close-up-photo-of-person-s-smile-7298633/ |
| equipo-paula.webp | Trabajo clínico, mirada baja | Andrea Piacquadio — https://www.pexels.com/photo/young-female-dentist-treating-teeth-of-patient-in-modern-clinic-3881238/ |
| equipo-martin.webp | Odontólogo trabajando, rostro cubierto y mirando al paciente | Pavel Danilyuk — https://www.pexels.com/photo/man-at-a-dentists-appointment-6812523/ |
| equipo-lucia.webp | Profesional de espaldas y paciente de perfil | Gustavo Fring — https://www.pexels.com/photo/dentist-working-with-patient-5622000/ |
| comparador-antes.webp | Base del comparador, recorte de una sonrisa | Vitaly Gariev — https://www.pexels.com/photo/close-up-of-human-smile-displaying-natural-teeth-39842774/ |
| comparador-despues.webp | Retoque digital ilustrativo de esa misma foto | Derivada de Pexels 39842774 de Vitaly Gariev, color del esmalte aclarado con herramienta de edición de imagen; sin cambiar identidad ni atribuir un resultado real. |

El comparador es una **SIMULACIÓN digital** y se rotula como simulación en la
UI. Las dos variantes parten de la misma fotografía de Pexels; no se usan
dos bocas diferentes. No es un resultado clínico. Fuente y edición quedan
registradas en los sidecars de cada imagen; el footer enlaza a estos créditos.

Todas las fotos elegidas se descargaron; no hubo sustituciones por error de
descarga. Las candidatas no utilizadas quedan fuera del repo público.

## Copy y límites

Voseo claro y cotidiano. Marca, personas y datos son ficticios en la UI;
se conserva noindex/nofollow. No se inventa dirección callejera, cobertura
de una prepaga concreta, horario 24 h, garantías ni resultados clínicos.
La frecuencia de limpieza se define en evaluación, sin intervalo universal.
Urgencias en horarios de atención y según disponibilidad confirmada.
Medios de pago solo como información ficticia, sin integración ni cobros.

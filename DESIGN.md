---
name: Clínica Dental Serena — Paso a paso luminosa
description: Una consulta clara y un recorrido vertical que se entiende antes de decidir.
colors:
  bg: "#F7FAFA"
  ink: "#123B4F"
  blue: "#2A7AB0"
  mint: "#9AD1C8"
  paper: "#FFFFFF"
  soft: "#EAF4F3"
  whatsapp: "#25D366"
  muted: "#456372"
  line: "rgba(18,59,79,.18)"
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
    lineHeight: 1.25
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
  photo: "24px 6px 24px 6px"
  comparison: "24px"
  pill: "999px"
  circle: "50%"
spacing:
  inset-mobile: "24px"
  inset-desktop: "32px"
  section-desktop: "100px"
  section-mobile: "70px"
  anchor: "104px"
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
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "14px 23px"
  consultation-card:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.surface}"
    padding: "30px 34px"
  whatsapp-floating:
    backgroundColor: "{colors.whatsapp}"
    textColor: "{colors.paper}"
    rounded: "{rounded.circle}"
    width: "58px"
    height: "58px"
---

# Design System: Clínica Dental Serena

## Overview

**Creative North Star: "Paso a paso luminosa"**

La promesa de Serena se vuelve un camino visible: la primera consulta se resume al entrar y la línea azul conecta las cuatro etapas reales. La consulta por tratamiento resuelve la elección sin navegar filtros.

El sitio conserva Sora, Manrope y las ocho imágenes existentes. La densidad alterna filas breves, una fotografía clínica amplia y el recorrido vertical con el presupuesto dentro del momento en que se entrega el plan. El comparador sigue siendo una simulación explícita.

**Key Characteristics:**
- Tarjeta de consulta sobre el borde inferior del hero.
- Ocho tratamientos en acordeón, con consulta específica.
- Comparador único del conjunto, siempre rotulado.
- Línea de tiempo azul con cuatro hitos; presupuesto en el tercero.
- Preguntas y respuestas visibles como lista de control.

## Colors

### Primary
- **Azul sereno** ({colors.blue}): botones principales, línea y números del recorrido. No grandes fondos oscuros.

### Secondary
- **Menta clínica** ({colors.mint}): tildes de la lista de control y pequeños acentos. Las tildes se apoyan sobre un círculo tinta para contrastar.
- **Menta suave** ({colors.soft}): fondo del hero, recorrido y cierre.
- **Verde WhatsApp** ({colors.whatsapp}): solo el flotante requerido.

### Neutral
- **Luz** ({colors.bg}): fondo general y comparador.
- **Papel** ({colors.paper}): tratamientos, equipo, preguntas y tarjeta de consulta.
- **Tinta clínica** ({colors.ink}): textos y único fondo oscuro, el footer.
- **Tinta secundaria** ({colors.muted}): lectura de apoyo sobre superficies claras.
- **Divisor clínico** ({colors.line}): separadores de acordeón, presupuesto y checklist; tinta al 18 %.

**The Light Journey Rule.** Ninguna sección oscura antes del footer. El azul estructura; no ocupa toda una pantalla como fondo.

## Typography

Sora 400/500/600 y Manrope 400/500/600/700, desde el enlace Google Fonts existente. No cambia el wordmark.
- Display Sora 500: 66 px escritorio / 44 px móvil, 1.09, tracking -.025em.
- H2 Sora 500: 40 px / 32 px, 1.16. Títulos con balance natural.
- H3 Sora 500: 24 px / 21 px, 1.25.
- Lectura Manrope 16 px, 1.65, medida máxima 68ch.
- Ajustes de contexto: intro 18 px; nombres de tratamientos 22/19/18 px; hitos 24/21 px; tarjeta 27/25 px; equipo 21/19/17 px.
- Metadatos 11–14 px, importes 25/23 px y marca 25/40/38 px según ubicación.
- Metadatos Manrope 14 px, 1.5; precios con cifras tabulares.

## Layout

Contenedor máximo 1180 px con 32 px laterales (24 px en móvil). Secciones 100 px / 70 px; anclas 104 px. Corte principal 800 px, ajuste móvil 600 px y estrecho 400 px.

Orden cerrado: hero → tratamientos → comparador → recorrido → equipo → lista de control → cierre → footer. Los datos +10 años, 4,9/5 y turnos en la semana quedan dentro del hero, debajo de la tarjeta.

El hero divide texto y foto en escritorio. Su tarjeta blanca cruza el borde de la superficie menta; en móvil se apila sin ampliar el ancho de página. La foto no pierde su proporción. La línea de tiempo mantiene cuatro hitos verticales también en escritorio. El presupuesto completo se inserta en Recibís tu plan: no se transforma en un paso adicional ni en una sección de venta.

## Elevation & Depth

Superficies planas y separación por tono. Solo la tarjeta flotante y el acceso fijo tienen sombra estructural.
- Consulta: 0 16px 40px rgba(18,59,79,.10).
- WhatsApp: 0 8px 24px rgba(18,59,79,.22).

## Shapes

Tarjeta 16 px; foto con esquinas alternadas 24/6 px; comparador 24 px; botones cápsula; hitos y flotante circulares. Acordeones y filas de precio sin cajas ni redondeos añadidos.

## Components

### Buttons
Azul y blanco, 14×23 px, mínimo 48 px de alto; hover tinta y foco azul con separación. Secundarios transparentes con borde tinta. Íconos de WhatsApp de 20 px, blancos, sin stroke. Flotante 58 px, verde y símbolo blanco de 28 px.

Se conserva exactamente el href de hero (en la tarjeta), cierre y flotante. Cada tratamiento incorpora Consulta con el nombre exacto y el mensaje del brief. La lista de precios no contiene enlaces ni botones.

### Consulta
Título Tu primera consulta; tres líneas copiadas de los primeros tres hitos. CTA Pedir turno, único texto de CTA ajustado por instrucción expresa. En escritorio lista y acción en columnas; móvil lista apilada y acción completa.

### Tratamientos
Ocho details nativos con summary accesible; nombre y precio publicado cuando corresponde. Limpieza se identifica explícitamente en la vista previa de Limpieza y control, sin asignarle precio nuevo al control. Descripción, Para vos si y categoría originales; fotos existentes en los dos primeros interiores. Sin filtros. El contenido es accesible sin JS mediante details nativos.

### Comparador
Se preservan ambas imágenes, warning visible, teclado por pasos de cuatro, Home/End, arrastre y aria-valuenow. Sin atribución clínica real.

### Recorrido y presupuesto
Línea azul vertical, 01–04 por orden real. En el tercer hito se conservan el título Un presupuesto por escrito, introducción, evaluación sin cargo, Limpieza desde $45.000, Blanqueamiento desde $180.000 y nota. Sin botones en precios.

### Equipo y visita
Fila simple con las tres fotos, nombres y roles intactos. En móvil, retratos y nombres legibles sin desborde. Seis preguntas y respuestas siempre visibles; tilde menta sobre círculo tinta. Sin segundo acordeón.

### Movimiento y estados
GSAP 3.12.5/ScrollTrigger y Lenis 1.1.14 existentes; entrada coordinada del hero y revelado leve de hitos al scroll, desde contenido visible. Sin librerías nuevas. Movimiento reducido desactiva entrada y suavizado; fallback nativo con contenido completo. Foco, selección y scrollbars desde la paleta.

## Do's and Don'ts

### Do:
- **Do** conservar textos y datos ficticios exactamente.
- **Do** mostrar los importes publicados sin botones en su lista.
- **Do** mantener todas las superficies claras excepto el footer.
- **Do** usar el path de WhatsApp proporcionado una sola vez con viewBox 24.
- **Do** revisar teclado, movimiento reducido y anchos 430/390 px.

### Don't:
- **Don't** inventar precios, servicios, garantías o resultados clínicos.
- **Don't** recuperar filtros ni convertir las preguntas en otro acordeón.
- **Don't** presentar la simulación como un caso real.
- **Don't** agregar fotos ni librerías cuando el material existente cubre la página.

## Fotografías y procedencia

Fotos libres de Pexels, descargadas y optimizadas a WebP en assets/.
Licencia: https://www.pexels.com/license/ . No se presentan como instalaciones,
equipo ni resultados propios reales de Serena. Son material ilustrativo de
una marca ficticia. Se revisan marcas, letras ajenas y caras frontales.

| Archivo | Uso | Autor y fuente |
|---|---|---|
| hero-consultorio.webp | Hero luminoso, reencuadre hacia sillón azul | Tima Miroshnichenko — https://www.pexels.com/photo/a-clinic-with-dental-equipment-5355920/ |
| tratamiento-control.webp | Interior del acordeón Limpieza y control, atención de perfil | Cedric Fauntleroy — https://www.pexels.com/photo/a-dentist-checking-the-woman-s-teeth-4270362/ |
| tratamiento-estetica.webp | Interior del acordeón Blanqueamiento, sonrisa | Kindel Media — https://www.pexels.com/photo/close-up-photo-of-person-s-smile-7298633/ |
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


## Molde resultante

Paso a paso luminosa: hero con tarjeta de consulta, tratamientos en acordeón con consulta por tratamiento, comparador único, línea de tiempo vertical, equipo simple, lista de control visible y cierre claro. La tarjeta queda completa en el primer viewport comprobado de 430×932 px: foto móvil de 160 px, tarjeta de 22 px de inset y 14 px entre grupos. El recorrido conserva exactamente los cuatro pasos y la lista original sin botones. Ocho consultas específicas más los tres enlaces originales suman once enlaces de WhatsApp, todos con un único símbolo oficial.

Verificación local completada en 1440, 768, 430 y 390 px: sin overflow, ocho fotos decodificadas, textos y precios comparados con la fuente, acordeón y comparador con teclado, movimiento reducido, lectura sin JS y desplazamiento con rueda. No se descargaron ni sustituyeron fotografías.

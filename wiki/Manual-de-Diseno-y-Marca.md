# Manual de diseño y de marca
### Boda Cecilia & Juan Pablo · 5 de diciembre de 2026

---

## 1. Concepto

**Floral editorial, romántico y contemporáneo.** La invitación se siente como un pliego de papel fino: fondo marfil, tinta oscura, mucho aire alrededor del texto y flores realistas que enmarcan sin invadir. Delicada, pero con carácter.

Palabras clave: *luz, aire, jardín, papel, vals de las flores.*

Frase de marca: «Vamos a sellar nuestro amor bajo el vals de las flores, queremos que nos acompañes en este nuevo camino».

---

## 2. Paleta de color

| Rol | Nombre | Hex | Token CSS | Uso |
|---|---|---|---|---|
| Fondo | Marfil (papel) | `#f4f1e9` | `--paper` | Fondo general de la invitación |
| Fondo de tarjeta | Marfil claro | `#faf8f2` | `--paper-2` | Tarjeta de portada, superficies |
| Texto principal | Tinta | `#303635` | `--brand-ink` | Nombres, títulos, cuerpo |
| Texto secundario | Tinta suave | `#5d6664` | `--brand-ink-soft` | Subtítulos, etiquetas |
| Acento | Rosa intenso | `#d94b76` | `--brand-rose` | Frase de invitación, «&», botones, foco |
| Acento suave | Rosa claro | `#f2a0b7` | `--brand-rose-light` | Fecha, ornamentos, pétalos |
| Acento | Azul medio | `#3b80c9` | `--brand-blue` | Degradado de botones, detalles |
| Acento suave | Azul claro | `#8db9e9` | `--brand-blue-light` | Difuminados del fondo, florecitas |
| Detalle | Verde botánico | `#6f8f5e` | `--botanic` | Hojas y tallos (presentes en las ilustraciones) |
| Detalle | Dorado | `#c9a96a` | `--brand-gold` | Filetes, bordes finos, centros de flor |

**Proporción recomendada:** 70 % marfil · 20 % tinta · 10 % acentos (rosa > azul > dorado).

**Reglas**
- El rosa claro tiene poco contraste sobre marfil: úsalo solo en textos grandes (≥ 28 px), como la fecha en Parisienne, y nunca para texto corrido.
- El rosa intenso es el único color de acento para textos de tamaño medio.
- Nunca pongas rosa sobre azul (ni al revés) como texto sobre fondo.

---

## 3. Tipografía

| Familia | Rol | Pesos | Ejemplo |
|---|---|---|---|
| **Cormorant Garamond** (serif) | Nombres, títulos, cifras de la cuenta regresiva | 400–600, itálica | *Cecilia & Juan Pablo* |
| **Montserrat** (sans serif) | Cuerpo, subtítulos, etiquetas tipo *eyebrow* en mayúsculas | 300 / 400 / 500 | NUESTRA BODA |
| **Parisienne** (script) | Acentos románticos: fecha, notas cortas | 400 | Sábado, 5 de diciembre de 2026 |

**Jerarquía de la portada**
1. *Eyebrow* — Montserrat 400, mayúsculas, espaciado 0,42 em, tinta suave («NUESTRA BODA»).
2. **Nombres** — Cormorant Garamond itálica 500, de 2,6 rem a 9 rem según el ancho; el «&» va en rosa intenso al 46 % del tamaño.
3. **Fecha** — Parisienne, 1,9–3 rem, rosa claro.
4. **Frase** — Cormorant Garamond itálica, 1,05–1,4 rem, rosa intenso, máximo 30 caracteres por línea.

**Reglas**
- Parisienne nunca en mayúsculas ni en bloques de más de una línea.
- No mezclar más de dos familias en un mismo bloque.

---

## 4. Diagramación

- **Portada a pliego completo:** ocupa el 100 % del alto visible, con un margen exterior proporcional (14–40 px).
- **Tarjeta:** ancho máximo de 1240 px, fondo marfil claro, borde dorado fino y un filete interior doble que evoca papel impreso.
- **Márgenes internos:** generosos (72–120 px arriba y abajo); a los lados, el espacio lo marcan las flores laterales más una holgura fija, de modo que el texto nunca toque las ilustraciones.
- **Eje:** composición centrada y simétrica; los filetes finos sobre y bajo la fecha y la frase separan los bloques.
- **Móvil:** las flores laterales se colocan en diagonal (arriba a la izquierda y abajo a la derecha) para liberar el ancho central.

---

## 5. Elementos florales

- **Estilo:** ilustración botánica realista; tulipanes y guisantes de olor en rosa, campanillas en azul, florecitas blancas y follaje verde.
- **Marco perimetral:** dos ramas laterales en forma de corchete enmarcan la portada; cuatro ramilletes de amapolas rosas completan los bordes superior e inferior.
- **Equilibrio:** las flores guían la vista hacia los nombres; no deben pisar el texto ni llenar el centro.
- **Ornamento vectorial:** la flor de cinco pétalos (símbolo `#fl`) se usa en separadores, en el carrusel y en el bokeh del fondo.

---

## 6. Movimiento

| Elemento | Comportamiento | Duración |
|---|---|---|
| Fondo marfil | Difuminado radial rosa/azul muy tenue que se desplaza como aire o luz | 38 s, ida y vuelta |
| Bokeh floral | Contornos de florecitas que aparecen, giran levemente y se desvanecen (opacidad ≤ 20 %) | 12–22 s cada una |
| Pétalos y destellos | Caen y titilan en una capa ligera | Continuo |
| Flores de portada | Se mecen suavemente desde el tallo | 7–8 s |
| Carrusel | Cada foto se ve 3 s, con un fundido de 0,6 s y un zoom lento | 3 s / 0,6 s |
| Frase de invitación | Efecto máquina de escribir al abrir la invitación | ~3 s |

**Reglas**
- El movimiento debe ser casi imperceptible; nada parpadea ni cambia de golpe.
- Con *movimiento reducido* activado en el sistema, el bokeh y los difuminados se detienen y las fotos cambian sin zoom.

---

## 7. Componentes

- **Botón principal:** píldora con degradado rosa intenso → azul medio, texto blanco Montserrat 500; al pasar el cursor se eleva y brilla.
- **Botón secundario (ghost):** fondo translúcido con borde de tinta al 28 %.
- **Separador:** dos filetes que se desvanecen con la flor `#fl` en rosa claro al centro.
- **Marco de fotos:** arco de medio punto (radio superior 170 px) con un filete rosa exterior.

---

## 8. Usos incorrectos

- ✗ Cambiar el fondo marfil por blanco puro o por degradados saturados.
- ✗ Usar el rosa claro en párrafos o textos pequeños.
- ✗ Agrandar las flores hasta cubrir los nombres o la fecha.
- ✗ Animaciones rápidas (menos de 6 s en el fondo) o parpadeos.
- ✗ Sustituir las tipografías por otras de sistema o decorativas.

---

## 9. Datos del evento (referencia)

- **Novios:** Cecilia & Juan Pablo
- **Fecha:** sábado, 5 de diciembre de 2026 · 3:00 p.m. (hora de Colombia)
- **Lugar:** Finca La Leyenda, Guarne, Antioquia
- **Vestimenta:** traje formal
- **Música:** «Algo que se quede» — Grupo Niche

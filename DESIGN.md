# DESIGN.md — cesarfoodlab

> Guía de branding derivada de capturas del perfil de Instagram (@cesarfoodlab) el 04/10/2026.
> **Nota de fiabilidad:** Instagram bloquea el acceso automatizado, así que todo se ha extraído de 3 capturas (cabecera del perfil, pestaña Reels y rejilla de Reels). Los hex son **estimaciones visuales**, las tipografías son **equivalencias aproximadas** y las secciones de "frases" se basan solo en los textos visibles en portadas y bio (no he podido leer captions). Valida con tus archivos originales (Canva/CapCut) antes de fijar nada.

---

## 1. Esencia de marca

- **Nombre:** cesarfoodlab
- **Posicionamiento:** Dietista-nutricionista y food designer. Cocina de técnica y estética de restaurante, explicada con ciencia y accesible para casa.
- **Promesa (bio):** "Elevando tu cocina con ciencia y técnica".
- **Arquetipo:** El científico-cocinero cercano. Rigor técnico + humor y curiosidad.
- **Dualidad clave:** dos mundos en un mismo perfil:
  1. **Alta cocina / técnica** (tuiles, espumas, esferificaciones, emplatados con anotaciones).
  2. **Nutrición práctica / supermercado** (tops de Lidl, Aldi, Mercadona, perder grasa).

---

## 2. Paleta de color

### Neutros (base de todo el feed)
| Token | Hex | Uso |
|---|---|---|
| `--black` | `#111111` | Fondos de portada, texto con contorno, contraste fuerte |
| `--white` | `#FFFFFF` | Texto principal sobre foto, títulos |
| `--granite` | `#8E959A` | Encimera de granito (fondo recurrente en foto) |
| `--plate` | `#F2F1EE` | Platos blancos, fondos limpios |

### Acentos de marca (los que más se repiten)
| Token | Hex | Uso |
|---|---|---|
| `--highlight-yellow` | `#F7D842` | **Color firma.** Palabra clave del título ("MELOSO", "CONGELADOS", "TOP", "PRODUCTOS", "BROWNIE") |
| `--alert-red` | `#E0302B` | Énfasis y llamadas de atención ("5", "COME", "Lo que SÍ compro") |
| `--fresh-green` | `#3DDC3C` | Cadena/retail ("MERCADONA"), mensajes de "sí" |
| `--lab-teal` | `#3C95B0` | Fondos de portada tipo infografía (Top congelados) |

### Acentos de producto/recetas
| Token | Hex | Uso |
|---|---|---|
| `--terracotta` | `#C8622E` | Plato de barro en emplatados de pescado |
| `--orange-warm` | `#D9702A` | Título "Lentejas" (cocina casera, reconfortante) |
| `--brown-earth` | `#7A3E14` | Título "abuela" (tono nostálgico) |
| `--sage` | `#8A9A94` | Fondo de portadas editoriales ("Productos favoritos") |
| `--cream` | `#E0DDB0` | Formas de apoyo sobre salvia |

### Highlights de perfil
| Highlight | Color estimado |
|---|---|
| Bio-Data | `#1B1B4B` (azul noche, estilo biotech) |
| Publi | `#5B6B3A` (verde oliva) con interior `#F3EBDD` |
| Recetas & Platos / BCC / TikTok | Marrón oscuro, blanco, negro |

### Reglas de uso
- **Regla 60/30/10:** 60 % foto real de comida (color natural) · 30 % blanco/negro en tipografía · 10 % amarillo `#F7D842` como único acento.
- **Un solo color de acento por portada.** El amarillo es el predeterminado; rojo o verde solo si el tema lo exige (ofertas, retail, alerta).
- Evita degradados, neones y fondos saturados que compitan con la comida.

```css
:root {
  --black: #111111;
  --white: #FFFFFF;
  --granite: #8E959A;
  --plate: #F2F1EE;
  --highlight-yellow: #F7D842;
  --alert-red: #E0302B;
  --fresh-green: #3DDC3C;
  --lab-teal: #3C95B0;
  --terracotta: #C8622E;
  --orange-warm: #D9702A;
  --brown-earth: #7A3E14;
  --sage: #8A9A94;
  --cream: #E0DDB0;
  --navy-biodata: #1B1B4B;
  --olive-publi: #5B6B3A;
}
```

---

## 3. Tipografías

> Equivalencias en Google Fonts por parecido visual. Si usas otras en Canva/CapCut, sustitúyelas aquí.

| Rol | Estilo observado | Equivalente sugerido |
|---|---|---|
| **Título de portada (impacto)** | Sans condensada, ultra bold, MAYÚSCULAS, interlineado muy cerrado | `Anton` / `Bebas Neue` / `League Gothic` |
| **Título secundario / etiquetas** | Sans bold blocky en mayúsculas, a veces con caja amarilla detrás | `Archivo Black` / `Montserrat ExtraBold` |
| **Títulos "amables"** | Sans redondeada bold, mezcla de mayúsculas/minúsculas ("EL MEJOR BROWNIE") | `Fredoka` / `Baloo 2` |
| **Subtítulos de vídeo (captions)** | Serif de contraste, peso medio, con sombra suave | `Fraunces` / `DM Serif Display` |
| **Anotaciones en emplatados** | Mayúsculas pequeñas, bold, con flechas finas blancas | `Montserrat Bold` (tracking +5 %) |
| **Texto de interfaz / documentos** | Sans limpia neutra | `Inter` |

### Reglas
- Máximo **2 tipografías por pieza** (impacto + una de apoyo).
- Palabra clave en **amarillo**, resto en **blanco**. Contorno o sombra negra si el fondo es claro.
- Títulos cortos: **2–4 palabras** en 2–3 líneas apiladas, tamaño decreciente o contrastado (una línea grande, otra más pequeña).
- Mezclar tamaños y colores dentro de un mismo título es parte de la identidad ("Lentejas **de la** abuela").

---

## 4. Estilo visual

### Fotografía y vídeo
- **Plano cenital o 3/4** sobre encimera de **granito gris** (elemento reconocible).
- Luz natural/cocina doméstica, sin fondos de estudio artificiales. Autenticidad de "laboratorio casero".
- Comida protagonista: texturas (arroz meloso, tuiles, salsas) en primer plano.
- Mezcla de formatos: **vídeo de proceso** (cucharas, espumas, técnicas), **emplatado artístico** y **supermercado/vlog**.

### Portadas (Reels)
- Formato vertical 9:16, texto grande ocupando el tercio superior o central.
- Tres plantillas detectadas:
  1. **Foto + título gigante** (Arroz meloso, Lentejas de la abuela).
  2. **Fondo plano de color + logo/marca** (Top congelados Lidl, Productos favoritos).
  3. **Foto real del sitio + título en caja amarilla** (6 productos top de Aldi, 5 productos perder grasa).
- Series con nombre propio: **"Técnicas Michelin"**, **"Eso se come"** (con icono propio: llave roja Michelin / texto bicolor).
- Uso de **logos de supermercados** (Lidl, Aldi, Mercadona) como gancho de reconocimiento inmediato.

### Posts de rejilla (emplatados)
- Marca de agua pequeña arriba: **@CESARFOODLAB** (mayúsculas, blanca, esquina superior izquierda).
- **Anotaciones con flechas finas** blancas señalando cada componente ("Reducción de vino tinto", "Carrillera ibérica", "Puro colágeno", "Ajo confitado", "Falsa..."). Estilo infográfico técnico.
- Carruseles con foto del plato + detalle de técnica.

### Elementos gráficos
- Flechas finas blancas · cajas de color plano tras el texto · iconos de emoji (🧑‍🍳 🤟 🍣 🧬 🥑 🎓 🔪) · logotipos de terceros.
- Sin marcos, sin filtros pesados, sin stickers genéricos.

### Avatar y presencia
- Foto con **chaquetilla blanca de cocinero**, sonriente, exterior con vegetación verde. Transmite: profesionalidad + cercanía.
- Highlights con iconos circulares de fondo oscuro o plano (coherentes entre sí).

---

## 5. Tono de voz

**En una frase:** *Un científico de cocina que habla como un colega: directo, curioso y sin postureo.*

### Atributos
| Atributo | Cómo suena |
|---|---|
| **Cercano** | Tuteo, lenguaje cotidiano, referencias a "la abuela", "en casa" |
| **Técnico pero accesible** | Palabras como *técnica, ciencia, colágeno, reducción*, siempre explicadas |
| **Directo / gancho** | Números y promesas claras: "6 productos top", "5 productos para perder grasa" |
| **Curioso y provocador** | Preguntas y retos: "¿Vodka hecho en laboratorio?", "Si quieres dominar…" |
| **Honesto con el consumidor** | "Lo que SÍ compro", "Productos favoritos" (opinión personal, no anuncio) |
| **Orgulloso sin arrogancia** | "El mejor brownie que he hecho este año" (primera persona, humilde) |

### Estructura típica de un título/gancho
1. **Número + categoría + marca** → "6 productos top de Aldi"
2. **Adjetivo de sabor/textura + plato** → "Arroz meloso"
3. **Nostalgia + plato** → "Lentejas de la abuela"
4. **Técnica + autoridad** → "Técnicas Michelin: huevo poché"
5. **Pregunta intrigante** → "¿Vodka hecho en laboratorio?"
6. **Contraste verdad/apariencia** → "Parece X, pero en realidad está…"

---

## 6. Frases que SÍ uso (extraídas de tu perfil)

**Bio y posicionamiento**
- "Nutricionista y Food Designer"
- "Dietista-Nutricionista"
- "Elevando tu cocina con ciencia y técnica"

**Títulos de contenido**
- "Arroz meloso"
- "Top congelados de Lidl"
- "Lentejas de la abuela"
- "Si quieres dominar…"
- "Productos favoritos"
- "Técnicas Michelin"
- "Eso se come"
- "6 productos top de Aldi"
- "Lo que sí compro (Mercadona)"
- "¿Vodka hecho en laboratorio?"
- "5 productos para perder grasa"
- "El mejor brownie que he hecho este año"
- "Niguiri de salmón con sweet chile mango (receta fácil para hacer en casa)"
- "Unta igual, pero en realidad está…"

**Patrones recurrentes (reutilizables)**
- "[Número] productos top de [supermercado]"
- "Lo que sí compro en [tienda]"
- "El mejor [plato] que he hecho este año"
- "Receta fácil para hacer en casa"
- "[Plato] de la abuela"
- "Técnicas Michelin: [técnica]"
- "Parece [A], pero en realidad es [B]"

---

## 7. Frases que NUNCA uso (recomendadas, inferidas del posicionamiento)

> No puedo verificar esto desde las capturas: es una propuesta coherente con tu marca. Ajústala a tu criterio.

**Evita (contradicen "ciencia y técnica")**
- "Dieta milagro", "quema grasa rápido", "detox", "adelgaza X kilos en Y días"
- "Alimento prohibido", "comida basura", "alimentos buenos y malos" (lenguaje moralista)
- "Truco secreto de chef que no quieren que sepas"
- "Bajar de peso sin esfuerzo"

**Evita (contradicen "cercano y honesto")**
- "Como experto te digo que…" (tono de autoridad impuesta)
- "Hola chicos, bienvenidos a mi canal" (fórmula genérica de youtuber)
- "Link en bio, no te lo pierdas" sin aportar valor
- "Publicidad encubierta" o recomendaciones sin aclarar colaboración (usa el highlight **Publi** y etiqueta siempre)
- Lenguaje jerárquico o elitista: "cocina para paladares exigentes"

**Evita (contradicen "accesible")**
- Jerga técnica sin explicar (ej. "transglutaminasa" sin contexto)
- Anglicismos innecesarios de moda ("hack", "foodie vibes")
- Exceso de hashtags y emojis de relleno

---

## 8. Pilares de contenido

| Pilar | Formato | Ejemplos |
|---|---|---|
| **Técnica de alta cocina en casa** | Reels de proceso, carruseles anotados | Tuile, espuma, huevo poché, esferificación |
| **Supermercado inteligente** | Vlog + lista numerada | Lidl, Aldi, Mercadona |
| **Nutrición y salud** | Reels informativos | Perder grasa, vodka de laboratorio, NoLo |
| **Cocina reconfortante** | Receta + foto cenital | Lentejas, arroz meloso |
| **Emplatado y food design** | Carrusel con flechas y etiquetas | Carrillera, bacalao Skrei |
| **Detrás de BCC** | Stories/highlight | Basque Culinary Center, clases, catas |

---

## 9. Reglas rápidas (Do / Don't)

### Do
- Título en 2–4 palabras, mayúsculas, con **una palabra en amarillo `#F7D842`**.
- Fondo con comida real o color plano de la paleta.
- Anotar los platos con flechas finas blancas.
- Dar números concretos y ser honesto sobre opiniones y colaboraciones.
- Mantener la encimera de granito y la luz natural como sello visual.
- Mostrar el proceso, no solo el resultado.

### Don't
- No mezclar más de un color de acento fuerte por portada.
- No usar tipografías decorativas, manuscritas o de moda.
- No filtros saturados que alteren el color de la comida.
- No prometer resultados de salud sin base.
- No esconder publicidad.

---

## 10. Prompt base para IA (copiar y pegar)

```
Actúa como el community manager de @cesarfoodlab, un dietista-nutricionista y food
designer estudiante de Basque Culinary Center. Tono: cercano, técnico pero accesible,
curioso, honesto, tuteo, español de España, sin postureo ni promesas milagro.
Estructura de ganchos: número + categoría + marca, o plato + adjetivo de textura,
o "técnica Michelin + técnica". Evita dietas milagro, lenguaje moralista sobre
comida y jerga sin explicar. Cuando hables de marcas, aclara si es opinión personal
o colaboración. Estilo visual: portada con foto real de comida sobre encimera de
granito, título en tipografía condensada bold en blanco con la palabra clave en
amarillo #F7D842, acentos puntuales en rojo #E0302B.
```

---

## 11. Pendiente de validar contigo

- [ ] Tipografías reales que usas (Canva/CapCut) para sustituir las equivalencias.
- [ ] Hex exactos del amarillo y del logo si tienes archivo original.
- [ ] Captions reales para refinar "frases que uso".
- [ ] Lista real de palabras/expresiones que quieres vetar.
- [ ] Si el icono de la llave roja (Técnicas Michelin) es parte de tu identidad o un recurso puntual.

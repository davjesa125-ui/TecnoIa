# Tecno · Humano digital de agricultura

Humano digital que habla desde Argentina (1980 a la actualidad), en primera persona y con voseo, para estudiantes de secundario. Explica la **agricultura convencional-tradicional** y responde preguntas por voz o por escrito.

Cada dato de su base de conocimiento está marcado como **documentado**, **atribuido**, **controvertido** o **didáctico**, y Tecno dice de dónde sale.

## Qué hay en esta carpeta

| Archivo | Para qué sirve |
|---|---|
| `index.html` | Página lista para publicar: pantalla completa con la imagen de Tecno y un único botón «Hablar con Tecno» (el widget de ElevenLabs). |
| `assets/tecno.jpg` | Imagen de referencia de Tecno (fondo de la portada). |
| `assets/tecno-retrato.jpg` | Recorte del retrato (ya no se usa en la página; se puede borrar o usar como avatar). |
| `knowledge/base_conocimiento_tecno.md` | Base de conocimiento con etiquetas y fuentes. Es el mismo texto cargado en ElevenLabs. |

## El agente en ElevenLabs

- **Nombre:** Tecno — Humano digital de agricultura
- **ID del agente:** `agent_3701m5dh96y3fmv8z7hp105g8ab3`
- **Idioma:** español
- **Modelo:** `claude-haiku-5-5`, temperatura 0,3
- **Base de conocimiento:** documento «Tecno - Base de conocimiento: agricultura convencional-tradicional Argentina 1980-2026», con RAG activado
- **Widget:** configurado en español rioplatense (verde y trigo)

### Pendiente: la voz argentina

Las voces argentinas de la biblioteca de ElevenLabs no se pudieron asignar de forma automática: el servicio devolvió `voice_not_found` porque primero hay que agregarlas a tu cuenta. Por ahora el agente habla con la voz por defecto (que entiende y habla español, pero sin acento rioplatense).

Para ponerle voz argentina:

1. Entrá a ElevenLabs → **Voices** y buscá una voz con acento argentino (por ejemplo «Diego», «Pablo, Argentino, Córdoba» o «Octavio»). Escuchá las muestras y elegí la que más te guste.
2. Apretá **Add to My Voices** (agregar a mis voces).
3. Abrí el agente Tecno → pestaña **Voice** → elegí esa voz y guardá.

También podés pedirme que la asigne por ID una vez que la hayas agregado.

## Probar el agente antes de publicar

1. En ElevenLabs abrí el agente y usá **Test AI agent**.
2. Hacele estas preguntas y fijate cómo responde:
   - «¿Qué es la siembra directa?» (debe nombrar a Aapresid o al INTA).
   - «¿El glifosato es cancerígeno?» (debe explicar el desacuerdo, sin un sí o no).
   - «¿Cuántas hectáreas de soja hubo en 1995?» (debe decir que no tiene el dato).
   - «¿A cuántos metros de una escuela se puede fumigar?» (no debe dar una distancia como obligatoria).
3. Confirmá que el agente permita conversaciones públicas (en **Security**, la autenticación debe estar desactivada), porque la página es pública.

## Publicar en GitHub Pages

1. Creá un repositorio nuevo en GitHub (por ejemplo `tecno-humano-digital`). Puede ser público.
2. Subí **todo el contenido de esta carpeta** (`index.html`, `assets/`, `knowledge/`, `README.md`), de modo que `index.html` quede en la raíz del repositorio.
3. En el repositorio: **Settings → Pages**. En *Build and deployment*, elegí **Deploy from a branch**, rama `main` y carpeta `/ (root)`. Guardá.
4. Esperá uno o dos minutos. La página va a quedar en:
   `https://TU-USUARIO.github.io/tecno-humano-digital/`
5. Abrila en el navegador, apretá el botón del agente (abajo a la derecha) y aceptá el permiso del micrófono.

### Si el botón del agente no aparece

- El widget se carga desde `unpkg.com`; si la red de la escuela bloquea ese sitio, no se va a ver.
- Verificá que el ID del agente en `index.html` (`agent-id="..."`) sea el correcto.
- Si usás un dominio propio, en ElevenLabs podés restringir qué dominios pueden usar el agente (lista de permitidos): agregá `TU-USUARIO.github.io`.

## Cómo actualizar la base de conocimiento

1. Editá `knowledge/base_conocimiento_tecno.md` (mantené las etiquetas `[DOCUMENTADO]`, `[ATRIBUIDO]`, `[CONTROVERTIDO]`, `[DIDÁCTICO]`).
2. En ElevenLabs, abrí el documento de la base de conocimiento del agente y reemplazá el texto, o creá un documento nuevo y vinculalo al agente.
3. Si agregás datos a la página, mantené la misma etiqueta y la fuente al lado.

## Criterios de la base de conocimiento

- Los datos numéricos salen de las fuentes citadas, con el año que ellas indican.
- Lo que sostiene un actor (industria, productor, investigador) se presenta como **atribuido**, nunca como verdad general.
- Temas con posiciones enfrentadas (por ejemplo, glifosato y salud) se presentan como **controvertidos**, con las dos miradas.
- Un punto a verificar antes de citarlo en un trabajo: la fecha de vencimiento de la patente del glifosato (1992) figura en una sola fuente universitaria y está marcado como atribuido.
- Un proyecto de ley (distancias de 10 y 45 metros) **no es** una ley vigente; Tecno no lo presenta como norma.

## Aviso

Tecno es un personaje creado con inteligencia artificial con fines educativos. No es una persona real, no representa al INTA ni a ninguna institución y puede equivocarse. La imagen de referencia es la que aportó el autor del proyecto.

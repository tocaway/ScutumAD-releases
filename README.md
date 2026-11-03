# Instalar y actualizar ScutumAD

**Versión actual:** ScutumAD 3.0.5

ScutumAD bloquea anuncios, rastreadores y webs peligrosas en Google Chrome (y en Edge o Brave), en Mac y en Windows. El instalador deja ScutumAD en una carpeta de tu usuario y añade un pequeño actualizador: así recibes las versiones nuevas con un botón, sin volver a instalar nada.

## 1. Instalar

### Mac

1. Descarga [ScutumAD-Mac.zip](https://github.com/tocaway/ScutumAD-releases/raw/main/instalar/ScutumAD-Mac.zip) y ábrelo con doble clic: aparece **Instalar ScutumAD.command**.
2. Haz clic derecho sobre **Instalar ScutumAD.command** → **Abrir** → **Abrir**.
   Si el Mac dice que no puede comprobar el archivo, ve a **Ajustes del Sistema → Privacidad y seguridad**, baja hasta el aviso de «Instalar ScutumAD» y pulsa **Abrir igualmente**.
3. Se abre una ventana negra. Si te lo pide, cierra Chrome del todo (**Cmd+Q**) y pulsa **Intro**.
4. Cuando ponga **Listo**, sigue con el apartado «En Chrome». La carpeta es `ScutumAD/extension`, dentro de tu carpeta de usuario.

### Windows

1. Descarga [ScutumAD-Windows.zip](https://github.com/tocaway/ScutumAD-releases/raw/main/instalar/ScutumAD-Windows.zip), haz clic derecho → **Extraer todo** → **Extraer**.
2. Abre **Instalar ScutumAD.bat** con doble clic.
   Si Windows muestra «Windows protegió su PC», pulsa **Más información** → **Ejecutar de todas formas**.
3. Se abre una ventana negra. Si te lo pide, cierra Chrome del todo y pulsa una tecla.
4. Cuando ponga **Listo**, sigue con el apartado «En Chrome». La carpeta es `C:\Users\<tu usuario>\ScutumAD\extension`.

### En Chrome (solo la primera vez)

1. Abre Chrome y escribe en la barra de direcciones `chrome://extensions`.
2. Activa **Modo de desarrollador** (arriba a la derecha).
3. Pulsa **Cargar descomprimida** y elige la carpeta `ScutumAD/extension` que indicó el instalador.
4. Recomendado: pulsa **Detalles** en la tarjeta de ScutumAD y activa **Permitir scripts de usuario**. Así los scriptlets también usan las listas que se actualizan solas.
5. Fija el icono de ScutumAD en la barra.

No borres ni muevas la carpeta `ScutumAD`: Chrome carga la extensión desde ahí.

## 2. Actualizar ScutumAD

Cuando hay una versión nueva, ScutumAD te avisa y aparece **Actualizar** en su menú. Púlsalo: el actualizador descarga la versión, comprueba que es auténtica (va firmada) e instala; ScutumAD se reinicia solo.

En Configuración → **Actualizaciones de ScutumAD** puedes:

- buscar versiones nuevas;
- activar que se instalen solas;
- **volver a la versión anterior** si la nueva te da problemas.

Si pulsas Actualizar y no pasa nada, cierra Chrome del todo, vuelve a abrirlo y repite.

## 3. Las listas se actualizan solas

ScutumAD descarga las listas de filtros cada 6 horas y las aplica sin reiniciar. En Configuración → **Listas de filtros** puedes:

- ver cuándo se actualizaron y la versión de cada lista;
- pulsar **Actualizar ahora**;
- desactivar la actualización automática;
- volver a las listas incluidas en la versión, si una web falla tras una actualización.

Las descargas son anónimas: sin cookies, sin referer y sin datos tuyos (ver `PRIVACIDAD.md`).

## 4. Uso diario

- **Modo del sitio** (popup): Desactivado, Básico, Óptimo o Estricto. Si una web falla, prueba **Básico**; si una web de streaming abre pop-ups, usa **Estricto**.
- **Ver lo bloqueado en esta pestaña** (popup): abre el registro en directo. Recarga la pestaña para verlo desde el principio.
- **Modo aprendizaje**: activa el interruptor y pulsa **Seleccionar** en la pastilla de la página. Con **Ampliar** y **Reducir** ajustas el bloque, ves el filtro antes de guardarlo, y **Quitar solo ahora** lo oculta sin guardar nada.

## 5. Si algo no funciona

- **Una web se rompe:** pon el sitio en **Básico** o **Desactivado** desde el popup y recarga.
- **Un anuncio sigue apareciendo:** pulsa **Actualizar ahora** en Configuración, o elimínalo con el modo aprendizaje.
- **Los scriptlets no se actualizan:** activa **Permitir scripts de usuario** (paso 4 de la instalación).
- **YouTube:** ScutumAD nunca bloquea en la red lo que inicia YouTube ni modifica sus respuestas, para evitar su bloqueo anti-adblock. Oculta los anuncios del feed y salta los del reproductor; no se puede garantizar el 100 % frente a cambios futuros de YouTube.

Chrome mostrará el aviso de extensiones en modo desarrollador: es normal en una extensión instalada de forma local.

# Cartridge — Guía para testers

*[Read this in English](README.en.md)*

¡Gracias por darle una mano a este proyecto! Cartridge es un launcher nativo
de macOS para fangames de Pokémon hechos en RPG Maker XP / Essentials. La
idea es simple: apretás JUGAR y el juego arranca, sin instalar Wine, sin
configurar nada a mano.

Es un proyecto **experimental y en desarrollo activo**, así que tu prueba
vale oro para encontrar cosas que todavía no cubrimos.

## Descargar

👉 **[Bajá la última versión acá](https://github.com/United2204/cartridge-releases/releases/latest)**
(el archivo `Cartridge.zip`). Con eso alcanza — una vez instalada, la app se
actualiza sola (ver más abajo).

## Requisitos

- macOS (Apple Silicon o Intel — la app es universal, corre nativo en las dos).
- Tus juegos ya descomprimidos en una carpeta (o los `.zip`/`.rar` originales
  para descomprimir vos mismo con el Finder / Archive Utility).
  **Importante: esa carpeta NO puede estar dentro de Descargas** — movela a
  Documentos, Escritorio, o cualquier otra ubicación antes de elegirla en
  Cartridge.

## Instalación

macOS va a bloquear la app la primera vez porque todavía no tiene firma de
Apple (eso es un trámite aparte, no afecta cómo funciona). Para abrirla:

1. Descomprimí el `.zip` que bajaste y mové `Cartridge.app` a tu carpeta de
   Aplicaciones (o donde prefieras).
2. **Probá primero:** click derecho sobre `Cartridge.app` → **Abrir**. Si
   aparece un aviso de "desarrollador no identificado", tocá **Abrir** igual.
3. **En macOS moderno (Sequoia / Tahoe) el click derecho ya no alcanza** —
   la primera vez te va a decir que no se puede abrir. Es normal. Hacé esto:
   - Abrí **Ajustes del Sistema → Privacidad y seguridad**.
   - Bajá hasta el final: vas a ver un mensaje tipo *"Se bloqueó el uso de
     Cartridge.app…"* con un botón **"Abrir igual"**. Tocalo.
   - Confirmá con tu contraseña/Touch ID y elegí **Abrir**.
4. **Si dice que "está dañada"** y no te deja de ninguna forma, abrí la
   Terminal y corré esto una sola vez (cambiá la ruta si moviste la app):
   ```
   xattr -cr /Applications/Cartridge.app
   ```
   y volvé a intentar.
5. Después de esa primera vez, abre normal con doble click.

## Actualizaciones automáticas

Desde la **beta 4**, Cartridge **se actualiza sola**. Cuando publicamos una
versión nueva, la app te la ofrece al abrirla y se instala con un click —
no tenés que volver a bajar nada a mano ni repetir los pasos de arriba.

Si querés forzar la búsqueda en cualquier momento, andá al menú **Cartridge
→ "Buscar actualizaciones…"** (arriba a la izquierda, en la barra de menú).

> Si estabas en una beta vieja (1, 2 o 3) que ya no aparece en la lista,
> esas no tenían auto-update: bajá la última desde el link de arriba y de
> ahí en más se actualiza sola.

## Cómo usar

1. Al abrir por primera vez, te va a pedir que elijas la carpeta donde
   tenés (o vas a tener) tus juegos descomprimidos. La recuerda para la
   próxima.
2. Los juegos que detecte van a aparecer en una grilla con su carátula.
   Algunos necesitan una conversión de compatibilidad la primera vez (vas a
   ver una barrita "APLICANDO PARCHE…") — es automático, no hay que hacer
   nada.
3. Apretás JUGAR y listo.

## Qué probar

Lo más útil para nosotros es que juegues como jugarías normalmente:
avanzar la historia, entrar a batallas (salvajes y de entrenador), guardar
y cargar partida, cambiar de mapa/ruta, y si el juego tiene, evolucionar,
usar objetos, menús, etc. Cuanto más "al fondo" llegues, mejor — la mayoría
de los problemas que encontramos hasta ahora aparecen recién en situaciones
puntuales (una ruta específica, una animación específica), no al arrancar.

## Limitaciones conocidas (por ahora)

- **Funciones online que usan conexión directa tipo LAN** (por ejemplo,
  algunas variantes de Cable Club por red local) todavía no están
  soportadas. Funciones online que usan HTTP/HTTPS normal (buscar
  actualizaciones, trades tipo GTS, etc.) sí deberían andar.
- Es posible que algún juego puntual con scripts muy particulares no
  arranque o falle en un punto específico — si te pasa, es justo el tipo de
  cosa que queremos que nos reportes.

## Cómo reportar un problema

Si algo falla, mandanos:

1. **Qué juego** (nombre y versión si la sabés).
2. **Qué estabas haciendo** justo antes (ej. "entré a una batalla salvaje
   en la Ruta 3", "cargué una partida guardada").
3. **Captura de pantalla** del error si apareció alguno.
4. Si podés reproducirlo más de una vez, contanos los pasos — eso es lo que
   más ayuda.

No hace falta que sea un reporte formal, con un mensaje contándonos lo que
viste alcanza.

También tenemos un Discord para reportar bugs, charlar y enterarte de
novedades: **<https://discord.gg/XjurW8XXPf>**

## Apoyar el proyecto

Cartridge es un proyecto personal, hecho en tiempo libre. Si te gusta y
querés bancar el desarrollo, podés invitarme un cafecito acá:
**<https://ko-fi.com/united2204>** — totalmente opcional, no afecta nada de la
app ni de esta beta.

¡Gracias de nuevo por probarlo!

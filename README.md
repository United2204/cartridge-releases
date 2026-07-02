# Cartridge — Guía para testers

¡Gracias por darle una mano a este proyecto! Cartridge es un launcher nativo
de macOS para fangames de Pokémon hechos en RPG Maker XP / Essentials. La
idea es simple: apretás JUGAR y el juego arranca, sin instalar Wine, sin
configurar nada a mano.

Es un proyecto **experimental y en desarrollo activo**, así que tu prueba
vale oro para encontrar cosas que todavía no cubrimos.

## Requisitos

- macOS (Apple Silicon o Intel — la app es universal, corre nativo en las dos).
- Tus juegos ya descomprimidos en una carpeta (o los `.zip`/`.rar` originales
  para descomprimir vos mismo con el Finder / Archive Utility).

## Instalación

macOS va a bloquear la app la primera vez porque todavía no tiene firma de
Apple (eso es un trámite aparte, no afecta cómo funciona). Para abrirla:

1. Descomprimí el `.zip` que te pasamos y movés `Cartridge.app` a tu carpeta
   de Aplicaciones (o donde prefieras).
2. **Click derecho sobre `Cartridge.app` → Abrir.** Te va a aparecer un
   aviso de "desarrollador no identificado" — tocá **Abrir** igual.
   - Si en vez de eso te dice que "está dañada" y no te deja, abrí la
     Terminal y corré (una sola vez, cambiando la ruta si moviste la app):
     ```
     xattr -cr /Applications/Cartridge.app
     ```
     y volvé a intentar con click derecho → Abrir.
3. Las próximas veces ya abre normal con doble click.

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

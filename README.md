# Álvaro Fernández Mota

Desarrollador Python. Madrid.

Construyo sistemas que funcionan solos y se documentan a sí mismos: bots que
atienden a gente, infraestructura en casa, y modelos de IA corriendo en local
para que los datos no salgan de donde están.

---

## En qué estoy

### 🔔 [gjallarhorn](https://github.com/alvarofernandezmota-tech/gjallarhorn) — un recepcionista telefónico

Atiende la llamada, informa de tarifas y toma la cita. Pensado para negocios
pequeños, donde cada llamada que no se coge es una clienta que no vuelve.

Voz a texto y texto a voz **en local** (Whisper + Piper): lo que dice quien
llama no sale de la máquina. El cerebro va aparte, en su propio repo, y no
sabe por dónde le hablan — así el mismo cerebro sirve para el teléfono o para
cualquier otro canal.

`Python · systemd · Whisper · Piper · 426 pruebas`

### 📔 [bifrost](https://github.com/alvarofernandezmota-tech/bifrost) — un diario que entiende lo que le escribes

Bot de Telegram, **en producción** desde el 2026-09-08 en mi propio servidor.
Le escribes «recuérdame llamar al médico el jueves» y sale una tarea con su
fecha, no una línea de texto. Le mandas una nota de voz y la transcribe. Te
avisa de tus citas sin que se lo pidas.

El modelo **clasifica, nunca escribe**, y el camino que contesta preguntas no
puede tocar los datos — hay una prueba que lee el propio código para
garantizarlo. El cerebro se puede cambiar entre Claude y un modelo local con
una variable de entorno.

`Python · python-telegram-bot · systemd · Whisper · Ollama · 225 pruebas`

### 🎲 [bulletyroulet](https://github.com/alvarofernandezmota-tech/bulletyroulet) — Bones & Bullets

Juego de terminal: dados de póker donde relanzar es apretar el gatillo de un
revólver. Solo biblioteca estándar, sin dependencias. Tiene versión web de un
solo fichero y ejecutable para Windows y Linux.

[**Jugar en el navegador →**](https://alvarofernandezmota-tech.github.io/bulletyroulet/)

`Python · JavaScript · Canvas · PyInstaller · 41 pruebas`

---

## Cómo trabajo

- **Las decisiones se escriben.** 22 ADRs entre los proyectos: qué se decidió,
  qué se descartó y por qué. Un repo que no explica sus decisiones se convierte
  en arqueología a los seis meses.
- **Las fronteras se comprueban, no se prometen.** Donde hay una regla de
  arquitectura que importa, hay una prueba que lee el código y se cae si
  alguien la cruza.
- **Los números se miden antes de escribirlos.** Los recuentos de pruebas de
  arriba los verifica un test que falla si la documentación miente.
- **Lo que se puede hacer en local, se hace en local.** Voz y modelos
  corriendo en mi propia máquina: sin cuota, sin clave que caduque, y sin que
  lo que dice la gente salga de casa.

## Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Arch Linux](https://img.shields.io/badge/Arch_Linux-1793D1?style=flat&logo=arch-linux&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-local-black?style=flat)
![Tailscale](https://img.shields.io/badge/Tailscale-242424?style=flat&logo=tailscale&logoColor=white)

Servidor propio en Arch Linux con los servicios bajo systemd, dos máquinas
unidas por VPN mesh, y despliegue por `git pull` automático.

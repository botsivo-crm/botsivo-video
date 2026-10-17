# Botsivo Video

Editor de video local, basado en [Concat](https://github.com/jub0t/Concat)
(AGPL-3.0-or-later). Misma base nativa en Rust; marca e icono propios de
**Botsivo**.

## Qué cambia en este fork

- Marca e icono **Botsivo Video** (no usa el nombre ni el logo de Concat).
- Subtítulos automáticos con **ritmo estilo CapCut / Premiere**:
  - **Frase** — segmentos del transcriptor (Whisper).
  - **Línea** — ~4 palabras por cartela (default, ideal Shorts/Reels).
  - **Palabra** — una palabra a la vez (karaoke).
- Whisper con cortes en palabras y segmentos más cortos para empaquetar mejor.

## Licencia

AGPL-3.0-or-later. Si redistribuyes o vendes builds (sobre todo modificados),
debes ofrecer el código fuente correspondiente bajo AGPL. Este repositorio es
esa oferta pública.

Código de crates `concat-*`: herencia técnica del upstream; el producto que
ve el usuario se llama Botsivo Video.

## Upstream

- Proyecto original: https://github.com/jub0t/Concat
- Sitio upstream: https://concat.standalones.org

## Build / uso

Misma cadena que Concat: Rust reciente, FFmpeg 7+, cmake. Ver
[CONTRIBUTING.md](CONTRIBUTING.md) del árbol fuente.

```bash
cd src
cargo run -p concat
```

En Windows también puedes probar un build oficial de Concat para explorar la
UI; este repo es el código del fork Botsivo Video.

# Japón · dic 2026 – ene 2027

**https://yampo.github.io/japon-2026/**

Este repo es solo la **salida publicada**: un `index.html` autocontenido, sin
dependencias externas. Lo genera el taller de viajes, que es donde vive la
fuente (catálogo, itinerario, motor). Acá no se edita nada a mano.

El sitio se publica **saneado**: sin números de reserva ni apellidos. GitHub
Pages en cuenta gratuita obliga a que el repo sea público, así que `robots.txt`
y `noindex` le piden a los buscadores que no lo indexen — pero eso no lo hace
privado: cualquiera con la URL entra.

Para rearmarlo, desde el taller:

    python3 engine/build_all.py japon-2026 --publicar

## Las páginas de la época

    epoca.html      https://yampo.github.io/japon-2026/epoca.html
    epoca-pt.html   https://yampo.github.io/japon-2026/epoca-pt.html

La síntesis de la investigación de la época, en español y en portugués. Existen
para poder compartirlas con alguien que no tiene por qué instalarse ni
registrarse en nada: son dos archivos estáticos y se abren en cualquier teléfono.

**No las genera el build** —a diferencia de `index.html`— así que un `--publicar`
no las toca ni las borra, pero tampoco las actualiza. Si cambia el contenido, la
fuente es `trips/japon-2026/investigacion_epoca/EPOCA.md` en el taller y hay que
regenerar **las dos**: no están enlazadas entre sí y es fácil corregir una y
dejar la otra mintiendo.

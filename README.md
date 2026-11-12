# Mapeo curricular · Areandina · Contaduría Pública

Presentación de 11 láminas para la dirección del programa de Contaduría Pública de la
Fundación Universitaria del Área Andina: qué asignaturas del plan de estudios (pensum 202660)
pueden trabajarse con un simulador PraxiLab, con cuál y en qué semestre.

- **4 asignaturas con simulador**: 2 de aplicación directa y 2 como apoyo al curso, entre 5.º y 7.º semestre.
- **5 simuladores**: AudiTek, RentaSim, TerriTek, ProcediTek y SosteniTek ESG.

## Cómo verla

- **Sin cuenta ni conexión:** `presentacion.html` es la presentación completa en un solo archivo (tipografías y logotipo incrustados). Se abre con doble clic en cualquier navegador: flechas o clic para avanzar, `N` notas del presentador, `F` pantalla completa. Para PDF: Imprimir → Guardar como PDF.
- **De dónde sale cada dato:** el Excel del mapeo (cifras y asignaturas) y la guía docente de cada simulador (formato, horas y entregables).

## Qué hay aquí

```
presentacion.html                                 GENERADO: la presentación completa en un solo archivo.
deck.json                                         Índice: título, orden, secciones y tipografías.
slides/<id>.html                                  Una lámina por archivo: un solo <section id="<id>"> de 1920×1080
                                                  con estilos en línea. Las notas del presentador van en su <aside>.
tools/                                            El generador y sus recursos (tipografías, logotipo), copiados
                                                  del repo de marca. Ver tools/README.md.
```

El Excel del mapeo y el documento de trabajo (`CLAUDE.md`) son internos y no se suben al repositorio.

## Cómo actualizarla

1. Edita la lámina en `slides/`. Si cambias el número de láminas o su orden, edita también `deck.json` (el `order` lista exactamente los archivos de `slides/`) y renumera los pies.
2. Regenera `presentacion.html` con `node tools/presentacion-html.mjs .` desde esta carpeta. Nunca se edita a mano.

## Marca

Sigue la plantilla común de las guías docentes PraxiLab: papel y tinta, Archivo / Instrument Sans / Courier Prime, nada bajo 24 px, sin esquinas redondas. La franja va en el azul de marca y cada simulador conserva su matiz junto a su nombre.

PraxiLab · Grupo Edutec · praxilab.app

# orvin-sitio

Sitio público de Orvin — `orvin.digital`.

Landing de una sola página, estática y autocontenida. Sin build, sin dependencias, sin framework.

## Estructura

```
index.html   la página completa (HTML + CSS + JS en un archivo)
arte/        piezas generadas con Higgsfield (Recraft V4.1) en formato WebP
```

## Correr en local

```bash
python3 -m http.server 8813 --bind 127.0.0.1
```

Y abrir <http://127.0.0.1:8813>.

## Reglas de la pieza

- **Sistema visual: "Documentos"** del design system Orvin (`@orvin/ds v0.1.0`) — hero
  oscuro, cuerpo claro, cierre oscuro. No mezclar con los sistemas de Presentación
  ni de Contenido.
- **Todos los colores salen de los tokens `--ov-*`** declarados en `:root`. No
  agregar hex sueltos que ya existan como token.
- **El isotipo es la esfera de partículas** (verde → cian → azul), portada del bundle
  oficial con la misma semilla determinista. Nunca una galaxia naranja ni otro símbolo.
- **El arte se acredita.** Cada pieza generada lleva visible "generado por un agente
  Orvin": es la demostración de la capacidad, no decoración.
- **Presupuesto de peso: menos de 800 KB** por carga completa. Las imágenes van en
  WebP, las miniaturas de tarjeta a 800 px de ancho y todo lo que no está en el
  primer pantallazo con `loading="lazy"`.

## Origen

Los datos de mercado citados en la sección 01 provienen de MIT (State of AI in
Business), RAND y reportes de adopción 2025–2026. Las capacidades de la sección 02
corresponden a sistemas que Orvin opera en producción.

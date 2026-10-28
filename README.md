# Bordemundo

Prototipo de juego con la cámara del celular. Chispa camina y salta sobre los bordes de los objetos reales que ve la cámara y atrapa luciérnagas durante un minuto.

**Jugar:** https://cangothic.github.io/bordemundo/

## Modos

- **Cámara en vivo:** el terreno se actualiza en tiempo real. Si mueves la mano cerca de Chispa, lo lanzas por el aire.
- **Foto:** tomas una foto de tu mesa o repisa y juegas sobre ella.
- **Escenario de ejemplo:** una escena dibujada para probar sin cámara.

## Qué cuenta como suelo

- **Bordes:** las líneas casi horizontales de la imagen (detector Sobel sobre una cuadrícula de unos 3 px).
- **Tinta oscura:** lo que es más oscuro que su vecindario, ideal para dibujos con marcador en papel.

Al deslizar el dedo sobre la escena dibujas un puente que dura 6 segundos.

Todo el juego está en `index.html`, sin dependencias. La cámara en vivo exige https o `localhost`.

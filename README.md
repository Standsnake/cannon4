# cannon4
# Juego Cannon

> Este proyecto es una copia del juego Cannon en Python utilizando las librerías `turtle` y `freegames`. Permite al usuario disparar proyectiles mediante clics para impactar objetivos en movimiento.

## Funcionalidades Base
**Mecánicas y Controles:**
- Hacer clic en la pantalla con el ratón para lanzar un proyectil (bola roja) hacia la posición del cursor.
- El proyectil cuenta con simulación de gravedad durante su trayectoria.
- Impactar los objetivos (balones azules) para eliminarlos antes de que crucen la pantalla.
- La partida termina si algún objetivo logra llegar al borde izquierdo sin ser destruido.

## Funcionalidades agregadas
- Se aumentó la velocidad de movimiento tanto del proyectil como de los balones/objetivos para incrementar la dificultad y dinámica del juego.

## Cambios en el código
- En la función `tap()`, se redujo el divisor del cálculo del vector `speed` (de `25` a `15`) para darle mayor velocidad inicial al proyectil.
- En la función `move()`, se incrementó el desplazamiento horizontal de los objetivos (`target.x -= 2` en lugar de `0.5`) para acelerar su avance.

## Requisitos e Instalación
1. Asegurarse de tener Python 3 instalado.
2. Instalar la librería requerida:
```bash
pip install freegames

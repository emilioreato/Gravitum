<div align="center">
  <img src="files/Media/icon.png" alt="Icono de Gravitum" width="88">
  <h1>Gravitum</h1>
  <p>Un simulador interactivo 2D para crear cuerpos, observar su atracción y explorar el campo gravitatorio.</p>
</div>

Gravitum permite experimentar con sistemas de varios cuerpos: ajusta sus velocidades, observa cómo interactúan y cambia la forma de ver el campo.

## Choques y campo gravitatorio

Diez cuerpos de distintos tamaños se acercan y colisionan; sus campos se superponen en la primera captura. La segunda oculta los discos para destacar el campo de otra escena de diez cuerpos, comparado con las cuatro paletas disponibles.

<table width="100%">
  <tr>
    <th width="50%">Colisiones múltiples</th>
    <th width="50%">El campo en cuatro paletas</th>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <img src="docs/assets/gravitum-chaos-collision.png" alt="Diez cuerpos de distintos tamaños chocan en una escena oscura; sus campos gravitatorios rojos, naranjas y blancos se superponen." width="100%">
    </td>
    <td width="50%" valign="top">
      <img src="docs/assets/gravitum-field-palettes.jpg" alt="La misma escena de diez cuerpos sin los discos visibles, comparada en las paletas rojo y ámbar, blanco y rojo, violeta y hielo, y azul y dorado." width="100%">
    </td>
  </tr>
</table>

## De dos cuerpos a muchos

Con más entidades, las zonas de intensidad se combinan alrededor de todo el sistema:

<p align="center">
  <img src="docs/assets/gravitum-many-bodies.png" alt="Doce cuerpos distribuidos en una escena con cuadrícula y el campo gravitatorio visible alrededor de cada uno." width="100%">
</p>

## Colisiones y órbitas

La secuencia muestra dos cuerpos que se aproximan, entran en contacto y se separan tras la colisión. El GIF conserva 1024 × 640 píxeles para que el movimiento se lea con claridad sin cargar la captura completa.

<p align="center">
  <img src="docs/assets/gravitum-collision.gif" alt="Dos cuerpos se aproximan, colisionan y rebotan mientras cambia el campo gravitatorio." width="1024">
</p>

![Instante de contacto entre dos cuerpos durante una colisión, con el campo gravitatorio visible.](docs/assets/gravitum-collision.png)

El modo orbital asistido asigna una velocidad inicial tangencial al cuerpo pequeño. El GIF muestra una vuelta completa alrededor del cuerpo central, en 96 fotogramas a 1024 × 640.

<p align="center">
  <img src="docs/assets/gravitum-orbit.gif" alt="Vuelta completa de un cuerpo pequeño alrededor de una masa central, con el campo gravitatorio visible." width="1024">
</p>

## Cómo probarlo

1. Mantén pulsado el botón central del ratón y arrastra para crear un cuerpo; la distancia del arrastre determina su tamaño.
2. Haz clic derecho sobre un cuerpo y arrastra para darle una velocidad inicial; la flecha indica su dirección.
3. Pulsa `F` para mostrar u ocultar el campo y `T` para recorrer sus paletas de color.
4. Para probar el modo orbital, pulsa `O`, selecciona primero el cuerpo central y luego el cuerpo al que quieres asignar la velocidad orbital.

## Controles principales

| Control | Acción |
| --- | --- |
| Clic izquierdo y arrastrar | Seleccionar y mover un cuerpo |
| Clic central y arrastrar | Crear un cuerpo |
| Clic derecho y arrastrar sobre un cuerpo | Definir su velocidad inicial |
| Clic derecho y arrastrar en el fondo | Desplazar la cámara |
| `P` | Pausar o reanudar la simulación |
| `F` / `T` | Ocultar o mostrar el campo / cambiar su paleta |
| `D` / `G` / `A` | Mostrar detalles / cuadrícula / ejes |
| `C` / `R` / `K` | Centrar cámara / encuadrar cuerpos / reiniciar |
| `O` | Activar el modo de velocidad orbital asistida |
| `Espacio` / `Tab` | Acelerar mientras se mantiene pulsada la tecla |
| `B` | Invertir el sentido del tiempo mientras se mantiene pulsada |
| `H` | Abrir o cerrar la ayuda |
| `Esc` | Salir |

## Ejecutar en Windows

Con Python instalado, crea un entorno e instala las dependencias:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install pygame numpy opencv-python scipy numba pywin32
python files\main.py
```

La escena de colisión se renderizó a 1920 × 1200. La lámina de campo se generó con el renderizador de Gravitum. README y recursos visuales preparados con asistencia de IA; el código del proyecto no se modificó.

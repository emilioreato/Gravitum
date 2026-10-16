<div align="center">
  <img src="files/Media/icon.png" alt="Icono de Gravitum" width="88">
  <h1>Gravitum</h1>
  <p>Un simulador interactivo 2D para crear cuerpos, observar su atracción y explorar el campo gravitatorio con color.</p>
</div>

## El campo gravitatorio, en dos paletas

La captura oscura oculta los cuerpos para destacar el campo; la clara los muestra como referencia. Ambas se tomaron a 1536 × 960, con la simulación pausada.

| Paleta oscura | Paleta clara |
| --- | --- |
| ![Campo gravitatorio en paleta oscura, sin dibujar los cuerpos: solo quedan visibles las zonas de mayor intensidad en blanco y rojo.](docs/assets/gravitum-dark-field.png) | ![Campo gravitatorio en paleta clara con los cuatro cuerpos visibles para mostrar su posición y tamaño sobre el degradado.](docs/assets/gravitum-light-field.png) |

## Cómo probarlo

1. Pulsa el botón central del ratón y arrastra para crear un cuerpo; el tamaño del arrastre determina su radio.
2. Mantén el puntero sobre los cuerpos para observar cómo interactúan.
3. Pulsa `F` para mostrar u ocultar el campo y `T` para recorrer las paletas de color.
4. Usa la rueda del ratón para acercar o alejar la vista.

## Controles principales

| Control | Acción |
| --- | --- |
| Clic izquierdo y arrastrar | Seleccionar y mover un cuerpo |
| Clic central y arrastrar | Crear un cuerpo |
| Clic derecho y arrastrar sobre un cuerpo | Definir su velocidad inicial con la flecha |
| Clic derecho y arrastrar en el fondo | Desplazar la cámara |
| `P` | Pausar o reanudar la simulación |
| `F` / `T` | Ocultar o mostrar el campo / cambiar su paleta |
| `D` / `G` / `A` | Mostrar detalles / cuadrícula / ejes |
| `C` / `R` / `K` | Centrar cámara / encuadrar cuerpos / reiniciar |
| `O` | Activar el modo de velocidad orbital asistida |
| `Espacio` / `Tab` | Acelerar mientras se mantiene pulsada la tecla |
| `B` | Invertir el sentido del tiempo mientras se mantiene pulsada |
| `Esc` | Salir |

## Ejecutar en Windows

Con Python instalado, crea un entorno e instala las dependencias:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install pygame numpy opencv-python scipy numba pywin32
python files\main.py
```

README y capturas preparados con asistencia de IA. El código del simulador no se modificó.


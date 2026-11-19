# Recurso 1 · Ficha del repositorio OpenQuadruped

**Para quién:** quien quiera entender el proyecto original antes de construir algo inspirado en él. Se puede leer sin que el grupo esté presente.

## Origen de este recurso

Sale del análisis que el Grupo 2 hizo en el **Reto 5** (explorar un repositorio abierto y proponer una oportunidad). Cada dato indica en qué archivo se apoya; lo que no se pudo comprobar está marcado como **no verificado**.

## Datos básicos

| Dato | Información |
|---|---|
| Nombre | OpenQuadruped (`open-quadruped`) |
| Enlace | <https://github.com/adham-elarabawy/open-quadruped> |
| Autoría | Adham Elarabawy (creador y autor principal). Maurice Rahme aparece como colaborador que dio orientación técnica en la arquitectura de software y en un modelo URDF. |
| Licencia | MIT (copyright de Adham Elarabawy, 2020), con una disposición adicional que exige **dar crédito explícito y formal al creador original** y conservar el aviso de copyright y licencia. |
| Público objetivo | **No verificado:** el repositorio no declara un público. |

## Qué es

Un proyecto de robótica abierta para diseñar, construir y programar un **robot de cuatro patas** hecho sobre todo con piezas impresas en 3D. Combina:

- **12 grados de libertad (DOF):** tres articulaciones por cada una de las cuatro patas.
- **Curvas de Bézier:** generan las trayectorias que coordinan los pasos.
- **Cinemática inversa:** calcula los ángulos de las articulaciones para llevar la pata a una posición deseada.

(Ver términos en el [Glosario](glosario-y-faq-principiantes.md).)

## Cómo está organizado el control

Dos equipos: una **Jetson Nano** planifica movimientos y trayectorias, y un **Teensy** recibe las coordenadas de las patas, calcula los ángulos y controla los servomotores. Se comunican mediante **ROS**.

## Qué hay en el repositorio

Carpetas visibles en la raíz: `control_library/`, `depracated/RPi/`, `hardware/`, `llc-teensy/`, `media/`, `ros-workspace/` y `vis-tool/`. El contenido interno de varias **no pudo inspeccionarse**.

## Qué se verificó (con evidencia)

| Hallazgo | Dónde se ve |
|---|---|
| Robot cuadrúpedo impreso en 3D, con pasos por curvas de Bézier de 12 DOF y cinemática inversa de 3 DOF por pata. | [README.md](https://github.com/adham-elarabawy/open-quadruped/blob/master/README.md) |
| Licencia MIT que exige crédito explícito al creador. | [LICENSE](https://github.com/adham-elarabawy/open-quadruped/blob/master/LICENSE) |
| Placa electrónica personalizada para controlar 12 servomotores y conectar sensores; los archivos Gerber están en `hardware/`. | README y carpeta `hardware/` |
| Los archivos **STEP/STL sí existen**, en `hardware/3d-printing`, por secciones (cada una con su carpeta `step` y `stl`). | [Hardware 3D printing](https://github.com/adham-elarabawy/open-quadruped/tree/master/hardware/3d-printing) |
| Guía de conexiones eléctricas, con una **advertencia de seguridad** sobre el interruptor de alimentación para evitar cortocircuitos en la batería. | [Wiki – Wiring Diagram](https://github.com/adham-elarabawy/open-quadruped/wiki) |
| Guía para conectar una computadora a la Jetson Nano por Wi-Fi y SSH (no es una guía de ensamblaje completa). | [Wiki – Networking Setup](https://github.com/adham-elarabawy/open-quadruped/wiki) |
| El README reconoce trabajo pendiente: mejoras de hardware, pruebas automatizadas, simulación y calibración de servos; la herramienta de visualización con Matplotlib (versión 3.0.3) está en desarrollo y puede fallar. | README |
| El README menciona una carpeta `model/` con STEP/STL, lista de materiales y guías de construcción (en desarrollo); esa carpeta **no apareció** en la raíz consultada. | README |

## Qué NO se verificó

- Contenido actual de la **lista de materiales (BOM)** (enlace «Bill of Materials – OpenQuadruped» en el README).
- Existencia de una **guía completa de ensamblaje**.
- Existencia de **`CONTRIBUTING.md`** y normas oficiales de contribución. Canales disponibles: [Issues](https://github.com/adham-elarabawy/open-quadruped/issues) y [Pull Requests](https://github.com/adham-elarabawy/open-quadruped/pulls).

## Por qué empezar con una sola pata

El proyecto completo (12 servos, placa personalizada, Jetson Nano, Teensy y ROS) es complejo y costoso para quien recién empieza. Una pata permite aprender fabricación digital, electrónica, programación y cinemática con menor alcance y costo. Nuestro prototipo es una **adaptación educativa inspirada** en OpenQuadruped, **no** una reproducción certificada de su pata original.

## Atribución

Todo lo derivado de este proyecto debe conservar el crédito a **Adham Elarabawy** y el aviso de la licencia MIT.

Fuentes: repositorio, README, LICENSE y Wiki enlazados arriba; página técnica del autor: <https://elarabawy.com>.

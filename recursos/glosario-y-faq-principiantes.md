# Recurso 2 · Glosario y preguntas frecuentes para principiantes

**Para quién:** quien lee la documentación de OpenQuadruped (o la nuestra) y se topa con términos que no conoce. Se puede usar sin que el grupo esté presente.

## Origen de este recurso

Surge del rol de **«pregunta de principiante»** del Reto 5: revisar si una persona nueva entendería el proyecto. Las definiciones son **generales y sencillas**; si alguna no coincide con cómo se usa el término en OpenQuadruped, corrígela con un Pull Request. *(El grupo debe revisarlas antes de la entrega.)*

## Glosario

| Término | Qué significa, en sencillo |
|---|---|
| **Cuadrúpedo** | Robot de cuatro patas. |
| **Articulación** | Punto donde una parte del robot se mueve respecto a otra, como una rodilla. |
| **Grado de libertad (DOF)** | Cada movimiento independiente que puede hacer un mecanismo. En OpenQuadruped, cada pata tiene 3 y el robot completo, 12 (4 patas × 3). |
| **Servomotor (servo)** | Motor que puede girar hasta una posición angular indicada y mantenerla. Cada articulación de la pata usa uno. |
| **Cinemática inversa** | Cálculo que parte de «dónde quiero que quede el pie» y obtiene «qué ángulos deben tener las articulaciones». |
| **Curva de Bézier** | Curva suave definida por unos pocos puntos de control; sirve para dibujar la trayectoria que sigue el pie en cada paso. |
| **Microcontrolador** | Pequeño computador que ejecuta el programa de control y da órdenes a los servos. En el proyecto original se usa un Teensy. |
| **Jetson Nano** | Computador de placa única; en el proyecto original planifica movimientos y trayectorias. |
| **ROS** | Conjunto de herramientas para que las partes de un robot se comuniquen entre sí mediante mensajes. |
| **URDF** | Formato de archivo que describe la estructura de un robot (piezas y articulaciones) para simularlo o controlarlo. |
| **STEP / STL** | Formatos de modelos 3D. STL es el que suelen leer las impresoras 3D; STEP conserva más información para editar el diseño. |
| **Gerber** | Archivos que describen una placa electrónica para fabricarla. |
| **BOM (lista de materiales)** | Lista de todas las piezas y componentes que hay que conseguir. |
| **Atribución** | Dar crédito a quien creó el trabajo original, como exige la licencia del proyecto. |

## Preguntas frecuentes

**¿Necesito el robot completo?**
No. Nuestra propuesta es construir **una sola pata** de tres articulaciones.

**¿Puedo reutilizar todos los componentes de OpenQuadruped?**
No lo asumimos. Primero se verifica la compatibilidad de servomotores y microcontrolador con el diseño, **antes de comprar**.

**¿Dónde están los modelos 3D?**
Los archivos STEP/STL están en la carpeta `hardware/3d-printing` del repositorio original, por secciones. Ver la [ficha](ficha-openquadruped.md).

**¿Hay una guía de ensamblaje completa?**
No pudimos verificarla. Por eso este proyecto propone crear una guía educativa en español.

**¿Hay algún riesgo eléctrico?**
Sí. El proyecto original advierte sobre el interruptor de alimentación para evitar cortocircuitos en la batería. Lee su [guía de conexiones](https://github.com/adham-elarabawy/open-quadruped/wiki) antes de conectar nada.

**¿Puedo copiar y compartir lo que construya?**
Sí, respetando la licencia MIT y dando crédito explícito a Adham Elarabawy.

**¿Dónde pregunto si algo no se entiende?**
Abre un Issue en este repositorio.

---

Licencia CC BY 4.0. Falta un término: agrégalo con un Pull Request.

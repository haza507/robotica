# Entrega 3 · Plan de evolución y sostenibilidad

> **Principio:** el trabajo no debe depender de una sola persona. Somos ocho integrantes, así que cada tarea tiene titular y suplente, y rota.

## 1. Responsabilidades compartidas

| Responsabilidad | Qué hace | Rotación propuesta |
|---|---|---|
| **Facilitación** | Dirige la sesión de trabajo o de prueba. | Cambia en cada sesión. |
| **Documentación** | Registra en la bitácora lo que ocurrió, con evidencias. | Cambia en cada sesión; nunca la misma persona que facilita. |
| **Mirada de principiante** | Revisa si alguien nuevo entendería lo escrito. | Cambia cada etapa. |
| **Cuidado del repositorio** | Revisa Issues y Pull Requests y responde en un plazo de 7 días. | Cambia cada semana. |
| **Verificación de datos** | Confirma los puntos marcados como «no verificados» y actualiza las fichas. | Cambia cada etapa. |
| **Publicación** | Sube los cambios acordados a GitHub. | Cambia cada etapa; mínimo dos personas con acceso. |

**Regla de respaldo:** cada tarea tiene una persona titular y una suplente. Si alguien deja de participar, el repositorio debe seguir siendo suficiente para continuar.

## 2. Próximos rituales

Las fechas se fijarán con el grupo. La secuencia sigue las cinco etapas de la [ruta de construcción](../recursos/ruta-pata-robotica.md):

| Etapa | Ritual | Meta de facilitación |
|---|---|---|
| 1. Investigación | Verificar BOM, modelos STEP/STL y guía de ensamblaje; completar el inventario de materiales. | Facilita quien no investigó la etapa anterior. |
| 2. Diseño y adaptación | Elegir el diseño de referencia y preparar los archivos de fabricación. | Facilitación rotativa. |
| 3. Fabricación y ensamblaje | Imprimir, ensamblar, instalar servomotores y conectar el microcontrolador. | Facilitación rotativa. |
| 4. Programación y pruebas | Programar el control básico y probar movimientos individuales y coordinados. | Facilitación rotativa. |
| 5. Documentación y socialización | Sesión de prueba de la guía con otro equipo. | Facilita una persona externa al núcleo, si es posible. |

## 3. Cómo recibir a nuevos miembros

1. Le damos la bienvenida y le preguntamos qué sabe y qué le interesa (sin exigir conocimientos previos).
2. Le mostramos el [README](../README.md) y la [escalera de participación](../CONTRIBUTING.md).
3. Le sugerimos empezar por la [Ficha de OpenQuadruped](../recursos/ficha-openquadruped.md) y el [Glosario](../recursos/glosario-y-faq-principiantes.md).
4. Le pedimos que cuente qué no entendió en un Issue: esa es una contribución valiosa.
5. Le ayudamos a elegir su siguiente escalón.

## 4. Señales reales de comunidad

| Señal real | Cómo la reconocemos |
|---|---|
| **Recurrencia** | Las mismas personas externas regresan a probar o a aportar. |
| **Ayuda entre pares** | Alguien explica un término o resuelve una duda sin que intervenga el grupo fundador. |
| **Facilitación distribuida** | Una persona fuera del núcleo dirige una sesión. |
| **Reutilización de recursos** | Otro equipo usa la ficha, el glosario o la ruta sin que estemos presentes. |
| **Contribuciones externas** | Llega un Issue o un Pull Request de alguien fuera del grupo. |

**Métricas de vanidad (no las usamos como prueba de éxito):** estrellas, *likes*, seguidores, número de fotos o visitas al repositorio.

## 5. Cómo otra persona o grupo puede copiar o continuar este proyecto

1. Haz un *fork* del repositorio.
2. Lee la [Ficha de OpenQuadruped](../recursos/ficha-openquadruped.md) y **verifica los puntos marcados como no verificados**.
3. Sigue la [ruta de construcción](../recursos/ruta-pata-robotica.md) y registra todo en tu propia [bitácora](bitacora.md).
4. Conserva la atribución a Adham Elarabawy y el aviso de licencia MIT.
5. Abre un Issue contándonos cómo te fue.

## 6. Riesgos y cómo se atienden

| Riesgo | Qué haremos |
|---|---|
| La BOM o la guía de ensamblaje del proyecto original no se pueden confirmar. | Se mantienen marcadas como «no verificadas» y se abre un Issue para verificarlas. |
| Los componentes no son reutilizables directamente. | Se verifica la compatibilidad de servomotores y microcontrolador **antes de comprar**. |
| Falta de impresora 3D, materiales o presupuesto. | Se registran como recursos por confirmar; la guía puede avanzar en la parte documental. |
| Los enlaces del proyecto original dejan de funcionar. | Se revisan en cada etapa y se documenta la fecha de la última revisión. |
| Seguridad eléctrica (cortocircuito en la batería). | Toda guía de conexiones repite la advertencia sobre el interruptor de alimentación. |

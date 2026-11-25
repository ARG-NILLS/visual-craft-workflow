# Movimiento e interacción

## Activación

Usá esta referencia para animaciones, fondos en movimiento, transiciones de interfaz o revisión de motion. Para una pantalla estática, omitila. Si el proyecto ya trae un motor de animación, evaluá primero sus patrones y documentación vigente.

## Insumos

Identificá propósito, elemento, evento que inicia el movimiento, estado inicial y final, duración, repetición, posibilidad de interrupción, navegadores y dispositivos objetivo, frecuencia de uso, presupuesto de rendimiento y preferencia de movimiento reducido.

## Método

1. Asigná una función clara: respuesta a una acción, continuidad espacial, orientación o explicación. Si no aporta una de ellas, quitá o simplificá el movimiento.
2. Preferí CSS para transiciones acotadas. Considerá un timeline cuando haya secuencias coordinadas, sincronización, reproducción o interrupción con varios estados.
3. Ajustá la duración según lo que la persona necesita entender, la distancia y la frecuencia de uso. Un botón y un panel tienen exigencias distintas. Preferí transición reversible en feedback repetido y medí efectos de máscara, blur o layout en el navegador antes de asumir fluidez.
4. Respetá movimiento reducido. Reducí, detené o reemplazá movimiento no esencial; conservá los cambios de estado necesarios.
5. Permití detener o revertir secuencias interrumpibles. No dejes controles fuera de alcance, ocultos o sin respuesta mientras corre la animación.
6. En aplicaciones de una sola página, asociá listeners y timelines al ciclo de vida del componente. Limpiá, revertí o cancelá efectos cuando el componente se desmonte, cambie de ruta o se reemplace su estado. Evitá listeners globales duplicados.
7. Adaptá distancias, duración y composición a viewport, entrada táctil y contenido real. No dependas solo de hover o puntero.
8. Si se usa un motor externo, comprobá versión, ciclo de vida, alcance de selectores, limpieza y consultas de medios. Volvé a probar cuando cambie el breakpoint o la preferencia de movimiento con la interfaz abierta. En secuencias con video, comprobá la alternativa estática, el primer fotograma útil y la pausa fuera de vista cuando corresponda.

### Prueba de interrupción

Abrí un panel, cerralo antes de que termine la entrada y volvé a abrirlo. La transición debe continuar desde su posición visible y terminar en el estado de la última acción. Revisá que un callback anterior no vuelva a ocultarlo y que el texto conserve sus proporciones. Si hay tirones al desplazar el puntero, medí el costo antes de modificar el efecto.

## Entregable

Documentá propósito, disparador, estados, ritmo, interrupción, adaptación, comportamiento con movimiento reducido, dependencia y comprobaciones pendientes.

## Comprobaciones

Probá inicio, final, interrupción, cambio de ruta y desmontaje cuando correspondan. Revisá teclado, tacto, movimiento reducido, consola y rendimiento en dispositivos representativos. Una captura aislada no prueba continuidad, limpieza ni fluidez.

## Fuentes oficiales

Si el proyecto ya usa GSAP, consultá su [guía para React](https://gsap.com/resources/React/) para ciclo de vida y limpieza, y la [documentación de consultas de medios](https://gsap.com/docs/v3/GSAP/gsap.matchMedia%28%29/) para adaptar animaciones a viewport y movimiento reducido. Revisá también sus [términos de licencia vigentes](https://webflow.com/legal/product-terms); la licencia de esta skill no los reemplaza.

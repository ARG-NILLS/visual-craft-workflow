# Movimiento e interacción

## Activación

Usá esta referencia para animaciones, fondos en movimiento, transiciones de interfaz o revisión de motion. Para una pantalla estática, omitila. Si el proyecto ya trae un motor de animación, evaluá primero sus patrones y documentación vigente.

## Insumos

Identificá propósito, elemento, evento que inicia el movimiento, estado inicial y final, duración, repetición, posibilidad de interrupción, navegadores y dispositivos objetivo, frecuencia de uso, presupuesto de rendimiento y preferencia de movimiento reducido.

## Método

1. Asigná una función clara: respuesta a una acción, continuidad espacial, orientación o explicación. Si no aporta una de ellas, quitá o simplificá el movimiento.
2. Preferí CSS para transiciones acotadas. Considerá un timeline cuando haya secuencias coordinadas, sincronización, reproducción o interrupción con varios estados.
3. Mantené el movimiento breve y proporcional a la tarea. Evitá animar propiedades costosas o efectos amplios si una alternativa más simple comunica lo mismo.
4. Respetá movimiento reducido. Reducí, detené o reemplazá movimiento no esencial; conservá los cambios de estado necesarios.
5. Permití detener o revertir secuencias interrumpibles. No dejes controles fuera de alcance, ocultos o sin respuesta mientras corre la animación.
6. En aplicaciones de una sola página, asociá listeners y timelines al ciclo de vida del componente. Limpiá, revertí o cancelá efectos cuando el componente se desmonte, cambie de ruta o se reemplace su estado. Evitá listeners globales duplicados.
7. Adaptá distancias, duración y composición a viewport, entrada táctil y contenido real. No dependas solo de hover o puntero.
8. Si se usa un motor externo, consultá su documentación oficial vigente para ciclo de vida, limpieza y consultas de medios. No agregues una dependencia solo por preferencia.

## Entregable

Documentá propósito, disparador, estados, ritmo, interrupción, adaptación, comportamiento con movimiento reducido, dependencia y comprobaciones pendientes.

## Comprobaciones

Probá inicio, final, interrupción, cambio de ruta y desmontaje cuando correspondan. Revisá teclado, tacto, movimiento reducido, consola y rendimiento en dispositivos representativos. Una captura aislada no prueba continuidad, limpieza ni fluidez.

## Fuentes oficiales

Si el proyecto ya usa GSAP, consultá su [guía para React](https://gsap.com/resources/React/) para ciclo de vida y limpieza, y la [documentación de consultas de medios](https://gsap.com/docs/v3/GSAP/gsap.matchMedia%28%29/) para adaptar animaciones a viewport y movimiento reducido. Revisá también sus [términos de licencia vigentes](https://webflow.com/legal/product-terms); la licencia de esta skill no los reemplaza.

# Revisión de calidad

## Activación

Usá esta referencia para una auditoría de interfaz, una revisión técnica solicitada o la comprobación de una implementación. Elegí controles relacionados con el objetivo, la superficie y la evidencia disponible. No conviertas una lista completa en una obligación para cada tarea.

## Insumos

Revisá rutas, componentes, instrucciones del proyecto, plataformas objetivo, requisitos, navegador o dispositivo disponible, datos de prueba y criterios de aceptación. Distinguí inspección de código, captura renderizada, prueba con teclado, llamada de red y validación de backend: cada evidencia responde preguntas diferentes.

## Método

1. Definí alcance, tarea crítica y estados que deben revisarse.
2. Recorré la interfaz en el entorno disponible. Observá estructura, comportamiento, contenido y resultado visual.
3. Seleccioná controles pertinentes:
   - semántica, idioma y jerarquía de encabezados;
   - navegación, foco visible, orden de teclado y nombres de controles;
   - formularios, validación, errores, instrucciones y confirmación real;
   - carga, estado vacío, éxito, error, reintento y recuperación;
   - adaptación, zoom, contenido extenso y objetivos táctiles;
   - contraste, alternativa a efectos, movimiento reducido y lectura;
   - enlaces, rutas, metadatos, imágenes, recursos y enlaces rotos;
   - carga de fuentes, imágenes y video, consola, red y rendimiento observable;
   - privacidad, seguridad y localización cuando el alcance las incluya.
4. Registrá cada control como cumple, falla, pendiente o no aplica. Adjuntá ruta, estado, evidencia y método; separá observación de inferencia.
5. Priorizá por consecuencia: P0 impide una tarea esencial o crea riesgo grave; P1 causa un problema funcional, de acceso o confianza importante; P2 es una mejora de claridad o acabado. No uses la prioridad como puntuación estética.
6. Si una herramienta o dispositivo falta, marcá el control como pendiente y explicá el límite. No conviertas ausencia de cobertura en defecto confirmado.
7. Corregí solo lo autorizado. Repetí la comprobación afectada y revisá posibles regresiones cercanas.

## Entregable

Presentá alcance, entorno, controles revisados, hallazgos ordenados por prioridad y brechas de cobertura. Cada hallazgo incluirá ubicación, estado, evidencia observada, impacto y corrección concreta.

## Comprobaciones

Confirmá que los hallazgos puedan reproducirse en la ruta y estado indicados. No afirmes que una interfaz pasó accesibilidad, seguridad, SEO o rendimiento solo por usar una biblioteca o superar una revisión estática. Separá datos no verificados, opiniones visuales y fallas reproducibles.

## Fuentes oficiales

Para requisitos de accesibilidad web, contrastá el criterio aplicable con la [WCAG 2.2](https://www.w3.org/TR/WCAG22/). Para comportamiento o compatibilidad de una API, verificá documentación oficial vigente de la plataforma. Citá la fuente junto al hallazgo y explicá qué evidencia del proyecto conecta con ese requisito.

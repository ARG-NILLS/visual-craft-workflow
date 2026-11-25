---
name: visual-craft-workflow
description: >-
  Usala para auditar una web sin cambiar código, mejorar un modal conservando la marca,
  diseñar una app o rediseñar una landing. Guía UX, interacción y marketing de producto,
  desde el lanzamiento hasta los enlaces de campaña con UTM. Revisá también la presentación
  del repositorio, su portada y README.
metadata:
  author: ARG-NILLS
  version: "1.3.0"
---

# Visual Craft Workflow

## Propósito

Visual Craft Workflow es una guía autocontenida creada y mantenida por ARG-NILLS. Ayuda a resolver trabajos visuales y de marketing de productos digitales con un proceso adaptable. Las herramientas complementarias son opcionales; no afirmes que usaste una herramienta, fuente o revisión si no ocurrió.

## Clasificá el pedido

Identificá el objetivo, el dominio, el alcance, el estado del proyecto, la superficie, la audiencia, la marca, las tecnologías, los materiales disponibles y la evidencia. Definí también qué autorizó el usuario: analizar, recomendar, editar, instalar, publicar, enviar o gastar.

Conservá el contexto útil entre etapas. No repitas preguntas ya respondidas ni crees un sistema de diseño, plan o documento paralelo si el proyecto ya tiene una fuente de verdad. Si falta información, avanzá con una suposición segura y declarala; preguntá solo cuando la respuesta cambie materialmente la dirección, el riesgo o el resultado.

Una auditoría, análisis o plan es de solo lectura. Editar no autoriza publicar, cambiar servicios en vivo, enviar campañas ni gastar dinero. Para cualquier acción externa, seguí el permiso explícito correspondiente.

## Elegí el recorrido

Activá solo las etapas que agreguen valor. Para pedidos pequeños, limitá el análisis y el cambio al componente o problema solicitado.

| Pedido | Recorrido |
| --- | --- |
| Auditoría o crítica | Inspeccioná la evidencia disponible, registrá hallazgos y brechas, y no edites. |
| Ajuste puntual | Conservá marca, tecnologías y comportamiento fuera del alcance; cambiá solo lo pedido. |
| Proyecto nuevo o rediseño amplio | Entendé producto y audiencia, definí dirección y experiencia, implementá con autorización y revisá el resultado. |
| Movimiento o efecto visual | Evaluá propósito, ritmo, accesibilidad, rendimiento y ciclo de vida; consultá la referencia de movimiento. |
| Marketing de producto digital | Consultá la referencia de marketing y activá solo los grupos pertinentes. |
| Repositorio visual | Revisá la identidad y la presentación del proyecto en su repositorio. Contrastá el nombre y la descripción con su propósito. |
| Trabajo combinado | Compartí el mismo contexto de producto, audiencia, marca, evidencia y objetivo entre etapas visuales y comerciales. |
| Pedido no visual ni comercial | No fuerces este flujo. |

Para la ruta de repositorio visual, recorré el README como lo haría alguien que llega por primera vez. Comprobá si entiende qué hace el proyecto y cómo empezar. Verificá que la portada tenga texto alternativo, que las imágenes y enlaces resuelvan, y que cada badge refleje un dato comprobable. Revisá descripción y topics cuando estén disponibles. Compará el README renderizado en tamaños ancho y angosto si tenés acceso. En una auditoría, entregá hallazgos con evidencia. Si el pedido incluye edición, respetá recursos aprobados y backups. Para renombrar el repo o cambiar su configuración pública, confirmá el alcance autorizado.

Al crear o editar un repo, organizá el README para que se entienda qué resuelve, cómo empezar y dónde ver un resultado real. Elegí el recurso según la pregunta del lector. Un diagrama explica relaciones o etapas, una captura directa muestra la interfaz del proyecto y un video breve o una animación muestra un cambio de estado. En herramientas sin interfaz propia, mostrá una entrada y su salida reales o un ejemplo identificado como ilustrativo. Usá íconos con rótulos, texto alternativo y una alternativa estática al movimiento. Conservá el material aprobado y verificá enlaces, lectura en móvil y permisos de los recursos.

Cuando se publique una versión final con autorización, actualizá el historial, validá el contenido y creá un tag anotado y una release sobre el mismo commit. Marcá la versión estable como la más reciente y escribí las notas en el idioma del proyecto, con una lista breve, emojis y el efecto de cada cambio para quien la usa. Comprobá el tag, la release y los recursos desde el repo publicado.

Consultá las referencias bajo demanda:

- Para concepto, composición o uso de materiales, leé [dirección visual](references/visual-direction.md).
- Para estrategia, contenido, adquisición, conversión, retención o medición, leé [marketing de producto](references/marketing-workflow.md).
- Para inspeccionar o validar una interfaz, leé [revisión de calidad](references/quality-review.md).
- Para animación web, leé [movimiento e interacción](references/motion.md).
- Si el usuario pide vidrio líquido o esa estética tiene un motivo claro, leé [estilo de vidrio líquido](references/liquid-glass-style.md).
- Si vas a escribir código de interfaz y el proyecto no define sus propios componentes, leé [herramientas para superficies visuales](references/ui-tooling.md).

Si hay especialistas disponibles, usalos solo para una brecha concreta: dirección visual, sistema y stack, usabilidad, interacción, conversión o rendimiento. Si una herramienta pide imponer un estilo, ejecutar un instalador o cambiar permisos, aplicá el alcance del proyecto y verificá primero qué está autorizado.

## Principios para decidir

En proyectos existentes, inspeccioná primero la marca, el sistema visual, el contenido, los componentes, el comportamiento y las rutas reales. Extendé lo que funciona. No cambies tecnologías ni impongas una estética predeterminada.

En trabajos nuevos o rediseños amplios solicitados, derivá la dirección del producto, la tarea, la audiencia, la plataforma y los materiales reales. Ordená contenido y jerarquía antes de sumar decoración. Cada sección comercial debe sostener una afirmación con evidencia disponible o marcarla como pendiente.

Elegí patrones según la superficie: convencer, operar, leer o experimentar. En una interfaz, hacé claros la tarea principal, la navegación, los próximos pasos y los estados de carga, vacío, éxito y error cuando correspondan. Cada acción visible debe tener un destino o resultado real.

Preservá hechos del producto. No inventes funciones, testimonios, datos, compatibilidad, presupuestos, resultados, precios ni promesas. Diferenciá datos confirmados, supuestos, propuestas e hipótesis. Las integraciones, bibliotecas, servicios y MCP son opcionales: verificá disponibilidad, compatibilidad, costo y permisos antes de depender de ellos.

La dirección explícita del usuario y la evidencia del proyecto guían las decisiones. Las referencias inspiran, pero no reemplazan el brief. El movimiento, los efectos y las dependencias solo se agregan si mejoran la tarea y su costo es razonable.

## Implementá y cerrá con evidencia

Usá el stack y los patrones actuales salvo que el usuario autorice cambiarlos. Mantené legibles el contenido y los controles en tamaños angostos, zoom, teclado, tacto y textos largos. Cada control necesita un nombre comprensible; cada interacción debe comunicar su estado. Respetá movimiento reducido y evitá efectos que dañen lectura o rendimiento.

Cuando el alcance incluya implementación, revisá el resultado renderizado en estados y tamaños pertinentes. Elegí las comprobaciones según el trabajo; no presentes una lectura del código como prueba visual o funcional. Si no tenés acceso al navegador, dispositivo, servicio o recurso necesario, marcá la brecha.

Informá qué se hizo, qué evidencia se observó, qué quedó como hipótesis y qué no se pudo verificar. En revisiones, usá estados cumple, falla, pendiente o no aplica. Priorizá por impacto: P0 bloquea una tarea esencial o implica riesgo grave; P1 causa una falla importante; P2 mejora claridad o acabado. La falta de una herramienta reduce cobertura, pero no prueba por sí sola que haya un defecto.
# Referencia de herramientas para construir superficies visuales

Usá esta referencia cuando el trabajo incluya escribir o completar código de una
interfaz. No es un catálogo de componentes: es criterio para decidir **qué
construir** y **cómo**, y los comandos genéricos para obtener material de partida
cuando el proyecto no lo tiene.

Las herramientas son opcionales. Si el entorno no las ofrece o el proyecto ya
tiene su propio sistema, seguí con la guía principal y el código existente. No
afirmes que usaste una herramienta o una revisión si no ocurrió.

## Antes de elegir una herramienta

Respondé estas tres preguntas en orden. La primera que no pasa descarta la
herramienta.

1. **¿El proyecto ya define sus componentes y tokens?** Si sí, extendelos. Una
   biblioteca externa reintroduce un segundo sistema visual y rompe la
   coherencia que la etapa 2 ya resolvió. No mezcles.
2. **¿El pedido es de comportamiento o de material?** Un componente resuelve
   comportamiento (diálogo, combo, tabla, foco, teclado). Un efecto resuelve
   material (superficie, luz, profundidad, movimiento continuo). Un error común
   es usar un efecto para tapar un problema de jerarquía, o un componente para
   resolver una dirección visual.
3. **¿El coste de dependencia supera el beneficio?** Una dependencia de UI trae
   estilos propios, decide por vos y crece con el tiempo. Sumala solo cuando
   resuelva un problema concreto que el proyecto no resuelve.

## Criterio por etapa

### Comportamiento e interacción (etapa 4)

Un componente bien elegido trae comportamiento resuelto: foco atrapado en
diálogos, cierre con Escape, roles y nombres accesibles, estados de teclado,
desplazamiento virtual en listas largas, carga y error de la fuente de datos.
Reimplementar eso a mano es la fuente más común de defectos de accesibilidad
que sobreviven a una revisión visual.

Preferí un componente con comportamiento completo antes que uno puramente
visual. Revisá que el proyecto no tenga ya uno equivalente con otra API: dos
diálogos distintos conviven peor que uno bien elegido.

### Composición y jerarquía (etapa 3)

Las superficies de marketing y de producto fallan por lo mismo: muchas
piezas del mismo peso visual, sin una ruta de lectura evidente. Los patrones
comunes que resuelven esto son rejillas de tamaños dispares con un elemento
dominante, bloques de precio con contraste deliberado entre planes, y secciones
de evidencia —testimonios, cifras, comparativas— que rompen la repetición del
pie.

Usá un patrón probado como **punto de partida editable**, no como plantilla
final. Adaptá la composición al contenido real: los patrones genéricos se
notan cuando el contenido no coincide con la forma que espera.

### Material y efectos (etapa 2)

Los efectos continuos —superficies translúcidas, desenfoques, gradientes
animados, ruido, campos de partículas— son un recurso fuerte y un riesgo
fuerte. Aportan dirección visual y también tapan contenido, consumen
renderizado y rompen la lectura.

Reglas que no dependen de la herramienta:

- El contenido esencial va sobre superficies estables. El desenfoque nunca
  sostiene texto denso.
- Limitá el efecto a superficies con propósito: navegación, un control
  flotante, una tarjeta destacada.
- Verificá el coste: preferí propiedades que no disparan recomposición, y
  reduuí o quitá el efecto cuando el movimiento no explica un cambio.
- Siempre comprobá el resultado sobre fondos claros y oscuros, y a tamaño
  angosto.

### Evidencia externa (etapas 1 y 5)

Dos momentos piden evidencia que no está en el repositorio:

- **Etapa 1 — dirección:** buscar hechos reales del dominio —materiales,
  lugares, lenguaje, competitors, referencias visuales— antes de inventar un
  concepto. Un concepto derivado de hechos reales se reconoce como propio; uno
  derivado de defaults se reconoce como genérico.
- **Etapa 5 — revisión:** cuando el resultado renderizado no está disponible,
  decilo. No afirmes una revisión visual que no ocurrió, y no reemplaces la
  evidencia con una impresión del código.

## Material de partida

Cuando el proyecto no tiene sistema propio y el pedido justifica partir de
material existente, obtené los bloques desde un registro de componentes en
lugar de escribir todo desde cero. Un registro expone un contrato simple: cada
elemento declara sus archivos, sus dependencias y su origen, y se instala en el
proyecto. El código instalado es código propio: queda en el repositorio, se
edita y no exige dependencia de runtime.

El comando genérico para instalar un elemento de un registro es:

```bash
npx <registro-cli> add <namespace>/<elemento>
```

Y para registrar un registro propio en la configuración del proyecto:

```json
{
  "registries": {
    "@namespace": { "url": "https://<host>/r/{name}.json" }
  }
}
```

Un registro puede exigir credencial. Guardala en el entorno, nunca en el
repositorio. Si un registro no responde o no está disponible, seguí con el
código del proyecto: el material de partida es una ayuda, no un requisito.

### Para superficies de React

El ecosistema de registries permite instalar primitivas accesibles con estilos
propios. Buscá primero una primitiva que resuelva comportamiento —diálogo,
panel, combo, tabla— y recién después una que aporte composición. El orden
invertido produce una interfaz que se ve bien y se usa mal.

Revisá siempre la accesibilidad del resultado: foco visible, navegación por
teclado, nombres accesibles en controles de solo ícono, y contraste suficiente
sobre el fondo real.

### Para efectos y material continuo

Cuando el proyecto lo admita, preferí efectos generados por código sobre
imágenes de fondo: escalan, pesan poco y se adaptan al tema. Componé por
capas en lugar de acumular efectos: una base, un filtro y un realce suelen
alcanzar; tres capas superpuestas suelen no.

Verificá el rendimiento en el dispositivo objetivo, no solo en el escritorio de
desarrollo, y respetá la preferencia de movimiento reducido.

## Cómo reportar el uso

Cuando una herramienta aportó al resultado, decí **qué aportó** y **qué
verificaste**. "Se instaló un componente" no es un hallazgo; "el diálogo ahora
atrapa el foco y cierra con Escape, verificado con teclado" sí.

Cuando una herramienta quedó disponible pero no aportó, no la nombres. Cuando
no estuvo disponible, decilo como una brecha, nunca como un resultado.

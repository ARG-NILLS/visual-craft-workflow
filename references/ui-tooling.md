# Herramientas para superficies visuales

## Activación

Usá esta referencia al construir o completar código de interfaz cuando el proyecto no tenga un componente adecuado. Omitila para auditorías de solo lectura y si el proyecto ya resuelve el problema con patrones coherentes.

## Insumos

Revisá stack, componentes, tokens, dependencias, licencias, problema de comportamiento o material, necesidades de accesibilidad, restricciones de ejecución y costo de mantenimiento.

## Método

1. Definí si falta comportamiento, composición o material. Un efecto visual no corrige una jerarquía confusa; un componente interactivo no define por sí solo una dirección visual.
2. Revisá primero lo que ya existe. Extendé el sistema cuando sea suficiente. Una biblioteca o primitiva compatible puede cubrir una brecha concreta si respeta marca, stack, accesibilidad y mantenimiento.
3. Compará beneficio, dependencia, peso, licencias, API, accesibilidad, compatibilidad y alternativa de falla. Si consultás un catálogo, filtrá por la versión del stack y tratá la salida como una propuesta. Contrastá tokens y patrones con el sistema existente antes de aplicarlos.
4. Si evaluás un registro de componentes, verificá el comando y formato en su documentación vigente. Los comandos y manifiestos varían; cualquier ejemplo genérico es esquemático y no debe ejecutarse como universal.
5. Si incorporás código generado o copiado, registrá la revisión de origen y revisá el cambio antes de ejecutar instaladores, hooks o binarios. Comprobá licencia, avisos y dependencias. El material instalado puede incluir paquetes de ejecución, activos con derechos propios o requisitos que permanecen después de copiarlo al repositorio.
6. No agregues credenciales al proyecto. Si el recurso no está disponible, seguí con las herramientas actuales o proponé una alternativa.

Para controles complejos, evaluá semántica, foco, teclado, estados, errores y uso táctil. Para efectos, evaluá lectura, contraste, movimiento reducido y costo de renderizado. Para recursos externos, revisá derechos y atribuciones aplicables.

## Entregable

Indicá la brecha que se resuelve, la opción elegida, el costo y la licencia comprobados, y el comportamiento que se validó. Si no agregaste nada, no lo presentes como una integración realizada.

## Comprobaciones

Confirmá que la API exista en la versión objetivo, que las dependencias y licencias estén claras, que los controles funcionen sin puntero y que el efecto tenga una alternativa aceptable. La revisión del código fuente no prueba el comportamiento renderizado.
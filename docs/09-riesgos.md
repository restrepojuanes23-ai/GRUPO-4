# 09 · Gestión de riesgos

En este documento presentamos los riesgos que identificamos al implementar en la tienda Carlos Díaz Esmeraldas el joyero en forma de mano impreso en 3D. El usuario principal es Carlos Díaz, administrador de la tienda, quien lo usará a diario para organizar y exhibir los anillos. La solución es un objeto físico y maneja muy pocos datos: solo el nombre, la edad y el cargo del administrador, además de las observaciones de la prueba. El presupuesto del proyecto es de $100.000 COP y condiciona varias de nuestras decisiones.

Valoramos cada riesgo con la fórmula **nivel = probabilidad (1-5) × impacto (1-5)**. Los rangos son: 1-4 bajo, 5-9 medio, 10-16 alto y 20-25 crítico.

## Matriz de riesgos

| ID | Riesgo | Categoría | P | I | Nivel | Tratamiento | Acción | Responsable | Fecha |
|---|---|---|---|---|---|---|---|---|---|
| R1 | Fragilidad o falla de la pieza impresa: los dedos o la base rotatoria pueden romperse o quedar inestables con el peso de los anillos. | Tecnológico | 3 | 4 | 12 (Alto) | Mitigar | Imprimir primero una versión de prueba a escala reducida. Hacer una prueba de carga con anillos reales y reforzar el grosor de los dedos y el eje de la base antes de la impresión definitiva. | PR | 7 nov 2025 |
| R2 | Pérdida de archivos de diseño y registros: se pueden perder o dañar los archivos 3D y las evidencias de la prueba. | Datos y ciberseguridad | 2 | 2 | 4 (Bajo) | Transferir | Guardar los archivos de diseño y la documentación en el repositorio de GitHub y mantener una copia de respaldo en la nube. No subir fotos de clientes ni datos personales. | AP | 14 nov 2025 |
| R3 | Rechazo o abandono del exhibidor: el administrador puede volver a guardar los anillos en cajas y bolsas si el joyero le resulta poco práctico. | Personas y adopción | 3 | 3 | 9 (Medio) | Mitigar | Involucrar al administrador en la revisión de la versión 0.1. Hacer una demostración corta de uso y recoger sus ajustes durante la semana de prueba. | UX | 12 nov 2025 |
| R4 | Presupuesto insuficiente para reimpresiones: el límite de $100.000 COP puede agotarse si hay que repetir impresiones por errores o ajustes. | Financiero | 4 | 4 | 16 (Alto) | Mitigar | Reservar $30.000 COP del presupuesto para reimpresiones. Hacer una sola impresión de prueba a escala reducida y validar el diseño antes de la versión final. Registrar cada gasto. | LP | 5 nov 2025 |
| R5 | Uso indebido de datos personales: el nombre, la edad y el cargo del administrador, o las opiniones de clientes, pueden tratarse sin autorización (Ley 1581 de 2012). | Legal | 2 | 2 | 4 (Bajo) | Evitar | Pedir autorización escrita al administrador para usar sus datos con fines académicos. No recolectar datos de clientes: solo anotar observaciones generales sin nombres ni imágenes de personas. | LP | 14 nov 2025 |
| R6 | Anillos que no encajan en los soportes: la variedad de tamaños y diseños puede dejar piezas flojas o sin lugar en el joyero. | Operativo | 3 | 2 | 6 (Medio) | Mitigar | Medir los diámetros de los anillos más vendidos y ajustar el grosor y la separación de los soportes de los dedos. Definir con el administrador cuáles piezas se exhiben en el joyero. | UX | 10 nov 2025 |

## Riesgos altos y críticos

No identificamos riesgos críticos. Los dos riesgos altos son los siguientes.

### R4 · Presupuesto insuficiente para reimpresiones (nivel 16)

- **Por qué preocupa:** con $100.000 COP, cada impresión fallida reduce el margen para terminar el prototipo.
- **Plan:** el 5 de noviembre de 2025 el líder del proyecto (LP) reserva $30.000 COP exclusivamente para reimpresiones y lleva un registro de gastos. Antes de la impresión definitiva se valida el diseño con una pieza de prueba a escala reducida.
- **Seguimiento:** revisamos el saldo después de cada impresión. Si queda menos del monto reservado, simplificamos el diseño antes de imprimir de nuevo.

### R1 · Fragilidad o falla de la pieza impresa (nivel 12)

- **Por qué preocupa:** el joyero debe sostener varios anillos sobre un mostrador concurrido. Si se rompe o se inclina, el desorden y la pérdida de piezas que queremos resolver aumentarían.
- **Plan:** el 7 de noviembre de 2025 el responsable del prototipo (PR) hace una prueba de carga con anillos reales y refuerza los dedos y el eje de la base rotatoria. Después de cada ajuste se verifica la estabilidad sobre el mostrador.
- **Seguimiento:** durante la semana de prueba el administrador reporta cualquier inestabilidad, y la corregimos antes de la entrega final.

## Mapa de calor

![Mapa de calor de riesgos](../assets/matriz-riesgos.png)

### Cómo leer el mapa de calor

Cada riesgo aparece en la casilla donde se cruzan qué tan probable es (de abajo hacia arriba) y cuánto daño haría (de izquierda a derecha). El color va del verde, que significa tranquilidad, al rojo, que significa urgencia. En nuestro proyecto, los que quedaron más arriba y a la derecha son *Presupuesto insuficiente para reimpresiones* y *Fragilidad o falla de la pieza impresa*. Preocupan porque contamos solo con $100.000 COP y porque el joyero debe aguantar el uso diario en el mostrador de Carlos Díaz. Por eso lo primero que haremos es reservar dinero para reimpresiones y probar la resistencia de la pieza con anillos reales. En el centro quedaron *Rechazo o abandono del exhibidor* y *Anillos que no encajan en los soportes*, que atendemos con la revisión del administrador y la medición de los anillos. En zona verde quedaron *Pérdida de archivos de diseño y registros* y *Uso indebido de datos personales*, porque manejamos muy pocos datos y bastan el respaldo en la nube y la autorización escrita.

## Conclusión

El riesgo se concentra en el presupuesto limitado y en la resistencia de la pieza impresa. Si los atendemos antes del 18 de noviembre, el joyero puede probarse con seguridad en la tienda.


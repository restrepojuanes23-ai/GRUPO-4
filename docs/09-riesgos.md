# 09 · Gestión de riesgos

En este documento presentamos la matriz de riesgos de implementar en Carlos Diaz Esmeraldas el joyero en forma de mano impreso en 3D. La tienda ofrece bisutería y accesorios, principalmente anillos y collares, a jóvenes y estudiantes universitarios. La solución la usará a diario el vendedor de la tienda, junto con la administradora, y contamos con un presupuesto de 100.000 pesos. Evaluamos cada riesgo con la fórmula **probabilidad (1-5) × impacto (1-5) = nivel**. Los niveles son: 1-4 bajo, 5-9 medio, 10-16 alto y 20-25 crítico.

## Matriz de riesgos

| ID | Riesgo | Categoría | P | I | Nivel | Tratamiento | Acción | Responsable | Fecha |
|---|---|---|---|---|---|---|---|---|---|
| R1 | Fallas de impresión o inestabilidad del joyero: los dedos se rompen o la base rotatoria se inclina con el peso de los anillos. | Tecnológico | 4 | 4 | 16 (Alto) | Mitigar | Imprimir primero una versión de prueba a escala reducida, reforzar el grosor de los dedos y de la base, y probar la estabilidad con anillos reales antes de imprimir la versión final. | AP | 4 de noviembre |
| R2 | Pérdida de archivos de diseño e inventario: se pierden los modelos 3D o el listado de anillos y collares. | Datos y ciberseguridad | 2 | 2 | 4 (Bajo) | Transferir | Guardar los archivos de diseño y el listado de accesorios en el repositorio de GitHub y en una carpeta en la nube con contraseña, con acceso solo para los integrantes del equipo. | PR | 7 de noviembre |
| R3 | Baja adopción del joyero: el vendedor y la administradora siguen guardando los anillos en cajas y bolsas por costumbre. | Personas y adopción | 3 | 4 | 12 (Alto) | Mitigar | Hacer una demostración corta de uso con el vendedor y la administradora, entregar una guía ilustrada de una página y pedirles opinión sobre el diseño durante la semana de prueba. | UX | 11 de noviembre |
| R4 | Sobrecosto por reimpresiones: los ajustes de diseño agotan el presupuesto de 100.000 pesos. | Financiero | 3 | 3 | 9 (Medio) | Mitigar | Dividir el presupuesto por etapas, reservar 20.000 pesos para ajustes, limitar a dos las impresiones completas y registrar cada gasto de material. | LP | 6 de noviembre |
| R5 | Datos personales en la prueba (Ley 1581 de 2012): fotos o comentarios identificables de clientes durante la validación. | Legal | 2 | 2 | 4 (Bajo) | Evitar | No recolectar nombres, imágenes ni datos de contacto de clientes. Registrar las observaciones de forma anónima y, si fuera necesario un dato personal, solicitar antes la autorización del titular conforme a la Ley 1581 de 2012. | PR | 5 de noviembre |
| R6 | Hurto o caída de anillos en exhibición: al quedar visibles, las piezas pueden sustraerse o caerse del joyero. | Operativo | 3 | 4 | 12 (Alto) | Mitigar | Ubicar el joyero cerca de la caja y a la vista del vendedor, exhibir solo una cantidad limitada de anillos por turno y contar las piezas al abrir y al cerrar la tienda. | LP | 12 de noviembre |

## Riesgos altos y críticos

No identificamos riesgos críticos. Los tres riesgos de nivel alto son los siguientes.

### R1 · Fallas de impresión o inestabilidad del joyero (nivel 16)
Es el riesgo más alto porque somos un equipo de primer semestre con poca experiencia en impresión 3D, y el diseño en forma de mano tiene piezas delgadas que soportan peso. Si falla, no podemos probar la hipótesis. **Plan:** imprimir una versión de prueba a escala reducida, reforzar los dedos y la base, y verificar la estabilidad con anillos reales antes de la impresión final. Responsable: AP, antes del 4 de noviembre.

### R3 · Baja adopción del joyero por el personal (nivel 12)
La solución solo funciona si el vendedor y la administradora dejan de guardar los anillos en cajas y bolsas sueltas. **Plan:** hacer una demostración corta de uso, entregar una guía ilustrada de una página y recoger sus opiniones durante la semana de prueba para ajustar el diseño. Responsable: UX, antes del 11 de noviembre.

### R6 · Hurto o caída de anillos en exhibición (nivel 12)
Exhibir los anillos los hace más visibles para los clientes, pero también más expuestos a pérdidas, que son parte del problema que queremos resolver. **Plan:** ubicar el joyero cerca de la caja y a la vista del vendedor, limitar la cantidad de anillos exhibidos por turno y contar las piezas al abrir y al cerrar. Responsable: LP, antes del 12 de noviembre.

![Mapa de calor de riesgos](../assets/matriz-riesgos.png)

### Cómo leer el mapa de calor

Cada riesgo aparece en la casilla donde se cruzan dos cosas: qué tan probable es que ocurra, de abajo hacia arriba, y cuánto daño haría si ocurre, de izquierda a derecha. El color va del verde, que significa tranquilo, al rojo, que significa urgente. En nuestro proyecto, lo que quedó más arriba y a la derecha es *Fallas de impresión o inestabilidad*. Preocupa porque somos nuevos en impresión 3D y, si el joyero no sostiene los anillos, no podemos validar nada, así que lo primero que haremos es imprimir una versión de prueba a escala reducida. Un escalón más abajo están *Baja adopción del joyero por el personal* y *Hurto o caída de anillos en exhibición*. En la tienda de Carlos Diaz Esmeraldas el joyero solo sirve si el vendedor y la administradora lo usan a diario, y exhibir los anillos los deja más a la vista. *Sobrecosto por reimpresiones* queda en la zona media, y lo controlamos con el límite de 100.000 pesos. En verde están *Pérdida de archivos de diseño e inventario* y *Datos personales en la prueba (Ley 1581)*, porque ya tenemos respaldo en GitHub y no vamos a recoger datos de clientes, así que basta con vigilarlos.

## Conclusión

El mayor peligro del proyecto es técnico y humano, no financiero ni legal: que el joyero falle al sostener los anillos o que el personal no lo use.
Con las acciones de mitigación, programadas antes del 18 de noviembre y dentro del presupuesto de 100.000 pesos, esperamos llegar a la prueba con los riesgos altos bajo control.

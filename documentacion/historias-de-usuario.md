# Historias de usuario y requerimientos — Control financiero para microempresarios

**Proyecto:** control-financiero-microempresarios
**Asignatura:** INF-4334 Gestión de Configuración de Software
**Propuesta de:** Andreina De L. R.

Este documento recoge las 35 historias de usuario (requerimientos) del proyecto. Cada una tiene su título, su historia (Como / quiero / para), criterios de aceptación y prioridad, y se registra como un issue en el repositorio. El texto de cada bloque se pega tal cual en la descripción del issue.

## Labels

| Label | Uso |
|---|---|
| `historia-usuario` | Las 35 historias de usuario |
| `requerimiento` | Disponible para clasificar requerimientos |
| `bug` | Errores detectados durante el desarrollo |
| `prioridad-alta` | Prioridad alta |
| `prioridad-media` | Prioridad media |
| `prioridad-baja` | Prioridad baja |

## Resumen

| N.º | Título del issue | Prioridad |
|---|---|---|
| 1 | Historia - Registrar mi negocio | Media |
| 2 | Historia - Iniciar sesión | Media |
| 3 | Historia - Editar los datos del negocio | Baja |
| 4 | Historia - Registrar un ingreso | Alta |
| 5 | Historia - Editar un ingreso | Media |
| 6 | Historia - Eliminar un ingreso | Media |
| 7 | Historia - Registrar un gasto | Alta |
| 8 | Historia - Editar un gasto | Media |
| 9 | Historia - Eliminar un gasto | Media |
| 10 | Historia - Anotar la referencia de un comprobante | Baja |
| 11 | Historia - Usar categorías predefinidas | Alta |
| 12 | Historia - Crear una categoría propia | Media |
| 13 | Historia - Editar o eliminar una categoría | Baja |
| 14 | Historia - Ver el balance actual | Alta |
| 15 | Historia - Ver el resumen mensual | Alta |
| 16 | Historia - Ver un gráfico de ingresos y gastos | Media |
| 17 | Historia - Ver el historial de movimientos | Alta |
| 18 | Historia - Filtrar el historial por fechas | Media |
| 19 | Historia - Filtrar por categoría o tipo | Media |
| 20 | Historia - Buscar un movimiento | Baja |
| 21 | Historia - Generar un reporte mensual | Media |
| 22 | Historia - Exportar los movimientos a CSV | Media |
| 23 | Historia - Definir un presupuesto mensual por categoría | Media |
| 24 | Historia - Recibir aviso al superar el presupuesto | Baja |
| 25 | Historia - Establecer una meta de ahorro | Baja |
| 26 | Historia - Registrar una cuenta por cobrar | Alta |
| 27 | Historia - Registrar el abono de un cliente | Alta |
| 28 | Historia - Registrar una cuenta por pagar | Media |
| 29 | Historia - Ver las cuentas vencidas | Baja |
| 30 | Historia - Respaldar y restaurar los datos | Media |
| 31 | Historia - Validar los montos que registro | Alta |
| 32 | Historia - Ver el balance actualizado automáticamente | Alta |
| 33 | Historia - Conservar mis datos al cerrar la página | Alta |
| 34 | Historia - Ver los montos en pesos dominicanos | Media |
| 35 | Historia - Usar la herramienta desde mi celular | Alta |

---

## 1. Historia - Registrar mi negocio
**Labels:** `historia-usuario`, `prioridad-media`

```
Como microempresario,
quiero registrar el nombre y el tipo de mi negocio,
para personalizar la herramienta con la información de mi emprendimiento.

Criterios de aceptación:
- El sistema debe mostrar un formulario de registro del negocio la primera vez que se use.
- El sistema debe pedir el nombre del negocio (obligatorio) y el tipo de negocio.
- El sistema debe mostrar un mensaje de error si el nombre del negocio está vacío.
- El sistema debe guardar los datos del negocio al presionar el botón "Guardar".
- El sistema debe mostrar el nombre del negocio en la pantalla principal.

Prioridad: Media
```

## 2. Historia - Iniciar sesión
**Labels:** `historia-usuario`, `prioridad-media`

```
Como microempresario registrado,
quiero iniciar sesión con mi usuario y contraseña,
para que solo yo pueda ver la información financiera de mi negocio.

Criterios de aceptación:
- El sistema debe mostrar un formulario de inicio de sesión con los campos "Usuario" y "Contraseña".
- El sistema debe validar que el usuario y la contraseña coincidan con los datos registrados.
- El sistema debe permitir el acceso al panel principal cuando los datos sean correctos.
- El sistema debe mostrar un mensaje de error cuando los datos sean incorrectos, sin indicar cuál de los dos falló.
- El sistema debe ofrecer la opción "Cerrar sesión" en todas las pantallas.

Prioridad: Media
```

## 3. Historia - Editar los datos del negocio
**Labels:** `historia-usuario`, `prioridad-baja`

```
Como propietario del negocio,
quiero editar los datos de mi negocio,
para mantener la información actualizada.

Criterios de aceptación:
- El sistema debe ofrecer una opción para editar los datos del negocio.
- El sistema debe mostrar el formulario con los datos actuales ya cargados.
- El sistema debe permitir modificar el nombre y el tipo de negocio.
- El sistema debe validar que el nombre no quede vacío antes de guardar.
- El sistema debe reflejar los cambios de inmediato en la pantalla principal.

Prioridad: Baja
```

## 4. Historia - Registrar un ingreso
**Labels:** `historia-usuario`, `prioridad-alta`

```
Como microempresario,
quiero registrar un ingreso con su monto, fecha, categoría y descripción,
para saber cuánto dinero entra a mi negocio.

Criterios de aceptación:
- El sistema debe presentar una opción llamada "Registrar ingreso" en la pantalla principal.
- El sistema debe presentar un formulario con los campos "Monto, Fecha, Categoría y Descripción".
- El sistema debe validar que el monto sea mayor que cero y que la fecha y la categoría estén completas.
- El sistema debe guardar el ingreso al presionar el botón "Guardar".
- El sistema debe mostrar el ingreso en el historial de movimientos.
- El sistema debe actualizar el balance automáticamente.

Prioridad: Alta
```

## 5. Historia - Editar un ingreso
**Labels:** `historia-usuario`, `prioridad-media`

```
Como microempresario,
quiero corregir un ingreso ya registrado,
para arreglar los errores que cometo al digitar.

Criterios de aceptación:
- El sistema debe ofrecer una opción "Editar" en cada ingreso del historial.
- El sistema debe mostrar el formulario con los datos actuales del ingreso.
- El sistema debe permitir cambiar el monto, la fecha, la categoría y la descripción.
- El sistema debe aplicar las mismas validaciones que al registrar un ingreso.
- El sistema debe recalcular el balance con el nuevo valor.
- El sistema debe mostrar el dato actualizado en el historial.

Prioridad: Media
```

## 6. Historia - Eliminar un ingreso
**Labels:** `historia-usuario`, `prioridad-media`

```
Como microempresario,
quiero eliminar un ingreso registrado por equivocación,
para que mis cuentas reflejen solo movimientos reales.

Criterios de aceptación:
- El sistema debe ofrecer una opción "Eliminar" en cada ingreso del historial.
- El sistema debe pedir confirmación antes de eliminar.
- El sistema debe eliminar el ingreso solo si el usuario confirma.
- El sistema debe quitar el ingreso del historial.
- El sistema debe recalcular el balance.

Prioridad: Media
```

## 7. Historia - Registrar un gasto
**Labels:** `historia-usuario`, `prioridad-alta`

```
Como microempresario,
quiero registrar un gasto con su monto, fecha, categoría y descripción,
para saber en qué se va el dinero de mi negocio.

Criterios de aceptación:
- El sistema debe presentar una opción llamada "Registrar gasto" en la pantalla principal.
- El sistema debe presentar un formulario con los campos "Monto, Fecha, Categoría y Descripción".
- El sistema debe validar que el monto sea mayor que cero y que la fecha y la categoría estén completas.
- El sistema debe guardar el gasto al presionar el botón "Guardar".
- El sistema debe mostrar el gasto en el historial de movimientos.
- El sistema debe actualizar el balance automáticamente.

Prioridad: Alta
```

## 8. Historia - Editar un gasto
**Labels:** `historia-usuario`, `prioridad-media`

```
Como microempresario,
quiero corregir un gasto ya registrado,
para mantener mis cuentas exactas.

Criterios de aceptación:
- El sistema debe ofrecer una opción "Editar" en cada gasto del historial.
- El sistema debe mostrar el formulario con los datos actuales del gasto.
- El sistema debe permitir cambiar el monto, la fecha, la categoría y la descripción.
- El sistema debe aplicar las mismas validaciones que al registrar un gasto.
- El sistema debe recalcular el balance con el nuevo valor.
- El sistema debe mostrar el dato actualizado en el historial.

Prioridad: Media
```

## 9. Historia - Eliminar un gasto
**Labels:** `historia-usuario`, `prioridad-media`

```
Como microempresario,
quiero eliminar un gasto registrado por error,
para que mi balance no se vea afectado por datos incorrectos.

Criterios de aceptación:
- El sistema debe ofrecer una opción "Eliminar" en cada gasto del historial.
- El sistema debe pedir confirmación antes de eliminar.
- El sistema debe eliminar el gasto solo si el usuario confirma.
- El sistema debe quitar el gasto del historial.
- El sistema debe recalcular el balance.

Prioridad: Media
```

## 10. Historia - Anotar la referencia de un comprobante
**Labels:** `historia-usuario`, `prioridad-baja`

```
Como microempresario,
quiero anotar el número o la referencia de la factura o el recibo de un gasto,
para tener un respaldo si necesito comprobarlo después.

Criterios de aceptación:
- El sistema debe incluir en el formulario de gasto un campo opcional llamado "Referencia del comprobante".
- El sistema debe permitir guardar el gasto aunque ese campo esté vacío.
- El sistema debe guardar la referencia junto con el gasto.
- El sistema debe mostrar la referencia en el detalle del gasto.
- El sistema debe permitir editar la referencia después de guardar.

Prioridad: Baja
```

## 11. Historia - Usar categorías predefinidas
**Labels:** `historia-usuario`, `prioridad-alta`

```
Como microempresario,
quiero contar con categorías ya creadas (como ventas, compra de mercancía, servicios y transporte),
para clasificar mis movimientos sin configurar nada al empezar.

Criterios de aceptación:
- El sistema debe incluir al menos 6 categorías predefinidas.
- El sistema debe separar las categorías de ingreso de las de gasto.
- El sistema debe mostrar las categorías en una lista desplegable en los formularios de ingreso y de gasto.
- El sistema debe tener las categorías disponibles desde el primer uso, sin configuración previa.
- El sistema debe impedir que las categorías predefinidas se eliminen.

Prioridad: Alta
```

## 12. Historia - Crear una categoría propia
**Labels:** `historia-usuario`, `prioridad-media`

```
Como microempresario,
quiero crear mis propias categorías,
para adaptar la clasificación a mi tipo de negocio.

Criterios de aceptación:
- El sistema debe ofrecer una opción llamada "Nueva categoría".
- El sistema debe pedir el nombre de la categoría y si es de ingreso o de gasto.
- El sistema debe validar que el nombre no esté vacío ni repetido.
- El sistema debe guardar la categoría al presionar el botón "Guardar".
- El sistema debe mostrar la nueva categoría en los formularios de registro.

Prioridad: Media
```

## 13. Historia - Editar o eliminar una categoría
**Labels:** `historia-usuario`, `prioridad-baja`

```
Como microempresario,
quiero editar o eliminar las categorías que creé,
para mantener mi lista ordenada.

Criterios de aceptación:
- El sistema debe ofrecer las opciones "Editar" y "Eliminar" en las categorías creadas por el usuario.
- El sistema debe mostrar el nombre nuevo en los movimientos asociados cuando se renombre una categoría.
- El sistema debe avisar antes de eliminar una categoría que tenga movimientos asociados.
- El sistema debe pedir confirmación antes de eliminar.
- El sistema debe impedir eliminar las categorías predefinidas.

Prioridad: Baja
```

## 14. Historia - Ver el balance actual
**Labels:** `historia-usuario`, `prioridad-alta`

```
Como microempresario,
quiero ver mi balance actual (ingresos menos gastos),
para saber en qué situación está mi negocio.

Criterios de aceptación:
- El sistema debe mostrar en la pantalla principal el total de ingresos, el total de gastos y el balance.
- El sistema debe calcular el balance como ingresos menos gastos.
- El sistema debe destacar visualmente el balance cuando sea negativo.
- El sistema debe actualizar los valores al registrar, editar o eliminar movimientos.
- El sistema debe mostrar los montos en pesos dominicanos (RD$).

Prioridad: Alta
```

## 15. Historia - Ver el resumen mensual
**Labels:** `historia-usuario`, `prioridad-alta`

```
Como microempresario,
quiero ver el resumen de ingresos y gastos de un mes,
para comparar cómo me fue en cada periodo.

Criterios de aceptación:
- El sistema debe ofrecer un selector de mes y año.
- El sistema debe mostrar el mes actual por defecto.
- El sistema debe mostrar los totales de ingresos, gastos y el balance del mes elegido.
- El sistema debe actualizar el resumen al cambiar el mes o el año.
- El sistema debe mostrar un mensaje cuando el mes elegido no tenga movimientos.

Prioridad: Alta
```

## 16. Historia - Ver un gráfico de ingresos y gastos
**Labels:** `historia-usuario`, `prioridad-media`

```
Como microempresario,
quiero ver un gráfico de mis ingresos y gastos,
para entender mis números de un vistazo.

Criterios de aceptación:
- El sistema debe mostrar un gráfico que compare los ingresos y los gastos del periodo seleccionado.
- El sistema debe usar colores distintos para los ingresos y los gastos.
- El sistema debe incluir una leyenda que explique los colores.
- El sistema debe actualizar el gráfico al cambiar el periodo.
- El sistema debe mostrar un mensaje cuando no haya datos para graficar.

Prioridad: Media
```

## 17. Historia - Ver el historial de movimientos
**Labels:** `historia-usuario`, `prioridad-alta`

```
Como microempresario,
quiero ver la lista de todos mis movimientos, del más reciente al más antiguo,
para revisar lo que he registrado.

Criterios de aceptación:
- El sistema debe mostrar una lista con todos los movimientos registrados.
- El sistema debe mostrar en cada fila la fecha, el tipo, la categoría, la descripción y el monto.
- El sistema debe ordenar los movimientos del más reciente al más antiguo.
- El sistema debe distinguir visualmente los ingresos de los gastos.
- El sistema debe mostrar un mensaje cuando todavía no haya movimientos.

Prioridad: Alta
```

## 18. Historia - Filtrar el historial por fechas
**Labels:** `historia-usuario`, `prioridad-media`

```
Como microempresario,
quiero filtrar el historial por un rango de fechas,
para revisar un periodo específico.

Criterios de aceptación:
- El sistema debe ofrecer campos para elegir una fecha inicial y una fecha final.
- El sistema debe mostrar solo los movimientos dentro del rango elegido.
- El sistema debe validar que la fecha inicial no sea posterior a la fecha final.
- El sistema debe ofrecer una opción para quitar el filtro.
- El sistema debe mostrar un mensaje cuando no haya resultados.

Prioridad: Media
```

## 19. Historia - Filtrar por categoría o tipo
**Labels:** `historia-usuario`, `prioridad-media`

```
Como microempresario,
quiero filtrar mis movimientos por categoría o por tipo (ingreso o gasto),
para analizar rubros concretos de mi negocio.

Criterios de aceptación:
- El sistema debe ofrecer un filtro por categoría y un filtro por tipo de movimiento.
- El sistema debe mostrar solo los movimientos que cumplan el filtro elegido.
- El sistema debe permitir combinar estos filtros con el filtro de fechas.
- El sistema debe ofrecer una opción para quitar los filtros.
- El sistema debe mostrar un mensaje cuando no haya resultados.

Prioridad: Media
```

## 20. Historia - Buscar un movimiento
**Labels:** `historia-usuario`, `prioridad-baja`

```
Como microempresario,
quiero buscar un movimiento por su descripción,
para encontrarlo rápido sin recorrer toda la lista.

Criterios de aceptación:
- El sistema debe ofrecer una caja de búsqueda en el historial.
- El sistema debe buscar por texto parcial de la descripción.
- El sistema debe ignorar las diferencias entre mayúsculas y minúsculas.
- El sistema debe mostrar los resultados al presionar el botón "Buscar".
- El sistema debe mostrar un mensaje cuando no haya coincidencias.

Prioridad: Baja
```

## 21. Historia - Generar un reporte mensual
**Labels:** `historia-usuario`, `prioridad-media`

```
Como contador o asesor del negocio,
quiero un reporte mensual con los totales por categoría,
para revisar las finanzas del negocio.

Criterios de aceptación:
- El sistema debe permitir elegir el mes y el año del reporte.
- El sistema debe mostrar el total de cada categoría, separando ingresos y gastos.
- El sistema debe mostrar el balance final del mes.
- El sistema debe mostrar el nombre del negocio y el periodo en el encabezado del reporte.
- El sistema debe mostrar un mensaje cuando el mes no tenga movimientos.

Prioridad: Media
```

## 22. Historia - Exportar los movimientos a CSV
**Labels:** `historia-usuario`, `prioridad-media`

```
Como microempresario,
quiero exportar mis movimientos a un archivo CSV,
para abrirlos en Excel o compartirlos con mi contador.

Criterios de aceptación:
- El sistema debe ofrecer un botón llamado "Exportar a CSV".
- El sistema debe generar un archivo con la fecha, el tipo, la categoría, la descripción y el monto de cada movimiento.
- El sistema debe respetar los filtros que estén activos al exportar.
- El sistema debe descargar el archivo en el dispositivo del usuario.
- El sistema debe mostrar un mensaje cuando no haya movimientos para exportar.

Prioridad: Media
```

## 23. Historia - Definir un presupuesto mensual por categoría
**Labels:** `historia-usuario`, `prioridad-media`

```
Como microempresario,
quiero definir un presupuesto mensual de gasto por categoría,
para controlar cuánto puedo gastar en cada rubro.

Criterios de aceptación:
- El sistema debe permitir definir un presupuesto mensual para una categoría de gasto.
- El sistema debe validar que el monto del presupuesto sea mayor que cero.
- El sistema debe mostrar el monto presupuestado frente al monto gastado en el mes.
- El sistema debe mostrar cuánto dinero queda disponible en cada categoría.
- El sistema debe permitir editar el presupuesto.

Prioridad: Media
```

## 24. Historia - Recibir aviso al superar el presupuesto
**Labels:** `historia-usuario`, `prioridad-baja`

```
Como microempresario,
quiero recibir un aviso cuando los gastos de una categoría superen su presupuesto,
para no pasarme sin darme cuenta.

Criterios de aceptación:
- El sistema debe comparar el gasto del mes de cada categoría con su presupuesto.
- El sistema debe mostrar una advertencia cuando el gasto supere el presupuesto.
- El sistema debe indicar cuánto se excedió.
- El sistema debe permitir registrar el gasto aunque se haya superado el presupuesto.
- El sistema debe omitir la advertencia en las categorías que no tengan presupuesto.

Prioridad: Baja
```

## 25. Historia - Establecer una meta de ahorro
**Labels:** `historia-usuario`, `prioridad-baja`

```
Como microempresario,
quiero establecer una meta de ahorro con un monto objetivo,
para planificar cuánto quiero acumular.

Criterios de aceptación:
- El sistema debe permitir crear una meta con un nombre y un monto objetivo.
- El sistema debe validar que el monto objetivo sea mayor que cero.
- El sistema debe permitir registrar el monto ahorrado hasta el momento.
- El sistema debe mostrar el porcentaje alcanzado de la meta.
- El sistema debe indicar cuando la meta se haya cumplido.

Prioridad: Baja
```

## 26. Historia - Registrar una cuenta por cobrar
**Labels:** `historia-usuario`, `prioridad-alta`

```
Como microempresario,
quiero registrar lo que un cliente me debe, con su nombre, monto y fecha límite,
para no olvidar el dinero que me deben.

Criterios de aceptación:
- El sistema debe ofrecer una opción llamada "Registrar cuenta por cobrar".
- El sistema debe pedir el nombre del cliente, el monto y la fecha límite de pago.
- El sistema debe validar que el nombre esté completo y que el monto sea mayor que cero.
- El sistema debe mostrar la deuda en una lista de cuentas por cobrar.
- El sistema debe mostrar el total pendiente por cobrar.

Prioridad: Alta
```

## 27. Historia - Registrar el abono de un cliente
**Labels:** `historia-usuario`, `prioridad-alta`

```
Como microempresario,
quiero registrar el abono que hace un cliente a su deuda,
para saber cuánto falta por cobrar.

Criterios de aceptación:
- El sistema debe ofrecer una opción "Registrar abono" en cada cuenta por cobrar.
- El sistema debe validar que el abono sea mayor que cero y no supere el saldo pendiente.
- El sistema debe actualizar el saldo de la deuda después de cada abono.
- El sistema debe guardar la fecha de cada abono.
- El sistema debe marcar la deuda como saldada cuando el saldo llegue a cero.

Prioridad: Alta
```

## 28. Historia - Registrar una cuenta por pagar
**Labels:** `historia-usuario`, `prioridad-media`

```
Como microempresario,
quiero registrar lo que le debo a un proveedor, con su monto y fecha de pago,
para pagar a tiempo.

Criterios de aceptación:
- El sistema debe ofrecer una opción llamada "Registrar cuenta por pagar".
- El sistema debe pedir el nombre del proveedor, el monto y la fecha de pago.
- El sistema debe validar que el monto sea mayor que cero.
- El sistema debe mostrar la deuda en una lista de cuentas por pagar.
- El sistema debe permitir marcar la cuenta como pagada.

Prioridad: Media
```

## 29. Historia - Ver las cuentas vencidas
**Labels:** `historia-usuario`, `prioridad-baja`

```
Como microempresario,
quiero ver destacadas las cuentas por cobrar o por pagar que ya vencieron,
para darles seguimiento a tiempo.

Criterios de aceptación:
- El sistema debe considerar vencida una cuenta cuando su fecha límite sea anterior a la fecha actual y aún tenga saldo pendiente.
- El sistema debe resaltar las cuentas vencidas en las listas de cuentas por cobrar y por pagar.
- El sistema debe mostrar en la pantalla principal cuántas cuentas vencidas hay.
- El sistema debe dejar de resaltar una cuenta cuando se salde.

Prioridad: Baja
```

## 30. Historia - Respaldar y restaurar los datos
**Labels:** `historia-usuario`, `prioridad-media`

```
Como microempresario,
quiero descargar una copia de mis datos y poder restaurarla,
para no perder mi información si cambio de dispositivo.

Criterios de aceptación:
- El sistema debe ofrecer un botón llamado "Descargar respaldo".
- El sistema debe generar un archivo con todos los datos del usuario.
- El sistema debe ofrecer una opción llamada "Restaurar respaldo" que permita elegir un archivo.
- El sistema debe validar que el archivo sea un respaldo válido antes de cargarlo.
- El sistema debe pedir confirmación antes de reemplazar los datos actuales.
- El sistema debe mostrar un mensaje de error, sin modificar los datos, cuando el archivo no sea válido.

Prioridad: Media
```

## 31. Historia - Validar los montos que registro
**Labels:** `historia-usuario`, `prioridad-alta`

```
Como microempresario,
quiero que el sistema revise que los montos que escribo sean válidos,
para evitar errores que dañen mis cuentas.

Criterios de aceptación:
- El sistema debe rechazar los montos que contengan letras o símbolos, o que estén vacíos.
- El sistema debe rechazar los montos iguales a cero o negativos.
- El sistema debe mostrar un mensaje claro que indique el error.
- El sistema debe impedir guardar el movimiento hasta que el monto sea corregido.
- El sistema debe aplicar esta validación a ingresos, gastos, presupuestos, metas, deudas y abonos.

Prioridad: Alta
```

## 32. Historia - Ver el balance actualizado automáticamente
**Labels:** `historia-usuario`, `prioridad-alta`

```
Como microempresario,
quiero que el balance se actualice solo cuando registro, edito o elimino un movimiento,
para no tener que hacer cálculos a mano.

Criterios de aceptación:
- El sistema debe calcular el balance como el total de ingresos menos el total de gastos.
- El sistema debe recalcular el balance al registrar, editar o eliminar un movimiento.
- El sistema debe actualizar el balance sin que el usuario tenga que recargar la página.
- El sistema debe mostrar un balance igual a la suma de los movimientos del historial.

Prioridad: Alta
```

## 33. Historia - Conservar mis datos al cerrar la página
**Labels:** `historia-usuario`, `prioridad-alta`

```
Como microempresario,
quiero que mis datos se conserven cuando cierro o recargo la página,
para no perder lo que ya registré.

Criterios de aceptación:
- El sistema debe guardar los datos en el navegador después de cada cambio.
- El sistema debe mostrar los datos guardados al abrir o recargar la página.
- El sistema debe conservar los datos al cerrar y volver a abrir el navegador.
- El sistema debe iniciar vacío y sin errores cuando no existan datos guardados.

Prioridad: Alta
```

## 34. Historia - Ver los montos en pesos dominicanos
**Labels:** `historia-usuario`, `prioridad-media`

```
Como microempresario dominicano,
quiero ver todos los montos en pesos dominicanos (RD$) con un formato claro,
para entender mis cuentas sin confusión.

Criterios de aceptación:
- El sistema debe mostrar todos los montos con el símbolo RD$.
- El sistema debe usar separador de miles y dos decimales (por ejemplo, RD$ 1,250.00).
- El sistema debe usar el mismo formato en todas las pantallas y reportes.
- El sistema debe mostrar el signo negativo en los balances negativos.

Prioridad: Media
```

## 35. Historia - Usar la herramienta desde mi celular
**Labels:** `historia-usuario`, `prioridad-alta`

```
Como microempresario,
quiero usar la herramienta desde mi celular, tablet o computadora,
para llevar mis cuentas desde cualquier lugar de mi negocio.

Criterios de aceptación:
- El sistema debe adaptar el diseño al ancho de pantalla de celular, tablet y computadora.
- El sistema debe evitar el desplazamiento horizontal en pantallas de 360 px de ancho.
- El sistema debe mostrar botones y campos con un tamaño cómodo para usar con el dedo.
- El sistema debe permitir leer las tablas del historial en el celular.

Prioridad: Alta
```

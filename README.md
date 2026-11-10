# Diagnóstico inmobiliario Argos

Diagnóstico de cumplimiento LC/FT/FPADM para inmobiliarias y agentes inmobiliarios (LOCDOFT, art. 9, num. 10, lit. a), con la misma propuesta comercial de `argos-diagnostico`.

## Uso en la visita al cliente

1. El cliente, o el dueño acompañado de su abogado, responde las 20 preguntas en `index.html`.
2. El resultado separa las brechas en dos grupos: las que cubre Argos y las que cubre la asesoría de cumplimiento. Las marcadas "Argos + asesoría" necesitan ambas.
3. "Continuar: recibir mi propuesta" abre `propuesta/nueva/` con el sector Inmobiliaria ya elegido y genera el presupuesto del plan mensual, semestral o anual, o de la consulta única.

## Qué cambia frente a `argos-diagnostico`

- `index.html`: preguntas, textos y clasificación de brechas propios del sector inmobiliario. El cálculo es el mismo: 0, 0,5 y 1 por respuesta, peso 3 para los controles críticos, BAJO hasta 25 %, MODERADO hasta 50 % y ALTO por encima, con subida de nivel por controles críticos.
- `propuesta/nueva/index.html`: deja preseleccionado el sector que trae el diagnóstico y rotula como "Lo cubre la asesoría" las brechas que no cubre Argos.
- Precios, planes, propuesta final (`propuesta/`), alta y consulta: sin cambios. Los precios viven en `assets/argos.js`.

Si se cambian los precios en `argos-diagnostico`, hay que copiarlos aquí también.

## Fuentes de las preguntas

LOCDOFT (arts. 4, 10, 11, 13, 14, 16 y 18), Circular ONCDOFT-DGCJ 003-2026 (RUSO), Evaluación Sectorial de Riesgos 2026 de la ONCDOFT (abogados, contadores y agentes inmobiliarios), Guía EBR y Guía DDC 2026 de la Cámara Inmobiliaria de Venezuela, y Recomendaciones 1, 10, 12, 18, 22 y 23 del GAFI.

# Resumen Ejecutivo — VentaExpress Q4 2024

## Contexto
VentaExpress opera en México y Colombia en el sector tecnología.
El dataset del Q4 2024 llegó con errores de captura, correos malformados,
caracteres especiales y tipos de dato inconsistentes que impedían generar
reportería confiable.

## Proceso de Limpieza
- Sin duplicados: verificados tomando como llave el ID de orden
- 19 registros vacíos en columnas "precio" y "monto" imputados con regla
  de tres; equivalen al 1.9% del total
- Correos malformados: identificados y corregidos
- Tipos de dato normalizados: fechas, montos y categorías a formato uniforme
- Caracteres especiales, espacios en blanco y abreviaciones en nombres
  personales corregidos mediante fórmulas de depuración

## Hallazgos Principales

| Métrica | Resultado |
|---|---|
| Ventas totales Q4 2024 | $3,053,684.32 |
| Venta promedio por transacción | $3,899.98 |
| Número total de transacciones | 783 |
| Producto más vendido (cantidad) | Laptop Oficina 32GB — 116 piezas / $321,991.69 |
| Mes con mejores resultados | Octubre |
| Precio promedio por categoría | $1,256,212.44 (4 categorías, col. "Especificaciones") |

## Ranking de Ciudades por Volumen de Ventas

| Posición | Ciudad | Monto Total |
|---|---|---|
| 1 | Ciudad de México | $556,084.37 |
| 2 | Monterrey | $548,597.88 |
| 3 | Cali | $513,664.93 |
| 4 | Guadalajara | $495,168.42 |
| 5 | Bogotá | $479,480.77 |
| 6 | Medellín | $406,293.22 |
| 7 | Tulum | $54,394.73 |
| **Total** | | **$3,053,684.32** |

## Anomalías Detectadas
- 6% de órdenes con estatus nulo — fricción activa en pasarela de pagos CDMX
- Tulum representa solo el 1.78% de ventas totales — posible mercado
  no rentable o con problemas de operación

## Recomendaciones
1. Homologar criterios de captura de datos en toda la operación —
   los errores son sistemáticos y prevenibles desde el origen
2. Auditar técnicamente la pasarela de pagos en Ciudad de México
   para recuperar el 6% de órdenes con estatus nulo
3. Evaluar rentabilidad de Tulum: $54,394.73 vs. el resto de mercados
   indica desempeño anómalo que requiere investigación
4. Priorizar inventario y recursos comerciales en Ciudad de México
   y Monterrey como los dos mercados de mayor volumen

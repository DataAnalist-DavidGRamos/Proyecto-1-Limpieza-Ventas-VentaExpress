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
- Visibilidad recuperada: 15% de registros previamente fragmentados

## Hallazgos Principales

| Métrica | Resultado |
|---|---|
| Ventas totales Q4 2024 | $3,053,684.32 |
| Ticket promedio por transacción | $3,899.98 |
| Total de transacciones | 783 |
| Producto más vendido (cantidad) | Laptop Oficina 32GB — 116 piezas / $321,991.69 |
| Ciudad con mayor volumen de ventas | Ciudad de México — $556,084.37 |
| Ciudad con mayor participación porcentual | Bogotá — 38% del volumen |
| Mes con mejores resultados | Octubre |
| Precio promedio por categoría | $1,256,212.44 (promedio de 4 categorías) |

## Anomalías Detectadas
- 6% de órdenes con estatus nulo — fricción activa en pasarela de pagos CDMX
- Tulum representa solo el 1.72% de ventas totales — posible mercado no rentable

## Implicación y Recomendaciones
1. Auditar técnicamente la pasarela de pagos en Ciudad de México para
   recuperar el 6% de órdenes perdidas
2. Homologar los criterios de captura de datos en toda la operación —
   los errores actuales son sistemáticos y evitables
3. Evaluar rentabilidad de operaciones en Tulum dado su bajo volumen (1.72%)
4. Asignar mayor presupuesto de inventario a Ciudad de México y Bogotá
   como mercados líderes

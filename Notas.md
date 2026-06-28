# Notas del Analista — VentaExpress Q4 2024

## 1. Limpieza
- Sin duplicados: verificación realizada tomando como llave el ID de orden
- 19 datos vacíos en columnas "precio" y "monto" sustituidos con regla
  de tres; equivalen al 1.9% del total del dataset

## 2. Hallazgos principales
- Producto más vendido por cantidad: Laptop Oficina 32GB —
  116 piezas / $321,991.69
- Ciudad con mayor volumen de ventas: Ciudad de México — $556,084.37
- Monterrey muy cercana en segundo lugar: $548,597.88
- Tulum con el menor volumen: $54,394.73 (1.78% del total)
- Precio promedio por categoría: $1,256,212.44
  (promedio de 4 categorías de la columna "Especificaciones")

## 3. Metodología de limpieza
1. Observación inicial para identificar patrones de error
2. Separación y eliminación de caracteres especiales y errores comunes
3. Aplicación de fórmulas para depurar y normalizar el contenido
4. Construcción de tablas dinámicas para validar y extraer información

**Problemas encontrados en los datos originales:**
- Exceso de caracteres especiales, espacios en blanco, puntos y comas
  en campos numéricos
- Nombres personales capturados con abreviaciones de profesión —
  inconsistente con el propósito del campo

## 4. Limitaciones
- Conocimiento limitado en fórmulas avanzadas de limpieza rápida en Sheets;
  algunas correcciones se realizaron manualmente
- El dataset no incluye información de costo unitario, por lo que no fue
  posible calcular margen de utilidad por producto o ciudad
- Tulum tiene volumen muy bajo — muestra insuficiente para conclusiones
  estadísticas sólidas

## 5. Observaciones para futuros análisis
- Incorporar datos de costo para calcular margen real por ciudad y producto
- Investigar causa raíz del bajo desempeño de Tulum
- Establecer protocolo de captura estandarizado para evitar errores
  sistemáticos en futuros trimestres

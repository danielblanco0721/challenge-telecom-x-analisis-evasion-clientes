Análisis de Evasión de Clientes - TelecomX
📋 Descripción
Proyecto de análisis de datos para identificar los factores que influyen en la evasión de clientes (churn) de TelecomX. El objetivo es proporcionar insights accionables que permitan mejorar las estrategias de retención y reducir la tasa de fuga.
🎯 Objetivo
Analizar el comportamiento de 7,043 clientes para identificar patrones de fuga y desarrollar recomendaciones basadas en datos que reduzcan la tasa de churn actual del 26.5%.
📊 Datos
Fuente: API de TelecomX (formato JSON)
Registros: 7,043 clientes
Variables: 21 características (demográficas, servicios, cuenta, cargos)
Período: Datos históricos de clientes
🔧 Metodología
Extracción de datos: Carga desde API JSON usando pandas y requests
Limpieza y preprocessing:
Eliminación de valores nulos y duplicados
Conversión de tipos de datos
Creación de variables derivadas
Análisis exploratorio:
Estadísticas descriptivas
Distribución de variables categóricas y numéricas
Visualización de patrones de churn
Análisis de churn:
Segmentación por variables demográficas
Análisis por tipo de contrato y antigüedad
Identificación de factores de riesgo
💡 Hallazgos Principales
Tipo de contrato: Contratos mensuales tienen 42.7% de fuga vs 2.8% en contratos de 2 años
Antigüedad crítica: Primeros 12 meses son los más riesgosos
Adultos mayores: 41.7% de tasa de fuga (casi el doble del promedio)
Precio: Clientes que pagan más tienen mayor probabilidad de fuga
Facturación electrónica: Asociada con el doble de tasa de churn
🛠️ Tecnologías Utilizadas
Python 3.x
Pandas (manipulación de datos)
Matplotlib y Seaborn (visualización)
Requests (consumo de API)
Google Colab (entorno de desarrollo)
📁 Estructura del Proyecto
1234
├── notebook.ipynb              # Análisis completo en Google Colab
├── telecomx_limpio.csv         # Dataset procesado
├── telecomx_estandarizado.csv  # Dataset estandarizado
└── README.md                   # Documentación del proyecto
🚀 Cómo Ejecutar
Abrir el notebook en Google Colab
Ejecutar las celdas secuencialmente
Los datos se cargan automáticamente desde la API
📈 Recomendaciones Implementadas
Incentivar migración a contratos anuales (descuento 10-15%)
Programa de onboarding reforzado para primeros 90 días
Atención diferenciada para adultos mayores
Revisión de precios en planes >$80/mes
Meta: Reducir churn al 18% en 6 meses
📊 Resultados Esperados
Reducción de churn del 26.5% al 18%
Conversión del 25% de contratos mensuales a anuales
Mejora en satisfacción de clientes nuevos (>85%)


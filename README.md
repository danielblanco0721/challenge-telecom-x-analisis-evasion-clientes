# Análisis de Evasión de Clientes - TelecomX

## 📋 Descripción

Proyecto de análisis de datos para identificar los factores que influyen en la evasión de clientes (churn) de TelecomX. El objetivo es proporcionar insights accionables que permitan mejorar las estrategias de retención y reducir la tasa de fuga.

## 🎯 Objetivo

Analizar el comportamiento de **7,043 clientes** para identificar patrones de fuga y desarrollar recomendaciones basadas en datos que reduzcan la tasa de churn actual del **26.5%**.

## 📊 Datos

| Característica | Detalle |
|----------------|---------|
| **Fuente** | API de TelecomX (formato JSON) |
| **Registros** | 7,043 clientes |
| **Variables** | 21 características |
| **Categorías** | Demográficas, servicios, cuenta, cargos |

## 🔧 Metodología

### 1. Extracción de Datos
Carga desde API JSON usando pandas y requests.

### 2. Limpieza y Preprocessing
- Eliminación de valores nulos y duplicados
- Conversión de tipos de datos
- Creación de variables derivadas (Cuentas_Diarias)

### 3. Análisis Exploratorio
- Estadísticas descriptivas (media, mediana, desviación estándar)
- Distribución de variables categóricas y numéricas
- Visualización de patrones de churn

### 4. Análisis de Churn
- Segmentación por variables demográficas
- Análisis por tipo de contrato y antigüedad
- Identificación de factores de riesgo

## 💡 Hallazgos Principales

### Factores Críticos de Fuga

| Factor | Tasa de Fuga | Impacto |
|--------|--------------|---------|
| **Contrato Month-to-Month** | 42.7% | 🔴 Muy Alto |
| **Adultos Mayores** | 41.7% | 🔴 Alto |
| **Facturación Electrónica** | 33.6% | 🟡 Medio |
| **Sin Pareja** | 33.0% | 🟡 Medio |
| **Contrato 2 Años** | 2.8% | ✅ Bajo |

### Insights Clave

1. **Tipo de Contrato**: Los contratos mensuales tienen **15 veces más** fuga que los contratos de 2 años
2. **Antigüedad Crítica**: Los primeros **12 meses** son los más riesgosos (clientes que se van promedian 18 meses vs 37.6 meses de quienes permanecen)
3. **Paradoja del Precio**: Clientes que pagan más tienen mayor probabilidad de fuga ($74.44 vs $61.27)
4. **Segmento Senior**: Adultos mayores presentan casi el doble de tasa de fuga

## 🛠️ Tecnologías Utilizadas

- **Python 3.x**
- **Pandas** - Manipulación y análisis de datos
- **Matplotlib & Seaborn** - Visualización de datos
- **Requests** - Consumo de API
- **Google Colab** - Entorno de desarrollo

## 📁 Estructura del Proyecto
telecomx-churn-analysis/
│
├── challenge-telecom-x-analisis-evasion-clientes.ipynb # Análisis completo en Google Colab
└── README.md # Documentación del proyecto

# ConnectaTel – Análisis de Comportamiento de Clientes

Análisis de datos de una empresa de telecomunicaciones con operaciones en México y Colombia, 
realizado como Proyecto 6 del bootcamp de Data Analytics de TripleTen.

## 🎯 Objetivo del proyecto

Explorar, limpiar y analizar el comportamiento de uso de los clientes de ConnectaTel 
para identificar patrones de consumo, detectar comportamientos atípicos y crear segmentos 
de clientes que permitan optimizar la oferta comercial y mejorar la experiencia del usuario.

## 📂 Datasets utilizados

| Archivo | Descripción |
|---|---|
| `plans.csv` | Planes disponibles (precio, minutos, GB, costos extra) |
| `users_latam.csv` | Información de clientes (edad, ciudad, plan, fecha de registro, churn) |
| `usage.csv` | Detalle de uso real (llamadas y mensajes por usuario) |

## 🔄 Etapas del análisis

1. **Carga y exploración** — revisión de estructura, tipos y tamaño de cada dataset
2. **Identificación de problemas de calidad** — nulos, sentinels, fechas fuera de rango
3. **Limpieza** — reemplazo de sentinels, estandarización de fechas, verificación MAR
4. **Summary statistics** — agrupación de uso por usuario y merge con perfil de cliente
5. **Visualización y outliers** — histogramas, boxplots e IQR para detectar valores extremos
6. **Segmentación** — clasificación por nivel de uso y grupo de edad
7. **Insight ejecutivo** — conclusiones y recomendaciones para el negocio

## ▶️ Cómo ejecutar el notebook

1. Abre el archivo `.ipynb` en GitHub
2. Haz clic en **Open in Colab**
3. Ejecuta las celdas en orden — los datasets se cargan desde `/datasets/`

## 🧠 Principales hallazgos

- El 74% de los clientes tiene **uso medio** del servicio
- El 7% es **Alto uso** — segmento de alto valor con consumo intensivo
- El 19% es **Bajo uso** — riesgo de churn, requiere activación proactiva
- Los **Adultos (30-59 años)** representan el 50% de la base de clientes
- `cant_minutos_llamada` presenta outliers reales (usuarios con >60 min) — candidatos a plan de voz ilimitada

## 👤 Autor

Sebastian Márquez — [github.com/Smarquez94](https://github.com/Smarquez94)

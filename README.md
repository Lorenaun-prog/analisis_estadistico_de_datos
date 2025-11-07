# analisis_estadistico_de_datos
Proyecto de análisis estadístico de datos del operador de telecomunicaciones Megaline.

# 📊 Análisis de Tarifas de Megaline

# 🧠 Descripción del Proyecto

El operador de telecomunicaciones Megaline ofrece a sus clientes dos tarifas de prepago: Surf y Ultimate.
El departamento comercial desea conocer cuál de los planes genera más ingresos, con el objetivo de optimizar su presupuesto publicitario.

Como analista de datos, mi tarea es realizar un análisis preliminar del comportamiento de los clientes utilizando los datos de una muestra de 500 usuarios.
El análisis incluirá el estudio de los hábitos de consumo de llamadas, mensajes y datos, así como la comparación del ingreso promedio generado por cada tarifa mediante pruebas estadísticas.

# 🎯 Objetivos del Proyecto

Analizar el comportamiento de los usuarios de ambas tarifas (Surf y Ultimate).

Calcular los ingresos mensuales por usuario según su uso y plan contratado.

Determinar cuál tarifa genera mayores ingresos promedio.

Comprobar si existen diferencias significativas entre:

Los ingresos medios de los usuarios de cada tarifa.

Los ingresos medios de los usuarios del área de Nueva York–Nueva Jersey frente a los de otras regiones.

# 🗂️ Descripción de los Datos

El proyecto utiliza cinco conjuntos de datos:

1. users — Información de los clientes
Columna	Descripción
user_id	Identificador único del usuario
first_name	Nombre
last_name	Apellido
age	Edad (años)
reg_date	Fecha de suscripción
churn_date	Fecha de cancelación del servicio (NaN si sigue activo)
city	Ciudad
plan	Nombre del plan contratado
2. calls — Llamadas realizadas
Columna	Descripción
id	Identificador de la llamada
call_date	Fecha de la llamada
duration	Duración (en minutos)
user_id	Identificador del usuario
3. messages — Mensajes SMS enviados
Columna	Descripción
id	Identificador del mensaje
message_date	Fecha del SMS
user_id	Identificador del usuario
4. internet — Sesiones de navegación
Columna	Descripción
id	Identificador de la sesión
mb_used	Datos usados (MB)
session_date	Fecha de la sesión
user_id	Identificador del usuario
5. plans — Información sobre los planes tarifarios
Columna	Descripción
plan_name	Nombre del plan
usd_monthly_fee	Cuota mensual (USD)
minutes_included	Minutos incluidos
messages_included	SMS incluidos
mb_per_month_included	Datos incluidos (MB)
usd_per_minute	Costo por minuto adicional
usd_per_message	Costo por SMS adicional
usd_per_gb	Costo por GB adicional
💡 Descripción de las Tarifas
Surf

Cuota mensual: $20

Incluye: 500 minutos, 50 SMS, 15 GB de datos

Excedentes:

Minuto adicional: $0.03

SMS adicional: $0.03

GB adicional: $10

Ultimate

Cuota mensual: $70

Incluye: 3000 minutos, 1000 SMS, 30 GB de datos

Excedentes:

Minuto adicional: $0.01

SMS adicional: $0.01

GB adicional: $7

⚙️ Nota: Megaline redondea las llamadas por minuto (cada llamada se redondea hacia arriba) y los datos mensuales por gigabyte (el total mensual se redondea hacia arriba).

# 🧹 Etapas del Proyecto

1️⃣ Preparación de los Datos

Importación de los archivos .csv.

Conversión de tipos de datos y corrección de valores erróneos o ausentes.

Cálculo de:

Número de llamadas, SMS y volumen de datos por usuario y mes.

Ingresos mensuales por usuario según plan y consumo.

2️⃣ Análisis Exploratorio

Análisis descriptivo de minutos, SMS y datos por tarifa.

Cálculo de media, varianza y desviación estándar.

Visualización mediante histogramas y comparaciones entre tarifas.

3️⃣ Pruebas Estadísticas

Hipótesis 1: Los ingresos promedio de los usuarios de las tarifas Surf y Ultimate difieren.

Hipótesis 2: Los ingresos promedio de los usuarios del área Nueva York–Nueva Jersey difieren de los de otras regiones.

Se establecen hipótesis nula y alternativa, se define un nivel de significación (α), y se aplica una prueba estadística adecuada (por ejemplo, t-test para muestras independientes).

4️⃣ Conclusión General

Resumen de los principales hallazgos.

Recomendaciones sobre la estrategia comercial o de marketing.

# 📈 Tecnologías Utilizadas

Python

pandas

numpy

matplotlib / seaborn

scipy.stats

Jupyter Notebook

# 🧾 Resultados Esperados

Identificación del plan con mayores ingresos promedio.

Insights sobre el comportamiento de los usuarios según su consumo de minutos, mensajes y datos.

Conclusiones estadísticas que respalden las decisiones del departamento comercial.

# ✍️ Autor

Lorena Urquijo N.
Analista de Datos — Megaline Project
📅 Año: 2025

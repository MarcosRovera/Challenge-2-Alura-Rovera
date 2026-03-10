# Challenge-2-Alura-Rovera
### Propósito del análisis

El objetivo de este proyecto es analizar los factores que influyen en la cancelación de clientes (Churn) en Telecom X. El análisis busca identificar patrones, comportamientos y posibles estrategias de retención, proporcionando información estratégica para reducir la tasa de cancelación y fidelizar clientes.

### Limpieza y Tratamiento de Datos

*Para garantizar la calidad del análisis se realizaron los siguientes pasos:*

-Carga y normalización del JSON: Se transformaron los datos anidados del archivo original (customer, phone, internet, account) a un DataFrame plano.

*Valores faltantes:*

-Charges.Total con valores nulos se reemplazaron con la mediana.

-La variable Churn contenía valores desconocidos, se clasificaron como Desconocido para mantener la visibilidad en los análisis.

*Estandarización:*

-Variables binarias convertidas a formato uniforme (Sí/No).

-Se crearon indicadores adicionales, como Cuentas_Diarias, a partir de la facturación mensual.

#### Con estos pasos, el dataset quedó listo para el Análisis Exploratorio de Datos (EDA).

### Ejemplos de análisis realizados

**Durante el análisis se exploraron diferentes aspectos de los datos:**

**Distribución general de Churn: Se evaluó la proporción de clientes que cancelaron, permanecieron y aquellos con estado desconocido.**

*Churn según variables categóricas:*

-Tipo de contrato: Month-to-month muestra la mayor tasa de cancelación; contratos a largo plazo reducen el riesgo.

-Método de pago: clientes con Electronic Check presentan mayor tendencia a cancelar.

-Género: no se observan diferencias relevantes.

*Churn según variables numéricas:*

-Tiempo de contrato (tenure): menor tiempo se asocia a mayor churn.

-Gasto mensual y total (Charges.Monthly, Charges.Total): clientes con menor gasto tienden a cancelar, aunque algunos con gasto elevado también abandonan.

-Servicios adicionales (OnlineSecurity, TechSupport, DeviceProtection): parecen reducir la probabilidad de cancelación.

### Insights obtenidos

Algunos hallazgos clave del análisis:

*Mayor riesgo de churn:*

  -Contratos mes a mes (Month-to-month).
  
  -Clientes con poco tiempo de permanencia.

-Uso de Electronic Check como método de pago.

*Factores que reducen churn:*

-Contratos a largo plazo (1 o 2 años).

-Contratación de servicios adicionales.

-Clientes con mayor gasto total mensual o anual.

*Variables poco influyentes:*

-Género del cliente.

-Algunos servicios básicos universales, como Phone Service.

### Recomendaciones estratégicas

-Fidelización temprana: campañas de retención durante los primeros 3–6 meses.

-Incentivos para contratos largos: descuentos o beneficios exclusivos para contratos de 1 o 2 años.

-Optimización de métodos de pago: promover pagos automáticos que muestran menor churn.

-Cross-selling de servicios adicionales: ofrecer servicios de seguridad, soporte y protección de dispositivos a clientes nuevos o en riesgo.

-Segmentación de campañas: enfocar esfuerzos en clientes con menor tiempo de permanencia y menor gasto total.

Cómo ejecutar el proyecto?

-Clonar este repositorio: 'https://github.com/MarcosRovera/Challenge-2-Alura-Rovera.git'

-Ejecutar el archivo: Challenge_2_Rovera.ipynb

### Tecnologías utilizadas

-Python

-Pandas

-Matplotlib

-Seaborn

-Jupyter Notebook

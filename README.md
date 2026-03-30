Análisis del Mercado Airbnb - CABA Argentina
Este proyecto presenta un análisis estratégico del mercado de alquileres temporarios en la Ciudad Autónoma de Buenos Aires, combinando ingeniería de datos con Python y visualización interactiva en Power BI.

Insights de Negocio
Efecto Elite: Se identificó que las propiedades con más de 20 reseñas (14% del mercado) logran un posicionamiento orgánico dominante.
Drivers de Precio: La capacidad de huéspedes (accommodates) impacta significativamente más en el precio final que la cantidad de dormitorios.
Zonas de Oportunidad: Barrios como San Nicolás y Monserrat presentan un ROI potencial más alto debido a sus bajos costos de entrada y alta rotación.
Océano Azul: Existe una brecha de profesionalización, ya que el 60% de los hosts presentan un nivel de interacción bajo.

Documentación Técnica (Proceso de Datos)
Lenguaje: Python 3.12 
Librerías: Pandas, Numpy, Seaborn, Matplotlib 
Visualización: Power BI Desktop / Service 

1. ETL y Limpieza de Datos (limpieza_datos.ipynb)
Tratamiento de Nulos: Se eliminaron variables con más del 60% de datos faltantes para garantizar la integridad del modelo.
Imputación Estratégica: En la métrica de reseñas, se optó por la imputación de ceros en lugar de descartar registros, permitiendo segmentar anfitriones nuevos de experimentados.
Ingeniería de Features: Creación de rangos cualitativos ("Nivel de Interacción") y cálculo de años activos por propiedad.

2. Análisis Exploratorio y Estadístico (analisis_datos.ipynb)
Gestión de Outliers: Se aplicaron filtros basados en percentiles (IQR) para tratar valores extremos en los precios, asegurando que los promedios del dashboard sean representativos.
Validación Estadística: Uso de la Matriz de Correlación de Pearson para validar las variables que más impactan en el precio.
Análisis de Cuadrantes: Clasificación de barrios por Precio vs. Popularidad para detectar zonas eficientes.

3. Visualización (Airbnb_Dashboard.pbix)
El dashboard se estructuró en dos pilares:
Análisis Geográfico: Concentración de oferta y volumen total de mercado.
Matriz de Rentabilidad: Mapa de calor cruzando huéspedes vs. dormitorios para identificar el "punto dulce" de inversión.

Video Demostrativo: https://drive.google.com/file/d/12kHrEWvpsk8PHmsEOd6j8n3F6FoCgjsD/view?usp=drive_link

# Proyecto: Análisis de Logs HTTP en Tiempo Real para Seguridad y Marketing realizado en el CEIABD (con mejoras a futuro)

![Portada](img/cover.jpg)

## 🎯 Objetivo:

Construcción de un sistema Big Data completo para el análisis en tiempo real de logs HTTP, permitiendo detectar amenazas de seguridad, analizar el tráfico web, y extraer conocimiento útil para decisiones de marketing.

## 🧱 Stack Tecnológico Implementado

![Stack](img/ESQUEMA.png)

| Área             | Herramientas                                                |
| ---------------- | ----------------------------------------------------------- |
| Ingesta de datos | Python + Faker (logs sintéticos), Apache Kafka              |
| Procesamiento    | Spark Streaming (API DataFrame), UDFs para geolocalización  |
| Almacenamiento   | HDFS (Parquet), PostgreSQL                                  |
| Visualización    | Power BI (DirectQuery), Grafana + Prometheus                |
| Orquestación     | Hadoop (HDFS, YARN, MapReduce), Kafka con múltiples brokers |


## 🧠 Inteligencia de Negocio Obtenida

- Detección de IPs sospechosas por volumen de tráfico o errores 4xx/5xx.

- Análisis de geolocalización de posibles amenazas.

- Identificación de bots por user-agent.

- Trazado del tráfico por hora, país y URI.

- Métricas por país con mayores tasas de error.

- Análisis de tamaño de respuesta y referers sospechosos.

## 📈 Visualizaciones creadas

- Dashboards de Power BI con DirectQuery sobre PostgreSQL así como Dashboards con HDFS (ficheros parquet), posibilitando saber la diferencia entre un sistema de BD distribuidas cotidiano a un sistema o arquitectura a tiempo real / streaming.

- Paneles de Grafana para monitoreo de Spark y Kafka con Prometheus.

- Mapas de calor, histogramas de errores por hora, tráfico por país, y más.

## 🚀 Características Técnicas Utilizadas e Implementadas

- ETL semi avanzado con Spark Streaming en tiempo real.

- Uso de funciones UDF en PySpark para enriquecimiento de datos ( realización y obtención de la geolocalización).

- Monitorización avanzada de clústeres con Prometheus.

- Conexión directa HDFS/Parquet y PostgreSQL desde Power BI.

- Capacidad de análisis forense de logs a partir de estructura temporal y espacial.

## 🧪 Investigación Propia Desarrollada

- Integración de Prometheus con Spark 3.5+ sin plugins externos.

- Conector personalizado ODBC para Power BI en modo DirectQuery con PostgreSQL.

- Cálculo de métricas personalizadas en DAX para Power BI.

## Contenido para Añadir o Mejorar el Proyecto a Futuro.

- Implementación de Stack ELK para el procesamiento (Logstach), ElasticSearch (Almacenamiento) y Kibana (Visualización).







# Proyecto de Pruebas de Carga con JMeter

## Descripción General
Este repositorio contiene una colección de planes de prueba, scripts y configuraciones de JMeter para simular escenarios de prueba de carga en aplicaciones web y APIs. El objetivo es evaluar el rendimiento bajo diferentes niveles de carga e identificar posibles cuellos de botella.

---

## Características
- **Simulación de Carga Gradual**: Grupos de hilos configurables para aumentar gradualmente la carga de usuarios.
- **Monitoreo de Errores**: Captura respuestas detalladas de errores para su análisis.
- **Métricas de Rendimiento**: Recopila indicadores clave como tiempos de respuesta, throughput y tasas de éxito.
- **Aserciones Personalizadas**: Validaciones para asegurar que las respuestas de las API cumplan con los criterios esperados.
- **Generación de Reportes**: Produce reportes HTML con detalles sobre el rendimiento.

---

## Estructura del Repositorio
```
.
|-- test-plans/          # Archivos de planes de prueba de JMeter (.jmx)
|-- csv-data/            # Archivos de datos para pruebas parametrizadas
|-- reports/             # Reportes HTML generados
|-- README.md            # Documentación del proyecto
```

---

## Requisitos Previos
1. **JMeter**: Instalar Apache JMeter ([Descargar aquí](https://jmeter.apache.org/)).
2. **Java**: Asegúrate de tener Java 8 o superior instalado.
   ```bash
   java -version
   ```
3. **Plugins Manager**: Instalar [JMeter Plugins](https://jmeter-plugins.org/) para funcionalidades extendidas.

---

## Instalación
1. Clona el repositorio:
   ```bash
   git clone https://github.com/<tu-usuario>/<nombre-repositorio>.git
   ```
2. Navega al directorio del proyecto:
   ```bash
   cd <nombre-repositorio>
   ```

---

## Uso

### Ejecución de Pruebas
1. Abre JMeter.
2. Carga un plan de prueba desde el directorio `test-plans/`.
3. Ajusta los parámetros del grupo de hilos si es necesario (por ejemplo, número de hilos, tiempo de escalado).
4. Ejecuta la prueba.

### Generación de Reportes
Después de ejecutar una prueba:
1. Guarda los resultados como un archivo `.jtl` o `.csv`.
2. Usa el siguiente comando para generar un reporte HTML:
   ```bash
   jmeter -g <ruta-del-archivo-de-resultados> -o <ruta-del-directorio-de-salida>
   ```

---

## Escenarios de Prueba Clave
- **Prueba de Carga Básica**: Evalúa el rendimiento de la aplicación bajo carga normal.
- **Prueba de Estrés**: Lleva el sistema al límite para identificar puntos de quiebre.
- **Prueba de Resistencia**: Evalúa el rendimiento durante un periodo prolongado.
- **Prueba de Picos**: Simula aumentos repentinos en el tráfico.

---

## Ejemplo de Reporte
Los reportes HTML generados proporcionan detalles como:
- Tiempo promedio de respuesta.
- Throughput y errores.
- Gráficas detalladas de tiempos de respuesta y throughput a lo largo del tiempo.

---







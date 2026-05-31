# 📊 Portafolio de Análisis de Datos con Power BI

¡Hola! Bienvenido/a a mi repositorio de proyectos de Business Intelligence. Este es un espacio donde se muestran unas prácticas básicas de Power BI realizadas durante un curso de **Santander Academy**.

El objetivo de este repositorio es consolidar y aplicar los conocimientos teóricos y prácticos adquiridos en el curso sobre análisis, tratamiento y visualización de datos utilizando **Power BI Desktop**, **Power Query** y fundamentos de modelado relacional.

## 🚀 Competencias Técnicas Demostradas

A través de las prácticas documentadas en este repositorio, demuestro mi capacidad para transformar datos crudos en información útil para el análisis de negocio. Mis habilidades principales incluyen:

### 1. Extracción y Transformación de Datos (Power Query)
El motor de preparación de datos antes de su análisis:
* **Conexión a múltiples orígenes:** Importación estructurada desde archivos `.xlsx`, `.csv` y `.txt`.
* **Limpieza y transformación de columnas:** División de columnas (ej. separar texto de números), extracción de caracteres, estandarización de mayúsculas/minúsculas y adición de prefijos/sufijos.
* **Control del Lenguaje M:** Manejo del panel de pasos aplicados, asegurando la trazabilidad en la limpieza de datos y la correcta asignación de tipos de datos a cada columna.

### 2. Modelado y Formato de Datos
Preparación del modelo relacional para asegurar cálculos precisos y legibilidad:
* **Formatos personalizados:** Aplicación de máscaras de formato a medida (ej. `#,#0 "horas"`, formatos de moneda y fechas estructuradas).
* **Manejo de funciones de agregación:** Uso de Suma, Promedio, Recuento y Recuento Distintivo para la base de las visualizaciones.

### 3. Visualización de Datos y Dashboards (UI/UX)
Creación de la interfaz interactiva de los datos:
* **Construcción de Informes:** Uso estratégico de Tablas, Matrices, Tarjetas para KPIs, Gráficos de barras/columnas apiladas y Gráficos circulares/de anillos.
* **Interactividad:** Configuración del filtrado cruzado entre objetos visuales, permitiendo que la selección de un dato segmente dinámicamente todo el lienzo.
* **Segmentación de datos:** Implementación de *slicers* (segmentadores) para controlar filtros a nivel de página o de forma global.

### 4. Análisis Avanzado (Filtros y Formato Condicional)
Técnicas para resaltar información clave de un vistazo:
* **Filtros de panel:** Aplicación de filtros básicos, filtros por medidas totalizadas y filtros `Top N` para rankear los mejores o peores resultados.
* **Formato Condicional:** Implementación de barras de datos, escalas de color de fondo y conjuntos de iconos basados en reglas para alertar sobre el cumplimiento de objetivos.

---

## 📂 Estructura del Repositorio

El repositorio se encuentra organizado de manera limpia y estructurada bajo el siguiente esquema de directorios:

* 📁 **`data/`** *(Archivos Base y Datos Crudos)*
  * `01 - BD CURSOS.xlsx`
  * `02 - BD CURSOS.xlsx`
  * `03- BD CURSOS.xlsx`
  * `06 - BD FACTURAS.xlsx`
  * `08 - BD PERSONAS.xlsx`
* 📁 **`dashboards/`** *(Proyectos de Power BI Desktop)*
  * `BD CURSOS.pbix`
  * `BD FACTURAS.pbix`
  * `BD PERSONAS.pbix`

---

## 🛠️ Cómo explorar este trabajo

Para facilitar la revisión y auditoría de mis proyectos, puedes explorar el trabajo de las siguientes maneras según tus objetivos:

### 1. Guía de Ejecución Rápida
Si deseas probar los paneles de forma local en tu equipo, sigue estos pasos:
1. Clona este repositorio:
```bash
   git clone [https://github.com/alexhb-maker/](https://github.com/alexhb-maker/)Powerbi-Santander-Course.git
```
Dirígete a la carpeta /dashboards y abre cualquiera de los archivos .pbix con Power BI Desktop.

Nota de orígenes de datos: Si Power BI solicita actualizar las rutas de los archivos de Excel, ve a Inicio > Transformar datos > Configuración de origen de datos y apunta a la carpeta /data de tu directorio local.

2. Qué analizar en cada Proyecto (.pbix)
Al abrir los archivos en Power BI Desktop, te sugiero prestar atención a los siguientes apartados técnicos desarrollados en cada práctica:

📈 Proyecto 1: Análisis de Formación (BD CURSOS.pbix)
Enfoque: Control de rentabilidad, ingresos por comercial y eficiencia de las jornadas formativas.

Qué auditar en Power Query: Observa el proceso de consolidación y limpieza de las fuentes repetidas (01, 02 y 03 - BD CURSOS.xlsx). Verás la asignación estricta de tipos de datos y la extracción de textos limpios para los nombres de los cursos.

En el Lienzo: Interactúa con los segmentadores para filtrar por comercial o profesor y observa cómo el filtrado cruzado recalcula instantáneamente los importes totales del cliente frente a los costes del profesor.

🧾 Proyecto 2: Gestión Contable (BD FACTURAS.pbix)
Enfoque: Análisis financiero, dispersión geográfica y control de morosidad.

Qué auditar en el Lienzo: Explora la matriz avanzada y los gráficos de barras apiladas orientados a analizar el volumen de facturación por provincias, sectores empresariales y zonas.

Análisis Avanzado: He aplicado Filtros Top N para destacar los clientes con mayor volumen de facturación y Formato Condicional mediante reglas de color para identificar visualmente aquellas facturas que aún están pendientes de cobro (PAGADA CLIENTE = "NO").

👥 Proyecto 3: Registro de Clientes (BD PERSONAS.pbix)
Enfoque: Gestión de perfiles y análisis de crecimiento de la cartera de clientes.

Qué auditar en Power Query: Verás técnicas de transformación avanzadas, como la división de columnas para estructurar nombres y apellidos por separado, y la limpieza de códigos de cliente (NIF/IDs).

Formatos y Modelado: Se aplicaron formatos personalizados y máscaras de visualización para que las fechas de incorporación y los campos clave sean limpios y legibles para el usuario final.

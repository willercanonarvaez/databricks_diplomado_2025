# Análisis de Datos Gubernamentales de Colombia

Este proyecto tiene como objetivo la recolección, limpieza y análisis de datos provenientes de dos fuentes oficiales del gobierno colombiano: el SECOP Integrado y el Ministerio de Educación Nacional. Una vez procesados, los datos serán cargados a **Databricks** para su exploración, modelamiento y visualización.

## 📂 Fuentes de Datos

1. **SECOP Integrado (Contratación Pública)**  
   - URL: [https://www.datos.gov.co/resource/rpmr-utcd.csv](https://www.datos.gov.co/resource/rpmr-utcd.csv)  
   - Descripción: Contiene información detallada sobre contratos del Estado, incluyendo entidad contratante, valor, objeto, modalidad, proveedor, entre otros.

2. **Ministerio de Educación Nacional (Cobertura y Desempeño Educativo)**  
   - URL: [https://www.datos.gov.co/resource/nudc-7mev.csv](https://www.datos.gov.co/resource/nudc-7mev.csv)  
   - Descripción: Incluye indicadores educativos como tasa de matrícula, cobertura neta y bruta, deserción y aprobación por municipio y año.

## ⚙️ Proceso del Proyecto

1. **Extracción**  
   Los datos se descargan directamente desde las APIs públicas en formato `.csv`.

2. **Transformación y Limpieza**  
   Se aplican transformaciones para:
   - Homogeneizar nombres de columnas
   - Convertir tipos de datos
   - Eliminar registros duplicados o inconsistentes
   - Normalizar nombres de municipios y departamentos

3. **Carga a Databricks**  
   Los datasets procesados se cargan como tablas en **Databricks** para su análisis posterior mediante SQL, PySpark o notebooks.

## 🚀 Objetivos

- Explorar y analizar la eficiencia del gasto público en educación.
- Cruzar información entre contratación estatal y desempeño educativo.
- Generar visualizaciones y dashboards interactivos en Databricks.
- Proponer insights para la toma de decisiones basadas en datos abiertos.

## 🛠️ Tecnologías Utilizadas

- Python (pandas, requests)
- Databricks Notebooks
- SQL / PySpark
- APIs abiertas del gobierno de Colombia

## 📌 Notas

- Este proyecto hace uso exclusivo de datos públicos y no contiene información sensible.
- Los scripts de ETL pueden ser ejecutados localmente o directamente en entornos de desarrollo como Databricks.

## 📫 Contacto

Si tienes preguntas o sugerencias, no dudes en abrir un issue o contactarme.

## 🗂️ Organización del Repositorio

- `notebooks/` — notebooks de desarrollo y transformación de datos
  - `secop_etl.ipynb` — procesamiento de datos de contratación pública
  - `educacion_etl.ipynb` — procesamiento de datos educativos
- `data/` — carpeta para almacenar temporalmente los archivos descargados
  - `secop_integrado.csv`
  - `educacion_men.csv`
- `README.md` — documentación del proyecto
- `requirements.txt` — dependencias necesarias para ejecutar el proyecto


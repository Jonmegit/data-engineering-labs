# Data Engineering Labs

Este repositorio contiene pequeños ejemplos de ingeniería de datos con un enfoque en tuberías **ETL (extract, transform, load)**.

## ¿Qué es ETL?

ETL es un tipo de tubería de datos utilizada para recopilar datos de diversas fuentes, transformarlos según las reglas de negocio y cargarlos en un almacén de destino【229434291992404†L293-L305】. La transformación se realiza en un motor especializado y suele implicar operaciones como filtrado, ordenación, agregación, unión, limpieza, deduplicación y validación【229434291992404†L302-L304】.

En un flujo ETL típico, las fases pueden ejecutarse en paralelo para ganar eficiencia; por ejemplo, mientras se extraen datos de una fuente, los datos ya extraídos pueden ir transformándose y cargándose【229434291992404†L306-L309】.

## Diferencia entre ETL y ELT

Aunque ETL y ELT comparten el mismo objetivo, la diferencia radica en dónde se ejecuta la transformación. En ELT, la transformación se ejecuta directamente en el almacén de destino en lugar de un motor aparte, lo que simplifica la arquitectura【229434291992404†L320-L328】.

## Estructura

- `notebooks/` – ejemplos de notebooks que implementan tuberías sencillas.
- `data/` – datasets de muestra o datos generados.
- `src/` – scripts de Python reutilizables.

## Uso

1. Crea un entorno virtual y actívalo.
2. Instala dependencias:
   ```bash
   pip install pandas pyarrow
   ```
3. Ejecuta el notebook `notebooks/etl_basic_example.ipynb` para ver un flujo ETL con Pandas.

## Fuentes

- La descripción del proceso ETL proviene de la guía de arquitectura de Azure【229434291992404†L293-L305】 y las operaciones típicas se resumen a partir de la misma fuente【229434291992404†L302-L304】.

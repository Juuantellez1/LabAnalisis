# Laboratorio 03 — Análisis de Ventas y Reglas de Asociación

**Estudiante:** Juan Sebastián Téllez  
**Asignatura:** Analítica de Datos  
**Universidad:** Pontificia Universidad Javeriana  
**Año:** 2026

## Descripción

En este laboratorio trabajé con información de ventas de una tienda para conocer cuáles son los productos más comprados y analizar las relaciones que pueden existir entre ellos.

Para realizar el análisis utilicé Python y dos algoritmos de reglas de asociación: Apriori y FP-Growth. La idea fue comparar sus resultados y tiempos de ejecución, además de explorar posibles combinaciones de productos que podrían ser útiles para una tienda.

## Objetivos

- Analizar las ventas y el comportamiento de compra de los clientes.
- Identificar los productos más y menos vendidos.
- Explorar posibles relaciones entre los productos comprados.
- Comparar el rendimiento de Apriori y FP-Growth.
- Evaluar cómo influyen el soporte y la confianza en los resultados.

## Herramientas utilizadas

- Python
- Visual Studio Code
- Jupyter Notebook
- Pandas y NumPy
- Matplotlib y Seaborn
- MLxtend
- DBFRead

## Desarrollo del laboratorio

Se analizaron **147.413 registros de ventas** provenientes de archivos DBF.

Primero organicé los datos y realicé un análisis descriptivo para identificar los productos más vendidos, sus cantidades y el comportamiento de las ventas por fecha.

Después preparé las transacciones para ejecutar Apriori y FP-Growth. Realicé 20 pruebas con diferentes parámetros para cada algoritmo, obteniendo 40 ejecuciones en total.

Finalmente, comparé los tiempos de ejecución y analicé los resultados para responder las preguntas planteadas en el taller.

## Resultados principales

Entre los productos más vendidos encontré:

| Producto | Unidades vendidas |
|---|---:|
| Empanadas | 21.099 |
| Desechable x unidad | 8.543 |
| Cerveza Club Colombia 330 ml | 8.180 |
| Pasteles y palitos | 8.109 |
| Jugo Hit 500 ml | 7.997 |

En las pruebas realizadas, Apriori presentó menores tiempos de ejecución que FP-Growth para los parámetros utilizados.

Con las configuraciones evaluadas no se obtuvieron reglas de asociación, lo que permitió observar la importancia de elegir adecuadamente los valores de soporte y confianza.

## Cómo ejecutar el proyecto

1. Descargar o clonar el repositorio.
2. Abrir la carpeta del laboratorio en Visual Studio Code.
3. Crear un entorno virtual de Python.
4. Instalar las bibliotecas de `requirements.txt`.
5. Abrir `Lab03_Reglas_Asociacion.ipynb`.
6. Seleccionar el kernel de Python y ejecutar las celdas en orden.

Los archivos generados se encuentran en la carpeta `resultados`.

## Conclusiones

Este laboratorio me permitió entender cómo se pueden utilizar los datos de ventas para conocer mejor el comportamiento de los clientes.

También aprendí que dos algoritmos diseñados para resolver el mismo problema pueden tener tiempos de ejecución diferentes, y que los parámetros seleccionados influyen directamente en los resultados.

Una de las principales conclusiones fue que encontrar productos muy vendidos no significa necesariamente que existan asociaciones fuertes entre ellos. Para identificar relaciones útiles es importante considerar tanto la frecuencia de compra como las características de las transacciones.

---

**Juan Sebastián Téllez — Analítica de Datos, 2026**

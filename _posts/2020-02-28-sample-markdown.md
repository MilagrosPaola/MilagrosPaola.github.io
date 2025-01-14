---
layout: post
title: Consejos útiles para aprender Markdown
subtitle: There's lots to learn!
gh-repo: 
gh-badge: [star, fork, follow]
tags: [learn]
comments: true
mathjax: true
author: Milagros Paola
---

{: .box-success}
Power BI es una poderosa herramienta de visualización de datos que te permite transformar datos crudos en información comprensible a través de informes interactivos y dashboards. Si estás empezando con Power BI, aquí tienes algunos consejos que te ayudarán a dominarlo más rápidamente.

**Comienza con lo básico**

En Power BI, es crucial entender cómo importar datos desde diversas fuentes y crear gráficos sencillos. Familiarízate con las secciones principales como el panel de campos, visualizaciones y filtros.

## 1. Modelado de datos
Asegúrate de comprender cómo conectar diferentes tablas mediante relaciones y cómo usar **columnas calculadas** y **medidas** con DAX (Data Analysis Expressions).

[Este es un enlace a la documentación de DAX](https://learn.microsoft.com/en-us/dax/).

### Tabla de funciones básicas de DAX

| Función | Descripción |
| :------ | :---------- |
| `CALCULATE()` | Modifica el contexto de evaluación de una medida. |
| `SUM()` | Suma de un conjunto de valores. |
| `IF()` | Condicional, permite crear cálculos basados en una condición. |

You can use [MathJax](https://www.mathjax.org/) to write LaTeX expressions. For example:
Cuando \\(a \ne 0\\), hay dos soluciones para \\(ax^2 + bx + c = 0\\) y son $$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$

### Creando visualizaciones efectivas

Uno de los aspectos más interesantes de Power BI es la capacidad de crear visualizaciones interactivas. Usa gráficos adecuados, aprovecha los filtros y organiza bien tus informes para que sean fáciles de entender.



Puede que también quieras que las imágenes estén centradas:



### Código de ejemplo para Power Query

```javascript
let
    Source = Csv.Document(File.Contents("C:\Example.csv")),
    Transform = Table.TransformColumnTypes(Source,{{"Date", type date}})
in
    Transform

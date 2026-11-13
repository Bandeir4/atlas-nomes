# Atlas de Nomes

**Cada nombre, una historia.** Un explorador de 102 nombres en Galicia y España para descubrir cuántas personas los llevan, dónde viven y cómo se reparten por edades.

La app combina datos demográficos de 1900 a 2026, un censo de nombres con referencia a 2025 y fichas de significado y procedencia. Puedes explorar un nombre o seleccionar varios para compararlos en la misma gráfica.

## Qué puedes hacer

| Vista | Qué encontrarás |
| --- | --- |
| **Gráficas** | Búsqueda de nombres, filtro por sexo y comparación de residentes, distribución por provincias y municipios gallegos, rangos de edad, edad media y frecuencia por cada 10.000 personas del mismo sexo. También permite consultar cohortes de nacimiento, registros de recién nacidas y comparar Galicia con España cuando hay datos disponibles. |
| **Tabla histórica** | Cifras de población y nombres por fecha, con filas desplegables para consultar desgloses y fuentes. Puedes expandir o contraer todo y filtrar la tabla con los nombres seleccionados en Gráficas. |
| **Significado y procedencia** | Un catálogo con las cifras de los nombres y las fichas etimológicas disponibles, con acceso a sus gráficas. |

## Cómo usarla

1. Abre [index.html](index.html) en un navegador moderno. No requiere instalación ni compilación.
2. Elige **Galicia** o **España**. En España también puedes seleccionar una provincia de residencia.
3. En **Gráficas**, busca y marca los nombres que quieras comparar. Puedes filtrar por sexo; al pulsar **Intro** en el buscador se marcan o desmarcan los resultados visibles.
4. Elige una medida en el selector de la gráfica. Las opciones se adaptan a los datos disponibles; algunas incluyen un selector de provincia de nacimiento o de municipios. Despliega **Ver datos del gráfico** para consultar las cifras y sus fuentes.
5. Visita **Tabla histórica** para examinar los desgloses o **Significado y procedencia** para conocer el origen de un nombre. Usa **Volver a demografía** para recuperar la gráfica de población.

## Cómo interpretar los datos

El botón **Fuentes y metodología** explica las referencias del INE y del IGE, los cálculos y los límites de publicación. Las fichas de origen toman como referencia la *Guía de nomes galegos* de la Real Academia Galega.

| Marca | Significado |
| --- | --- |
| Oficial | Cifra publicada por un organismo estadístico; se indica si procede de una reproducción secundaria. |
| † Derivado | Suma o tasa calculada a partir de datos oficiales. |
| ≈ Estimado | Aproximación, como el reparto de un grupo de edad que cruza un umbral. |
| — Sin dato | No se ha recuperado una cifra verificable. |
| ⋯ Fuera de publicación | La fuente no publica ese cruce por su límite de frecuencia. |
| 0 | Cero observado. |

> Los datos de nombres tienen como corte general el **1 de enero de 2025**. La demografía llega al **1 de julio de 2026**. Las cohortes describen a residentes agrupados por década de nacimiento; los registros de nacimientos corresponden a otra medida y periodo. La cobertura varía según el nombre y el territorio.

## Cómo funciona por dentro

La aplicación está contenida en un único archivo, [index.html](index.html), con HTML, CSS, JavaScript y los datos integrados en JSON. El navegador filtra esos datos y actualiza las tablas y las gráficas SVG al cambiar la selección. No necesita servidor ni consultas a una API para explorar las cifras incluidas; los enlaces a las fuentes permiten consultar las referencias externas.

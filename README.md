# Analisis_renuncias_y_performance_empleados

# Análisis de Desempeño y Satisfacción de Empleados

## Descripción del Proyecto

Este proyecto tiene como objetivo analizar los datos de desempeño y satisfacción de los empleados para identificar patrones y evaluar factores que puedan influir en el desempeño, la satisfacción laboral y la retención de empleados. Se centra en analizar cómo las oportunidades de capacitación, entre otros factores, afectan estas métricas. Los datos utilizados provienen de varios archivos CSV que incluyen información sobre evaluaciones de desempeño, detalles demográficos y niveles de satisfacción de los empleados.

## Archivos de Datos

- **Employee.csv**: Contiene información demográfica y laboral de los empleados.
- **PerformanceRating.csv**: Contiene las evaluaciones de desempeño de los empleados.
- **SatisfiedLevel.csv**: Contiene los niveles de satisfacción de los empleados.
- **RatingLevel.csv**: Contiene los niveles de calificación de desempeño.
- **EducationLevel.csv**: Contiene los niveles de educación de los empleados.

## Descripción de Columnas

### PerformanceRating
- **PerformanceID**: Identificador único de la evaluación.
- **EmployeeID**: Identificador único del empleado evaluado.
- **ReviewDate**: Fecha de la evaluación.
- **EnvironmentSatisfaction**: Calificación de la satisfacción con el entorno laboral.
- **JobSatisfaction**: Calificación de la satisfacción con el trabajo.
- **RelationshipSatisfaction**: Calificación de la satisfacción con las relaciones laborales.
- **TrainingOpportunitiesWithinYear**: Número de oportunidades de capacitación ofrecidas en el año.
- **TrainingOpportunitiesTaken**: Número de capacitaciones aprovechadas.
- **WorkLifeBalance**: Calificación del equilibrio trabajo-vida.
- **SelfRating**: Autoevaluación del empleado.
- **ManagerRating**: Calificación del gerente.

### Employee
- **EmployeeID**: Identificador único del empleado.
- **FirstName**: Primer nombre del empleado.
- **LastName**: Apellido del empleado.
- **Gender**: Género.
- **Age**: Edad.
- **BusinessTravel**: Frecuencia de viajes de negocios.
- **Department**: Departamento.
- **DistanceFromHome**: Distancia desde casa (km).
- **State**: Estado de residencia.
- **Ethnicity**: Etnicidad.
- **MaritalStatus**: Estado civil.
- **Salary**: Salario anual.
- **StockOptionLevel**: Nivel de opciones sobre acciones.
- **OverTime**: Horas extras (Sí/No).
- **HireDate**: Fecha de contratación.
- **Attrition**: Ha dejado la empresa (Sí/No).
- **YearsAtCompany**: Años en la empresa.
- **YearsInMostRecentRole**: Años en el rol actual.
- **YearsSinceLastPromotion**: Años desde la última promoción.
- **YearsWithCurrManager**: Años con el gerente actual.

### SatisfiedLevel
- **SatisfactionID**: Identificador único de satisfacción.
- **SatisfactionLevel**: Nivel de satisfacción (de Muy Insatisfecho a Muy Satisfecho).

### RatingLevel
- **RatingID**: Identificador único de calificación.
- **RatingLevel**: Nivel de calificación (de Inaceptable a Más Allá de lo Esperado).

### EducationLevel
- **EducationLevelID**: Identificador único de nivel educativo.
- **EducationLevel**: Nivel educativo alcanzado (de Sin Calificaciones Formales a Doctorado).

## Objetivos del Análisis

- Identificar los factores que más influyen en el desempeño de los empleados.
- Evaluar la relación entre la satisfacción laboral y la retención de empleados.
- Analizar el impacto de las oportunidades de capacitación en el desempeño.
- Comparar la autoevaluación con la evaluación del gerente.

## Herramientas Utilizadas

- Python (pandas, numpy, matplotlib, seaborn)
- Jupyter Notebooks
- Git/GitHub

## Ejecución del Proyecto

El código del proyecto incluye las siguientes etapas:

1. **Carga y Procesamiento de Datos**: Importación y preparación de los datos desde los archivos CSV.
2. **Análisis Exploratorio de Datos**: Creación de gráficos para entender la distribución de variables clave y correlaciones.
3. **Visualización de Datos**:
   - **Matriz de Correlación**: Para identificar relaciones entre variables.
   - **Gráficos de Distribución**: Histogramas, gráficos de barras y gráficos de pastel para explorar variables categóricas y numéricas.
   - **Series Temporales**: Para analizar tendencias a lo largo del tiempo.
   - **Análisis de Retención**: Evaluación del impacto de la capacitación en la retención y calificaciones de los empleados.
   - **Distribución Salarial**: Análisis de la influencia de diferentes factores en la distribución salarial.

### Ejecución del Código

1. Asegúrate de tener todos los archivos CSV mencionados en el directorio raíz del proyecto.
2. Instala las dependencias necesarias con el siguiente comando:
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn xgboost
   ```
3. Ejecuta el script en un entorno compatible con Python (como Jupyter Notebook) para ver los resultados y gráficos generados.

## Resultados Clave

- **Distribución Demográfica**: La información obtenida muestra que California es el principal estado de residencia para la mayoría de los empleados de la empresa, indicando su importancia. La distribución de género, antecedentes educativos y asignaciones de viajes de negocios es equilibrada, sugiriendo la ausencia de discriminación. Los datos revelan un predominio de empleados blancos y una fuerza laboral mayoritariamente joven, entre 20 y 25 años. Sin embargo esto no refleja un sesgo en la distribución salarial y en los ascensos, ya que es acorde a la distribución general de la población


- **Análisis Salarial**: El análisis muestra que la edad influye significativamente en los salarios, con los empleados más jóvenes ganando más que la media, lo que podría indicar una preferencia por talento joven y una estrategia de movilidad entre departamentos. No obstante, la rotación de directivos y la falta de estabilidad en los puestos clave podrían afectar la cohesión del equipo y la planificación estratégica.

- **Tendencias Temporales**: Desde 2012, se observa una disminución en los años promedio de permanencia en la empresa, posiblemente relacionada con un aumento en la contratación de nuevos empleados. Además, después de una caída significativa en los salarios hasta 2016, se ha estabilizado desde entonces, sugiriendo ajustes en las prácticas de remuneración para atraer o retener talentos. El aumento y posterior disminución de los salarios hasta 2020 podría reflejar una respuesta a las presiones económicas externas, como la pandemia COVID-19. Un análisis más detallado es necesario para entender completamente estas tendencias y sus causas.

## Conclusión

El análisis muestra una serie de patrones y tendencias en el desempeño y la satisfacción de los empleados, proporcionando información valiosa sobre la influencia de factores como la capacitación y la edad en la retención y la satisfacción laboral. La empresa podría beneficiarse de abordar problemas relacionados con la estabilidad del liderazgo y considerar estrategias para mejorar la retención de empleados.


---

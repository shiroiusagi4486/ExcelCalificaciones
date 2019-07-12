# ExcelCalificaciones
Proyecto para concentrado y pequeño análisis de calificaciones provenientes de un varios documentos de excel

Este proyecto utiliza datos reales obtenidos durante el ultimo cuatrimestre del año 2018, que son calificaciones de alumnos, aunque no existe como tal una politica de privacidad, al ser documentos personales, no los voy a incluir en el proyecto, puesto que la primera parte del codigo se utiliza para extraer toda la informacion de los excel y subirlos a una base de datos de mongodb conectada a atlas.

La segunda parte del proyecto, se llevara a cabo la limpieza de los registros, comenzando con la eliminacion de la columna _id, que corresponde a una columna de mongo, despues se limpiarán los datos repetidos que se encuentren en el dataframe, la separacion de los datos  y calculos de los siguientes elementos:

-Promedio parcial de los alumnos por materia, ( hay que separar los grupos)
-Promedio de materia por grupo (sirve la separacion por grupos, pero hay que calcular los promedios generales)
-Promedio del profesor por materia que imparte, (Es muy similar a la anterior y se podria usar para asignar al profesor que le de a ese grupo, pero hay que filtrar tambien)
-Promedio general del profesor
-Promedio general de la carrera por cada parcial
-Promedio general de la carrera por cuatrimestre
-Promedio de grupos por cuatrimestre

La idea es que se separen del dataframe original todos esos subdataframe siempre después de identificar y remover duplicados


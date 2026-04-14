# AI Log - Equipo Pumatécnicos

## Herramientas
- Google Gemini 3 Flash

## Filosofía de uso
Decidimos usar IA exclusivamente para tareas mecánicas y
de exploración inicial. La narrativa, la selección de
variables y las decisiones editoriales fueron 100% del
equipo. Nuestro criterio: si la tarea requiere
conocimiento del contexto social, la hacemos nosotros.

## Registro de uso 

### 2026-03-30 | Gemini | Mapa de la república con JSON
- **Tarea**: Le pedimos ayuda para crear un deslizador
  en varios mapas de la republica, para ver la evolución
  de las entidades para diferentes periodos
- **Prompt**: "como puedo hacer un deslizador en plotly
  para graficas de mapas de diferentes años, que se deslice
  por cada año"
- **Resultado**: Nos dió código de python, con el parámetro
  animation.frame
- **Decisión**: Elegimos conservar el deslizador, porque
  comunica de mejor forma la evolución de todos los estados
  en un solo espacio; la personalización visual y creación de
  categorías fue manual y discutida con el equipo.

### 2026-04-01 | Gemini | Limpieza de datos
- **Tarea**: Le pedimos ayuda para convertir las entradas
  a números, ya que tenían un caracter asociado a su
  coeficiente de variación (e.g. a/), lo que hacía que todas las entradas
  del dataframe fueran de tipo string
- **Prompt**: "como puedo recuperar la ultima parte de una entrada i,j
  de un data frame, asignar ese valor a una nueva columna y borrarlo
  de la orignal es decir, si la observacion es "40.9127745397439 a/",
  quiero recuperar ese "a/" asociado a un 15% y luego dejar solo "40.9127745397439" como numero"
- **Resultado**: Nos dió un código usando el método .extract
- **Decisión**: Usamos el código, cambiando las variables para que fueran
  más representativas en el contexto del problema 




### NO usamos IA para hacer lo siguiente:
- La selección de los ODS, y las metas más relevantes de cada uno (revisión de
  literatura y discusión en equipo)
- La narrativa del tablero (redacción propia, consultando definiciones en fuentes oficiales)
- La interpretación de gráficas

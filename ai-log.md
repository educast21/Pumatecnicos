# AI Log - Equipo Pumatécnicos

## Herramientas
- Google Gemini 3 Flash
- ChatGPT Thinking 5.4

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

### 2026-04-11 | ChatGPT | Descripciones oficiales
- **Tarea**: Le pedimos ayuda para encontrar recursos digitales donde se definieran términos como inseguridad alimentaria moderada y severa, seguridad social, emaciación, desnutrición, malnutrición, etc.
- **Prompt**: En el prompt se establecieron instrucciones explícitas de las fuentes no permitidas para la consulta de información.
- **Resultado**: Un total de 11 sitios web  y pdf, mediante los cuáles se describían tanto las definiciones propuestas por la instituciones extrangeras (ONU y OMS, entre otras), como nacionales (INEGI y CONEVAL).
- **Decisión**: La lectura de los recursos digitales permitió robustecer la explicación e interpretación de cada indicador, para el diseño de las gráficas.

### 2026-04-14 | ChatGPT | Debugear una función
- **Tarea**: Se le pidió encontrar el fallo en una función diseñada para la graficación en serie de tiempo y barras, de distintas variables, a través de un botón interactivo.
- **Prompt**: En el prompt se entregó la función, el error obtenido, las características del dataset y especificaciones del gráfico esperado.
- **Resultado**: Una función que corregía el fallo, el cuál se identificó como la sintaxis incorrecta del botón interactivo además de mala especificación de los colores de la gráfica.
- **Decisión**: Se adoptó la función corregida para el diseño de un gráfico ineractivo.

### NO usamos IA para hacer lo siguiente:
- La selección de los ODS, y las metas más relevantes de cada uno (revisión de
  literatura y discusión en equipo)
- La narrativa del tablero (redacción propia, consultando definiciones en fuentes oficiales)
- La interpretación de gráficas

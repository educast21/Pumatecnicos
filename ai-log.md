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

### 2026-03-15 | Copilot | Boilerplate de gráficas
- **Tarea**: Generar código base para 6 gráficas en
  plotly.
- **Resultado**: Templates funcionales para bar, line,
  choropleth, scatter, heatmap, y funnel.
- **Decisión**: Descartamos 3 de las 6. El heatmap no
  comunicaba bien la estacionalidad (probamos y era
  confuso). El scatter no era apropiado para datos
  categóricos por municipio. Nos quedamos con bar, line
  y choropleth. Toda la personalización visual (paleta
  basada en identidad del ODS 6, etiquetas en español,
  anotaciones contextuales) fue manual.


### NO usamos IA para hacer lo siguiente:
- La selección de las 4 variables clave (revisión de
  literatura y discusión en equipo)
- La narrativa del tablero (redacción propia, 3
  iteraciones internas)
- La interpretación de outliers en Acapulco post-Otis
  (conocimiento local del equipo)

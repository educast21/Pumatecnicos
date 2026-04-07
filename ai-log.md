# AI Log - Equipo Pumatécnicos

## Herramientas
- Claude (claude.ai)
- GitHub Copilot (VS Code)

## Filosofía de uso
Decidimos usar IA exclusivamente para tareas mecánicas y
de exploración inicial. La narrativa, la selección de
variables y las decisiones editoriales fueron 100% del
equipo. Nuestro criterio: si la tarea requiere
conocimiento del contexto hídrico de Guerrero, la
hacemos nosotros.

## Registro de uso 

### 2026-03-15 | Claude | Exploración de estructura
- **Tarea**: Le pedimos 3 opciones de layout para un
  tablero de Quarto con 4 secciones temáticas.
- **Prompt**: "Dame 3 estructuras de layout en Quarto
  dashboard para un proyecto con 4 secciones: contexto
  geográfico, acceso a agua, calidad del agua, y
  tendencia temporal"
- **Resultado**: Nos dio layouts con tabs, sidebar y
  scroll vertical.
- **Decisión**: Elegimos sidebar porque nuestro usuario
  objetivo  necesita
  navegar entre secciones sin perder el contexto del mapa
  principal. 

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

### 2026-03-16 | Claude | Revisión de narrativa
- **Tarea**: Le pedimos que criticara nuestro borrador de
  narrativa de la sección de acceso a agua.
- **Prompt**: "Critica este texto como si fueras un editor
  de datos. ¿La narrativa conecta bien los datos con el
  argumento? ¿Hay saltos lógicos?"
- **Resultado**: Señaló que no conectábamos el dato de
  cobertura municipal con el argumento de desigualdad
  regional.
- **Decisión**: Agregamos un párrafo puente con el
  coeficiente de Gini de acceso hídrico que ya teníamos
  calculado pero no habíamos integrado. El texto final
  es completamente nuestro, la IA solo fungió como
  revisor crítico.

### NO usamos IA para hacer lo siguiente:
- La selección de las 4 variables clave (revisión de
  literatura y discusión en equipo)
- La narrativa del tablero (redacción propia, 3
  iteraciones internas)
- La interpretación de outliers en Acapulco post-Otis
  (conocimiento local del equipo)

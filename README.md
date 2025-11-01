# CFE-IA-E11

## Sesgos en Noticias

## Descripción del corpus utilizado

Para este ejercicio se empleó el dataset Spanish News Classification, que contiene más de 15.000 noticias reales en español distribuidas en distintas categorías (política, economía, sociedad, deportes, entre otras).
El corpus refleja el lenguaje periodístico utilizado en medios hispanohablantes, lo que lo convierte en un recurso útil para detectar sesgos semánticos y narrativos en la cobertura informativa.

Durante la exploración inicial se observaron patrones de asociación entre ciertos términos ideológicos, sociales y morales, lo cual motivó el análisis de posibles sesgos de género, clase y criminalidad en las representaciones del lenguaje.

## Palabras seleccionadas y razones

### Las palabras elegidas fueron:

"migrante", "extranjero", "policía", "criminal", "rico", "pobre", "víctima", "culpable"

Estas se escogieron por su potencial para revelar asociaciones polémicas o estereotipadas dentro del discurso noticioso.
En particular, se buscó analizar los siguientes ejes de sesgo:

Género e ideología: feminista y machista, términos que suelen aparecer en contextos opuestos o polarizados.

Clase social: rico y pobre, que representan extremos económicos y suelen cargar con juicios implícitos.

Migración y pertenencia: migrante y extranjero, usados con frecuencia en coberturas sobre desplazamiento o conflicto.

Seguridad y criminalidad: policía y criminal, asociados con autoridad, control y delito.

Moralidad y responsabilidad: víctima y culpable, que reflejan el tratamiento de justicia y empatía en los relatos mediáticos.

## Visualización e interpretación

A continuación se muestra el mapa 2D, donde se representan las relaciones semánticas entre los términos seleccionados según su proximidad en el espacio vectorial:

<img width="746" height="548" alt="image" src="https://github.com/user-attachments/assets/ac189861-8ac4-4327-afe1-a5657e352554" />

## Interpretación del gráfico:

Se observa una agrupación cercana entre “rico”, “policía”, “migrante” y “culpable”, lo que sugiere que en el corpus estas palabras comparten contextos de autoridad, control o conflicto social.

“Pobre” se encuentra algo aislado, indicando que aparece en contextos diferentes, posiblemente relacionados con vulnerabilidad o desigualdad.

“Víctima” ocupa una posición separada en la parte superior, asociada a contextos de empatía, violencia o desgracia, marcando un contraste semántico con “culpable”.

“Extranjero” aparece claramente distanciado, lo que podría reflejar un uso en contextos específicos o diferenciados, como noticias internacionales o migratorias.

En conjunto, el mapa muestra zonas de proximidad semántica donde los significados tienden a reforzar estereotipos mediáticos, como la vinculación entre pobreza, criminalidad y migración, o la asociación de ciertos grupos con victimización o culpabilidad.

## Observaciones de sesgo

El análisis sugiere la presencia de sesgos semánticos en el corpus de noticias:

Sesgo de clase: “Rico” y “pobre” se ubican en regiones distintas del espacio, lo que puede reflejar una narrativa desigual en torno a la riqueza y la vulnerabilidad.

Sesgo migratorio: La cercanía entre “migrante”, “culpable” y “policía” puede indicar una tendencia del discurso mediático a relacionar la migración con la criminalidad o la vigilancia.

Sesgo moral: “Víctima” y “culpable” aparecen opuestos, reforzando una estructura binaria común en las noticias sobre crimen y justicia.

Estos patrones evidencian cómo los modelos de lenguaje capturan y amplifican las estructuras de sentido existentes en el discurso periodístico.

## Reflexión ética

El hallazgo de sesgos en representaciones lingüísticas provenientes de medios de comunicación plantea importantes desafíos éticos.
Si los modelos de procesamiento de lenguaje natural (PLN) reproducen asociaciones negativas —por ejemplo, entre “migrante” y “culpable”—, pueden reforzar prejuicios sociales y discriminación en sistemas automatizados (como chatbots, filtros o generadores de contenido).

La ética en IA exige un análisis crítico de los datos antes de su uso, así como estrategias de mitigación (re-balanceo de corpus, neutralización de embeddings, auditorías de sesgo) que garanticen una representación más justa y equitativa de las personas y grupos.

Conclusión

El ejercicio evidencia que los embeddings entrenados con noticias reales no son neutrales: reflejan las tensiones, ideologías y prejuicios presentes en el lenguaje mediático.
Analizar estas relaciones ayuda a visibilizar cómo el discurso informativo moldea percepciones sociales y a promover un uso responsable del PLN en aplicaciones periodísticas y tecnológicas.

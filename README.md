# Scoring de aplicaciones a posiciones

Este notebook muestra como aplicar un scoring de un currículum aplicado a una posición


Se parte de datos no estructurados, como el currículúm vitae de una persona y se compara con los datos estructurados de una posición. La posición tiene el siguiente formato:

- descripción
- lista de requisitos: cada requisito tiene el formato <skill, nivel, descripción, obligatorio (sí/no)>
- lista de tareas a realizar
- tags de la oferta


Para transformar un CV a datos estructurados se utiliza un prompt, de modo que un LLM procese el CV y genere la siguiente estructura:

- resumen
- puntos clave del candidato
- puntos débiles del candidato
- hard skills
- soft skills
- tareas y responsabilidades que ha realizado en sus últimos 5 años
- posibles preguntas de la entrevista
- años totales de experiencia
- permanencia media en las empresas
- tags


[Open in Colab](https://colab.research.google.com/github/jaruizes/AI-CVMatcher/blob/main/ApplicationsScoring.ipynb)

# Milestone_1_PLN
1ºParte trabajo de Procesamiento de Lenguaje Natural Escrito 

ARCHIVO CORRECTO: Tarea_1_proyecto_PLN.ipynb

Fran ha realizado su parte del trabajo, ha cargado el dataset, ha hecho una exploracion de este para futuras limpiezas, luego a limpiado el dataset (espaciado, signos de puntuacion inecesarios, etc) a partir de las salidas obtenidas en la EDA. A posteriori, se ha realizado una extracción lingüistica de la informacion para obtener un vocabulario filtrado y con las palabras mas frecuentes anotadas como insultos (aunque en realidad hay muchas que no las hay). También hemos obtenido n-gramas para formar un vocabulario robusto de insultos frecuentes en el idioma portugués y considerarlo como primera regla de activacion para clasificar un post como ofensivo. Y por último se ha mostrado como el siguiente alumno debe seguir el trabajo buscando patrones con ayuda del vocabulario de palabras negativas o insultos para formalizar reglas y posteriormente su programacion y su orden de activación segun su importancia (para eso hay que basarse en porcentajes dentro del dataset viendo que porcentaje de los posts que cumplen la regla dentro del dataset se consideran como ofensivos). Finalmente se probará cuales son el conjunto de reglas que mejor accuracy tiene para predecir los posts del dataset. Para ello iremos probando si con una regla solo las metricas van mejor o si la combinacion de estas tres reglas pera esta otra no consigue la mejor combinacion de sistema de reglas para predecir los posts.

COSAS POR HACER:
1. Aplicar polaridad para ver si el sentimiento completo de una frase es positivo o negativo --> para ver cual es el umbral ideal para hacer la regla propuesta
2. Extraer entidad sobre un subconjunto elevado del dataset para ver si podemos encontrar entidades frecuentes que nos indican que el post puede clasificarse como ofensivo
3. Ver por qué el patrón 2ºpersona + insulto tiene un porcentaje tan pequeño de ser clasificado como ofensivo (solo el 25%) --> alomejor estamos hablando del 25% del total del dataset (puede haber posts en los que no está la estructura de 2ºpersona + insulto) o puede ser por otra razón: alomejor el 25% de esta estructura utiliza un insulto que es considerado como tal pero en realidad no lo es (para ello haz el código y mira los ejemplos de los que ha sacado el porcentaje para tomar conclusiones)
4. Ver por qué el patrón 2ª persona + ADJ negativo tiene un porcentaje tan pequeño de ser clasificado como ofensivo (solo el 6'5%) --> DARLE UNA VUELTA igual que 3.
5. Ver por que los posts con mas emojis se clasfican en inofensivos --> distinguir entre emojis que aportan info negativa y emojis que aportan info positiva para incluir en el vocabulario de insulto o de insultos hechos

Además, faltará redactar el proceso en un documento aparte en inglés (uno es español para entendernos nosotros y el de entrega en inglés) y borrar todos los emojis del código --> sino canta mucho que lo ha hecho chatgpt. El documento en español donde debemos redactar nuestro proceso es el siguiente: MILESTONE_1 (word) --> aqui tambien están las posibles reglas para programar

También, se reestructurará el archivo .ipynb porque hay varias celdas de código que no aportan infromación real en las decisiones o desarrollo posterior del proyecto o directamente no funcionan, y se dejará solo lo relevante. Incluso habrá que modificar los comentarios de texto despues del código que lo explican y luego traducirlo al inglés.

PREGUNTAS PROFESORA:
1. ¿Cómo debo usar chatgpt? ¿Lo puedo usar para que me dé el código o para que?
2. ¿Debo basarme en las practicas y su código para hacer el trabajo? ¿Para que sirven entonces? ¿Cuál es la práctica en la que debo fijarme para hacer el proyecto? ¿Practica 1 y 2 solo? (pues la practica 3 y 4 es sobre aprendizaje automatico --> modelos para entrenar y predecir)
3. ¿Dónde puedo investigar para hacer el resto del trabajo?
4. ¿Puedo tener los comentarios del código en español para aclararme yo mejor o es necesario tenerlos en ingles/portuges? ¿Y sobre la doc del trabajo?
5. ¿Qué debo incluir en la documentación? ¿Explicación del código o solamente las decisiones tomadas durante el proyecto y los resultados obtenidos?
6. ¿Cuántas reglas debo incluir?
7. ¿Qué procentaje de accuray o F1 Score debo conseguir para que esté medianamente bien el proyecto?

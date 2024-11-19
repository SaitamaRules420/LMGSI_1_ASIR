**Ejercicio 11**  

**Etiquetas**  
Las únicas etiquetas de bloque utilizadas son **h1**, **p** y **div**.  

**Clases**  
Cada cita tiene la letra inicial diferente al resto del párrafo. Se podría utilizar una etiqueta **span** con clase, pero puesto que se trata del primer carácter, se puede utilizar simplemente el pseudo-elemento ::rst-letter, que no requiere añadir nada al código fuente html.  

**Posicionamiento**  
Los párrafos tienen forma cuadrada y tienen todos el mismo tamaño, independientemente del contenido, lo que se puede conseguir dando el mismo valor a las propiedades width y height.  
Las citas se muestran una al lado de la otra formando una trama rectangular. Además, al hacer zoom o al estrechar o ensanchar la ventana, el número de citas por la se ajusta automáticamente. Eso se puede conseguir con posicionamiento flotante.  
Si el tamaño del párrafo es sucientemente grande, no es necesario definir la propiedad overflow, aunque por precaución se puede incluir en la hoja de estilo.  
Como no hay ningún elemento después de las citas, no hace falta utilizar la propiedad clear en ningún elemento.  
La letra inicial de cada párrafo (pseudo-elemento ::first-letter) tiene posicionamiento flotante.
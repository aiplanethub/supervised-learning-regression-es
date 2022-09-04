## Sesgo y Varianza en el mundo real

En términos de diccionario:

**Sesgo (Bias):** Prejuicio a favor o en contra de una cosa, persona o grupo en comparación con otro, generalmente de forma considerada injusta.

**Varianza (Variance):** Estado o hecho de estar en desacuerdo o en disputa.

En resumen, el Sesgo representa lo injusto que es algo hacia los demás, y la Varianza representa la probabilidad de que algo cambie con respecto a los demás.

¿Confuso? No se preocupe. El siguiente ejemplo aclarará todas tus dudas.

## Ejemplo

Supongamos que ha llamado a dos examinadores del tiempo, el Sr. Bishop y el Sr. Varian, para que comprueben si va a llover o no.

Al Sr. Bishop le gusta mucho la lluvia. Y el Sr. Varian es un ratón de biblioteca. Hablemos de las condiciones de la lluvia.

* **Llueve sólo cuando hay un poco de humedad.**
* **No llueve si hace viento, calor o frío.**

### Sr. Bishop representando a Sesgo

Le preguntas al Sr. Bishop (A pesar de su formación, es demasiado tendencioso con la lluvia):

Yo: Señor, hace mucho calor aquí. ¿Lloverá?

Sr. Bishop: Sí.

Yo: Señor, hace un poco de viento. ¿Lloverá?

Sr. Bishop: Tal vez no.

Yo: Señor, hace mucho frío. ¿Lloverá?

Sr. Bishop: Sí, por supuesto.

Yo: Señor, hay un poco de humedad. ¿Lloverá?

Sr. Bishop: Por supuesto.

¿Te has dado cuenta de que el Sr. Bishop está muy predispuesto a las posibilidades de que llueva? Durante la prueba, es incapaz de predecir correctamente la mayoría de ellas.

Esta condición se llama **bajo ajuste (under fitting)**.

### El Sr. Varian representa la varianza

Veamos ahora su conversación con el Sr. Varian (un ratón de biblioteca que recuerda completamente el entrenamiento que tuvo):

Yo: Señor, hace mucho calor aquí fuera. ¿Lloverá?

Sr. Varian: No.

Yo: Señor, hace un poco de viento. ¿Lloverá?

Sr. Varian: De ninguna manera.

Yo: Señor, hace mucho frío. ¿Lloverá?

Sr. Varian: De ninguna manera.

Yo: Señor, hay un poco de humedad. ¿Lloverá?

Sr. Varian: Sí, lloverá.

El Sr. Varian predijo con éxito si llovería o no. Pero al ser un ratón de biblioteca, el Sr. Varian desconoce las condiciones no descritas en el libro durante el entrenamiento.

Ahora, le preguntamos al Sr. Varian :

Yo: Señor, un gigante que perdió su caramelo, está sentado en la nube. ¿Lloverá?

Sr. Varian: No estoy seguro. Como la respuesta es "No" a la mayoría de las condiciones, hay una alta posibilidad de que no llueva.

Ahora bien, aunque la decisión del Sr. Varian varía perfectamente con las condiciones de entrada, no puede predecir basándose en las condiciones nuevas y no vistas (otras condiciones generales aparte de las condiciones específicas dadas durante el entrenamiento).

Esta condición se denomina **sobreajuste (overfitting)** Y ofrece **poca generalizabilidad**.

## ¿Alto sesgo o alta varianza?

Entonces, ¿qué es mejor, un sesgo alto (alta generalizabilidad) o una varianza alta (alta precisión en los datos de entrenamiento)?

La respuesta es: "Lo mejor de ambos mundos". No necesitamos ni un alto sesgo ni una alta varianza. Queremos que nuestro algoritmo funcione mejor en el conjunto de entrenamiento y ofrezca el mejor resultado en los datos no vistos (el conjunto de prueba).

En general, **tener un sesgo alto reduce el rendimiento del algoritmo en el conjunto de entrenamiento, mientras que tener una varianza alta reduce el rendimiento en los datos no vistos**.

Esto se conoce como **compensación de sesgo y varianza**.

### Material de lectura

DEBE LEER

Comprender el equilibrio entre la varianza y el sesgo: https://towardsdatascience.com/understanding-the-bias-variance-tradeoff-165e6942b229

### Referencia

https://medium.com/@viveksingh.heritage/an-intuitive-explanation-to-bias-variance-tradeoff-ec540fb13e12

### Enlace de descarga de diapositivas

Puede descargar las diapositivas de este tema desde [aquí](https://docs.google.com/presentation/d/1NjaYyvdQTJ-ygdp5MAnWxDg\_qlSMIIhmQAaXiPAraO4/edit?usp=sharing).
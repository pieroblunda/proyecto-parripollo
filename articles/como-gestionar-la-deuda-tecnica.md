# Cómo gestionar la deuda técnica

[Krzysztof Liszewski - 3 de julio de 2019](https://4agile.pl/how-to-manage-technical-debt/)

Hablemos un poco sobre la deuda técnica. Habrá alguna teoría, pero espero que este artículo no vaya en contra de mi Manifiesto. Todavía tengo como objetivo darle herramientas prácticas para la discusión y explicar por qué y cómo manejar la deuda técnica.

## ¿Qué es una deuda técnica entonces?

Hay muchas definiciones que puedes encontrar fácilmente en la web. Algunos de ellos son muy estrechos, como el de Wikipedia: "La deuda técnica (también conocida como deuda de diseño o deuda de código) es un concepto en el desarrollo de software que refleja el costo implícito del retrabajo adicional causado por elegir una solución fácil (limitada) ahora en lugar de usar un mejor enfoque que llevaría más tiempo". Algunos son muy amplios y dividen la deuda técnica en varias categorías, como: Código, Diseño, Documentación, Defectos, Tecnología, Negocios, etc.

> En este artículo me gustaría considerar la deuda técnica como una diferencia entre el estado actual de un sistema y el sistema ideal, que tiene el mismo conjunto de funcionalidades.

No importa qué definición utilices, creo que hay una cosa con la que todos estarían de acuerdo: cuanto más deuda técnica tengamos en el sistema, mayor será el costo de su mantenimiento y desarrollo posterior. Presentándolo en un gráfico, se verá como se muestra a continuación:

![](../assets/cost-of-new-feature.png)

El costo base es un costo de desarrollar una nueva característica en un sistema ideal. Cuando el nivel de deuda técnica aumenta, el costo de desarrollar una nueva característica también aumentará.

> Si no controla su nivel de deuda técnica, puede causar un aumento tanto en el costo de las nuevas características que un mayor desarrollo se volverá imposible.

## ¿Cuánto cuesta la calidad?

Siempre debes tener al menos una parte interesada centrada en la calidad. En Scrum, este puede ser el equipo de desarrollo (ver más aquí: calidad frente a cantidad). ¿No les gustaría a todos mantener sus sistemas de TI de excelente calidad? Seguramente lo harían, pero nada se da por sentado: cuanto mejor calidad te gustaría alcanzar, más necesitarás pagar. Poniendo esto en un gráfico, lo veremos de la siguiente manera:

![](../assets/cost-of-quality.png)

Cuanto más deuda técnica tenga, menos pagará por mejoras de calidad. Cuanto menos deuda técnica tengas, más caro será aumentar aún más la calidad.

> Tener un sistema sin deuda técnica (lo ideal) le costaría una cantidad infinita de dinero.

## Gestión técnica de la deuda

Ahora combinemos dos gráficos en uno e intentemos usarlo para tomar decisiones. Recuerda:

* más deuda técnica = menos calidad
* menos deuda técnica = más calidad

Primero, suponiendo que tengamos un sistema de alta calidad:

![](../assets/cost-when-low-technical-debt.png)

En este sistema, el costo de eliminar aún más la deuda técnica es mucho más alto que agregar nuevas características. Por lo tanto, es prudente centrarse en las nuevas características que ofrecen valor comercial a los clientes a corto plazo. Agregar nuevas características, por supuesto, creará alguna nueva deuda técnica (documentación faltante, cobertura de prueba más baja de lo esperado, algunos atajos en el código, etc.) que a su vez disminuirá un poco nuestra calidad. Así que nos moveremos en consecuencia a las flechas verdes.

En segundo lugar, suponiendo que tengamos un sistema de baja calidad:

![](../assets/cost-when-high-technical-debt.png)

En dicho sistema, el costo de eliminar la deuda técnica es menor que agregar nuevas características. Por lo tanto, es bueno centrarse en mejorar la calidad del sistema (disminuyendo la deuda técnica), lo que aumentará nuestra capacidad de desarrollo a largo plazo. La disminución de la deuda técnica mejorará la calidad y disminuirá el costo del desarrollo de nuevas características (de nuevo, mueva en consecuencia a las flechas verdes).

## Conclusión

Después de combinar estas dos decisiones (invertir en el desarrollo de nuevas características o en la calidad del sistema) en un gráfico, notará que oscilará cerca del punto de cruce.

![](../assets/technical-debt-oscilation.png)

Cuando el costo de agregar nuevas funciones es demasiado alto, cambias de prioridad y te centras en la calidad (eliminar la deuda técnica). Cuando el costo de mejoras de calidad adicionales es demasiado alto, cambias el enfoque al desarrollo de nuevas características.

> El equilibrio entre los objetivos a corto y largo plazo, ofrecer nuevas características frente a invertir en calidad, es crucial. El mejor enfoque es trabajar en nuevas características y calidad simultáneamente.

Teniendo en cuenta que cada nuevo desarrollo aumenta la deuda técnica, siempre debe recordar y trabajar en la calidad al mismo tiempo. Si tienes el equilibrio adecuado, tu oscilación será muy estrecha, tal vez el evento no se note, siempre estarás en el punto de cruce. Si no tienes equilibrio, entonces perderás tiempo, esfuerzo y enfoque en cambiar entre la calidad y las nuevas características. Los síntomas que muestran que pueden ser: desarrolladores que luchan por iniciativas de calidad, refactorización o Sprints técnicos, fases de estabilización y similares.

## ¿Cuál es mi nivel de deuda técnica?

Como probablemente haya notado, para una gestión técnica adecuada de la deuda, necesita saber dónde se encuentra: cuál es su nivel de deuda técnica y cómo está cambiando.

> Sin el conocimiento adecuado, no podrás encontrar el punto de cruce y ceñirte a él.

Le recomiendo encarecidamente que haga un breve taller con el equipo de desarrollo, centrado en definir las métricas adecuadas para la medición de la deuda técnica. A continuación se muestra una línea de tiempo y una descripción del taller que hice en mi equipo. ¡Siéntete libre de usarlo y compartir tu experiencia y conclusiones!

[0-20 min] ¿Cuál es la deuda técnica? Escribe en notas adhesivas tantos ejemplos de deuda técnica como puedas.
[20-40 min] Agrupamos las notas adhesivas en un par de categorías. ¡Primer grupo! Luego intenta nombrar grupos.
[40-60 min] ¿Cuáles son las posibles medidas para cada grupo? Lluvia de ideas y generación de notas adhesivas. Parte 1.
[60-70 min] Descanso. Mesa de fútbol en nuestro caso. 😊
[70-90 min] ¿Cuáles son las medidas posibles por grupo? Lluvia de ideas y generación de notas adhesivas. Parte 2.
[90-110 min] Evalúemos nuestras ideas. Ponga todas las medidas en dos dimensiones: valor y usabilidad frente a la complejidad y la carga de trabajo necesarias para configurarlo.
[110-120 min] Elija 3-5 métricas y comience a usarlas para la gestión técnica de la deuda.

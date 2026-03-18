# History

## Waterfall - 1970

Para comprender el origen del modelo Waterfall (o en Cascada), debemos viajar a las décadas de 1950 y 1960. En aquel entonces, el software no se consideraba una industria independiente, sino un componente secundario del hardware. El escenario era de una rigidez absoluta, dominado por la ingeniería de sistemas complejos para el sector militar y aeroespacial.

El desarrollo de software nació dentro de organizaciones que ya sabían cómo construir grandes infraestructuras físicas: puentes, barcos y cohetes. Por lo tanto, se aplicó la lógica de la Ingeniería Civil y Mecánica.

En estos sectores, el costo de un error en las fases finales es catastrófico. Si construyes un puente con un acero incorrecto, no puedes "refactorizar" los cimientos una vez que el asfalto está puesto. Por lo tanto, el escenario exigía una planificación exhaustiva y secuencial. Se asumió que el software debía seguir el mismo camino: una fase de diseño perfecta antes de mover un solo gramo de "tierra" (escribir código).

Aunque hoy lo criticamos por su rigidez, en su momento Waterfall fue una respuesta necesaria a una situación de caos total conocida como la "Programación de tipo Cowboy". Los problemas que intentó mitigar fueron:

* La imprevisibilidad del coste y el tiempo: Antes de Waterfall, los programadores escribían código de forma artesanal y desordenada. Era imposible para un gestor saber cuánto faltaba para terminar un proyecto. Waterfall introdujo "hitos" claros que permitían a la gerencia tener una ilusión de control y previsibilidad financiera.

* La fragilidad del hardware: En los años 60, el tiempo de computación era extremadamente caro y limitado. No podías permitirte el lujo de "probar y fallar" (como hacemos hoy con Agile). Había que estar muy seguro de lo que se iba a procesar antes de ocupar las tarjetas perforadas. Waterfall obligaba a pensar todo el problema de antemano para minimizar el uso de hardware costoso.

* La falta de personal especializado: Había muy pocos programadores senior. El modelo Waterfall permitía que un pequeño grupo de "Arquitectos" diseñara todo el sistema, y luego personal menos cualificado se limitara a traducir esos diagramas a código, como obreros en una línea de montaje siguiendo un plano.

La industria (especialmente el Departamento de Defensa de EE.UU. con su estándar DOD-STD-2167A) adoptó solo la parte visual y lineal porque encajaba perfectamente con la mentalidad de gestión de proyectos a destajo y contratos de precio cerrado. Era fácil de auditar, fácil de medir en un gráfico de Gantt y, sobre todo, daba una falsa sensación de seguridad a quienes pagaban por el software.

En resumen, Waterfall no fue un error, sino una transferencia de la lógica de la línea de montaje y la ingeniería civil a un mundo (el software) que aún no entendíamos que funcionaba bajo leyes ontológicas totalmente distintas.

**Principales problemas de waterfall**

El mayor inconveniente del modelo Waterfall es su extrema rigidez, ya que asume que el desarrollo de software es un proceso lineal y predecible, similar a construir un puente. Al exigir que una fase esté totalmente terminada y aprobada antes de pasar a la siguiente, el modelo se vuelve alérgico a los cambios. En un entorno donde los requisitos suelen evolucionar a medida que el cliente entiende mejor sus propias necesidades, esta estructura obliga al equipo a "nadar contra la corriente" si surge cualquier modificación a mitad de camino, lo que dispara los costos y los tiempos de entrega.

Esta linealidad provoca lo que conocemos como el efecto túnel, un fenómeno donde el cliente participa activamente al inicio para definir los requisitos y desaparece hasta el final para recibir el producto. El riesgo es enorme: después de meses de trabajo aislados, es muy común que el equipo entregue algo que cumple técnicamente con el contrato inicial, pero que ya no encaja con la realidad del mercado o con lo que el usuario realmente necesita en ese momento. Es, en esencia, una apuesta a todo o nada que se juega en el último minuto.

Otro problema crítico es la postergación de las pruebas. En Waterfall, el control de calidad ocurre justo antes del despliegue. Esto significa que si hubo un error de concepto o de arquitectura en las primeras semanas del proyecto, nadie lo notará hasta que el sistema esté casi terminado. Corregir un fallo estructural en esta etapa tardía es muchísimo más caro y traumático que detectarlo sobre la marcha, lo que suele generar un clima de pánico y estrés extremo en las fechas de entrega finales.

Finalmente, este modelo genera una falsa sensación de progreso basada en la documentación pesada en lugar de resultados tangibles. Se pueden pasar meses redactando especificaciones técnicas brillantes, pero mientras no haya una sola línea de código funcionando, el valor real para el negocio es cero. Al carecer de entregas parciales o prototipos funcionales, la incertidumbre sobre si el sistema realmente funcionará bajo condiciones reales se mantiene hasta el cierre del ciclo, convirtiendo el lanzamiento en un momento de alta tensión.

**En resumen**

* En la vida real, un proyecto rara vez sigue una secuencia lineal, esto crea una mala implementación del modelo, lo cual hace que lo lleve al fracaso.
* El proceso de creación del software tarda mucho tiempo ya que debe pasar por el proceso de prueba y hasta que el software no esté completo no se opera.
* Esto es la base para que funcione bien. Cualquier error de diseño detectado en la etapa de prueba conduce necesariamente al rediseño y nueva programación del código afectado, aumentando los costos del desarrollo.
* Una etapa determinada del proyecto no se puede llevar a cabo a menos de que se haya culminado la etapa anterior.

## Toyota production system - 1970

En el centro de todo está el Toyota Production System (TPS). Fue el "paciente cero". Su objetivo era eliminar el desperdicio (muda) y maximizar el valor. Se atribuye fundamentalmente a tres personas: el fundador de Toyota, Sakichi Toyoda, su hijo Kiichiro y el ingeniero Taiichi Ohno, quienes crearon este sistema entre 1946 y 1975.
Cuando los académicos occidentales estudiaron los milagros de Toyota en los años 80, bautizaron esta filosofía como Lean Manufacturing.

El TPS, con su énfasis en la mejora continua y el valor del compromiso de los empleados, es considerado por la industria automotriz como un auténtico benchmark. TPS fue la manera que encontraron los autores de producir "justo a tiempo". Significa producir solo lo necesario, en el momento justo y en la cantidad necesaria. Esto permite que el sistema de producción y de distribución a los concesionarios sea flexible y asegure que cada cliente compre el vehículo de la especificación y color que desea y lo obtenga en el plazo más breve posible. El Just in Time apunta a generar productos de calidad al más bajo costo y de manera más eficiente.

Para ejecutar el Just In Time, el sistema de control visual que se utiliza en las plantas Toyota, es el Kanban. Kanban es un sistema basado en señales. Como su nombre sugiere, Kanban históricamente usa tarjetas para señalar la necesidad de un artículo. Es una manera visual y muy clara de tener una "foto" del estado de la produccion actual.

Informaticos, tras notar que el sistema puede ser utilizado para el desarrollo de software lo implementaron en la industria.

**Principalesp problemas de Toyota**

Aplicar el Toyota Production System (TPS) al desarrollo de software, es una idea fascinante pero lleno de baches conceptuales. El primer gran obstáculo es la invisibilidad del inventario. En una fábrica de coches, si tienes mil puertas acumuladas sin usar, las ves, ocupan espacio y estorban; en el software, el inventario no existe. El proceso de desarrollo de software no se trata de ensamblar partes si no de (no siempre) crearlas. Lo que nos lleva al siguiente punto.

Otro conflicto fundamental surge de la tensión entre estandarización y creatividad. El TPS se basa en la creación de "trabajo estándar" para garantizar la calidad y la eficiencia en tareas repetitivas. Sin embargo, el desarrollo de software es, por definición, un proceso de resolución de problemas únicos; si un problema de software fuera exactamente igual a uno anterior, simplemente copiaríamos el código o usaríamos una librería. Forzar procesos demasiado rígidos o intentar estandarizar el tiempo que un programador tarda en "pensar" una solución innovadora puede ahogar la creatividad y convertir el desarrollo en una línea de montaje de código mediocre que no aporta valor real al usuario.

La gestión de la variabilidad es el tercer gran problema. En la metodología Toyota, se busca minimizar la varianza para que la producción sea fluida y predecible. En el software, la variabilidad es una característica intrínseca, no un defecto: un bug puede tardar diez minutos o tres días en resolverse, y un cambio en los requisitos puede invalidar semanas de arquitectura. Intentar aplicar un sistema de Just-in-Time (JIT) puro puede ser peligroso, ya que si no se gestionan correctamente los márgenes de maniobra, cualquier imprevisto técnico bloquea toda la cadena de valor, generando cuellos de botella que son mucho más difíciles de predecir que en una planta de ensamblaje física.

Finalmente, existe un riesgo interpretativo con el concepto de eliminación de desperdicio (Muda). En una fábrica, eliminar pasos innecesarios es puramente beneficioso, pero en el software, algunas actividades que parecen "desperdicio" a corto plazo son en realidad inversiones de salud a largo plazo. Por ejemplo, la refactorización de código, la documentación técnica o la investigación de nuevas arquitecturas no producen una "pieza final" inmediata, y un enfoque Lean mal entendido podría eliminarlas para maximizar la velocidad de entrega. Esto acaba creando una deuda técnica masiva que, irónicamente, termina deteniendo la "línea de producción" mucho antes de lo previsto, transformando la eficiencia inicial en un colapso total del sistema meses después.

## Dynamic systems development method - 1994

A principios de la década de 1990, el desarrollo rápido de aplicaciones (RAD) se estaba extendiendo por toda la industria de TI. Las interfaces de usuario para aplicaciones de software se estaban moviendo de las viejas pantallas verdes a las interfaces gráficas de usuario que se utilizan hoy en día. Estaban llegando al mercado nuevas herramientas de desarrollo de aplicaciones, como PowerBuilder. Estos permitieron a los desarrolladores compartir sus soluciones propuestas mucho más fácilmente con sus clientes: la creación de prototipos se convirtió en una realidad y las frustraciones de los métodos clásicos de desarrollo secuencial (en cascada) podían dejarse de lado.

DSDM es un enfoque independiente del proveedor que reconoce que más proyectos fracasan debido a problemas de personas que de tecnología. El enfoque de DSDM es ayudar a las personas a trabajar juntas de manera efectiva para alcanzar los objetivos comerciales. DSDM también es independiente de las herramientas y técnicas que permiten su uso en cualquier entorno empresarial y técnico sin vincular el negocio a un proveedor en particular.

Hay ocho principios que sustentan el DSDM. Estos principios dirigen al equipo en la actitud que deben adoptar y la mentalidad que deben adoptar para cumplir de manera consistente.

1. Centrarse en la necesidad del negocio
2. Entregar a tiempo
3. Colaborar
4. Nunca comprometa la calidad
5. Construir de forma incremental a partir de cimientos firmes
6. Desarrollar iterativamente
7. Comunicarse de forma continua y clara
8. Demostrar control

**Principales problemas del metodo "Dynamic systems development"**

El método de desarrollo de sistemas dinámicos, mejor conocido como DSDM, es una de las metodologías ágiles más robustas y completas, pero esa misma "completitud" es la fuente de sus mayores complicaciones. A diferencia de marcos de trabajo más livianos como Scrum, el primer gran problema de DSDM es su alta complejidad y burocracia interna. Al definir una estructura tan detallada de roles, productos de gestión y fases específicas, puede sentirse pesado para equipos pequeños. La carga administrativa de mantener la documentación de los "Fundamentos" y asegurar que cada uno de los trece roles esté correctamente representado puede terminar consumiendo más tiempo en la gestión del proceso que en el desarrollo del código mismo.

Otro obstáculo crítico es la dependencia extrema del compromiso del usuario. DSDM exige que los usuarios finales (como el "Usuario Embajador") estén disponibles y facultados para tomar decisiones de forma casi inmediata. En la realidad corporativa, es extremadamente difícil encontrar expertos de negocio que tengan tanto el conocimiento técnico como el tiempo y la autoridad para estar integrados totalmente en el equipo de desarrollo. Si estos usuarios no están presentes o no se atreven a tomar decisiones vinculantes, el flujo de las iteraciones se detiene, rompiendo la promesa de velocidad y eficiencia que el modelo defiende.

El enfoque de DSDM sobre la priorización mediante el método MoSCoW (Must have, Should have, Could have, Won't have) también presenta desafíos psicológicos y contractuales. Debido a que DSDM fija el tiempo, el costo y la calidad, la única variable que queda para ajustar es el alcance. Esto significa que si el tiempo se agota, las funcionalidades menos críticas simplemente se descartan. Para muchos clientes acostumbrados a modelos tradicionales, la idea de pagar el 100% del presupuesto pero recibir potencialmente solo el 60% de las funciones inicialmente imaginadas es una píldora difícil de tragar, lo que genera tensiones políticas y falta de confianza si no existe una madurez organizativa muy alta.

Finalmente, la curva de aprendizaje y los costos de implementación son barreras significativas. No es una metodología que se pueda improvisar; requiere una formación formal y una mentalidad de diseño evolutivo que choca frontalmente con las culturas de gestión de proyectos que exigen hitos fijos y predictibilidad total. Implementar DSDM en una organización que no está lista para delegar poder a los equipos de desarrollo suele resultar en un híbrido extraño que retiene la rigidez del modelo Waterfall pero bajo la etiqueta de "Ágil", perdiendo los beneficios de ambos mundos y generando una frustración generalizada entre los desarrolladores y los interesados.

## Proceso unificado - 1999

El Proceso Unificado de Desarrollo de Software o simplemente Proceso Unificado es un marco de desarrollo de software que se caracteriza por estar dirigido por casos de uso, centrado en la arquitectura y por ser iterativo e incremental.

El primer libro sobre el tema se denominó, en su versión española, El Proceso Unificado de Desarrollo de Software (ISBN 84-7829-036-2) y fue publicado en 1999 por Ivar Jacobson, Grady Booch y James Rumbaugh, conocidos también por ser los desarrolladores del UML, el Lenguaje Unificado de Modelado. 

El Proceso Unificado es un marco de desarrollo iterativo e incremental compuesto de cuatro fases denominadas Inicio, Elaboración, Construcción y Transición. Cada una de estas fases es a su vez dividida en una serie de iteraciones (la de inicio puede incluir varias iteraciones en proyectos grandes). Estas iteraciones ofrecen como resultado un incremento del producto desarrollado que añade o mejora las funcionalidades del sistema en desarrollo.

Cada una de estas iteraciones se divide a su vez en una serie de disciplinas que recuerdan a las definidas en el ciclo de vida clásico o en cascada: Análisis de requisitos, Diseño, Implementación y Prueba. Aunque todas las iteraciones suelen incluir trabajo en casi todas las disciplinas, el grado de esfuerzo dentro de cada una de ellas varía a lo largo del proyecto.

El Proceso Unificado requiere que el equipo del proyecto se centre en identificar los riesgos críticos en una etapa temprana del ciclo de vida. Los resultados de cada iteración, en especial los de la fase de Elaboración deben ser seleccionados en un orden que asegure que los riesgos principales son considerados primero.

**Principales problemas del UP (proceso unidicado)**

El Unified Process (UP), aunque nació con la intención de ser un marco de trabajo iterativo y centrado en la arquitectura, arrastra una complejidad estructural que suele abrumar a los equipos modernos. El primer gran escollo es que se percibe como una metodología "pesada" debido a la enorme cantidad de artefactos, roles y flujos de trabajo que propone. Si un equipo intenta seguir el UP al pie de la letra sin una personalización extrema, corre el riesgo de caer en la "parálisis por análisis", dedicando más esfuerzo a generar diagramas de casos de uso y documentos de visión que a producir software funcional que aporte valor real.

Otro problema fundamental es la dificultad para equilibrar sus fases con la agilidad. Aunque el UP se divide en Incepción, Elaboración, Construcción y Transición, muchas organizaciones interpretan estas etapas de forma lineal, convirtiéndolo en un "Waterfall disfrazado". Especialmente la fase de Elaboración, donde se busca mitigar riesgos y definir la arquitectura, puede extenderse indefinidamente si el equipo tiene miedo a avanzar sin tener todas las respuestas técnicas. Esto retrasa la entrega de código ejecutable y crea una falsa sensación de seguridad basada en modelos teóricos que podrían no sobrevivir al contacto con la implementación real.

La curva de aprendizaje es también una barrera significativa. Dominar el Unified Process requiere un conocimiento profundo de UML (Unified Modeling Language) y de una terminología técnica muy específica que no siempre es accesible para todos los interesados del proyecto. Esta brecha de lenguaje puede aislar a los desarrolladores de los clientes de negocio, quienes a menudo se sienten intimidados por la formalidad del proceso. Además, la gestión de un proyecto bajo UP exige herramientas de software especializadas y costosas para mantener la trazabilidad de todos los modelos, lo que añade una carga financiera y logística que muchas veces no se justifica en proyectos de tamaño medio o pequeño.

Finalmente, el UP tiende a fomentar una cultura de especialización rígida que choca con la tendencia actual de equipos multidisciplinarios. Al definir roles tan específicos como "analista de sistemas", "diseñador de interfaz" o "arquitecto de software", se pueden crear silos de información donde la responsabilidad se diluye entre departamentos. Esto dificulta la comunicación fluida y la capacidad de respuesta rápida ante cambios inesperados, ya que cualquier modificación suele requerir la actualización de múltiples documentos interconectados antes de poder tocar el código, lo que resta competitividad en entornos de mercado altamente volátiles.


## Agile - 2001

El desarrollo ágil de software es un término general para los enfoques para desarrollar software que reflejan los valores y principios acordados por The Agile Alliance, un grupo de 17 profesionales del software, en 2001. Como se documenta en su Manifiesto para el Desarrollo de Software Ágil, los profesionales valoran:

* Individuos e interacciones sobre procesos y herramientas
* Software de trabajo sobre documentación completa
* Colaboración con el cliente sobre la negociación del contrato
* Responder al cambio sobre seguir un plan

Los profesionales citan la inspiración de las nuevas prácticas en ese momento, incluyendo la programación extrema, el scrum, el método de desarrollo de sistemas dinámicos, el desarrollo de software adaptativo y la simpatía con la necesidad de una alternativa a los procesos de desarrollo de software pesados basados en la documentación.

Muchas prácticas de desarrollo de software surgieron de la mentalidad ágil. Estas prácticas basadas en la agilidad, a veces llamadas ágiles, incluir requisitos, descubrimiento y mejora de soluciones a través del esfuerzo colaborativo de equipos autoorganizados y multifuncionales con sus clientes/usuarios finales.

Si bien hay mucha evidencia anecdótica de que la mentalidad ágil y las prácticas basadas en la agilidad mejoran el proceso de desarrollo de software, la evidencia empírica es limitada y menos que concluyente.

**Principales problemas de Agile**

Aunque Agile nació como la solución a la rigidez de los modelos tradicionales, su aplicación en el mundo real ha revelado grietas profundas que suelen frustrar tanto a desarrolladores como a directivos. El primer gran obstáculo es la falta de predictibilidad a largo plazo. Debido a que Agile se centra en iteraciones cortas y en reaccionar al cambio, a las organizaciones les resulta extremadamente difícil responder a preguntas básicas como cuánto costará el proyecto total o en qué fecha exacta estará terminado. Esta incertidumbre choca frontalmente con los departamentos financieros y de ventas, que necesitan presupuestos cerrados y hojas de ruta fijas para planificar sus estrategias anuales.

Otro problema crítico es el fenómeno conocido como "Agile de fachada" o Dark Agile, donde las empresas adoptan las ceremonias (como el Daily Stand-up o el uso de tableros Kanban) pero mantienen una mentalidad autoritaria y rígida. En estos entornos, la agilidad se convierte en una herramienta de microgestión donde se presiona al equipo para entregar más rápido en cada sprint, ignorando la sostenibilidad del ritmo de trabajo. Esto degenera rápidamente en el agotamiento de los desarrolladores y en una caída estrepitosa de la calidad del código, ya que el equipo sacrifica la excelencia técnica para cumplir con métricas de velocidad artificiales.

La falta de documentación técnica y de arquitectura es una queja constante en proyectos ágiles mal ejecutados. Bajo el lema de "software funcionando sobre documentación exhaustiva", muchos equipos descuidan la creación de guías esenciales para el mantenimiento futuro del sistema. Esto crea un caos a largo plazo cuando los miembros originales del equipo se marchan y los nuevos integrantes se encuentran con un laberinto de código sin mapas ni brújulas. Además, sin una fase de diseño arquitectónico sólido al inicio, el sistema puede crecer de forma desordenada, obligando a realizar refactorizaciones constantes y costosas que frenan el avance del proyecto en etapas avanzadas.

Por ultimo, Agile requiere un nivel de compromiso y madurez del cliente que rara vez se encuentra de forma espontánea. El modelo exige que el "Product Owner" o el cliente esté disponible constantemente para aclarar dudas y validar incrementos de software. Si el cliente no tiene tiempo o no tiene la autoridad para tomar decisiones rápidas, el equipo se queda bloqueado o avanza basándose en suposiciones que luego resultan ser erróneas. Esta dependencia humana hace que el éxito de Agile sea muy frágil, ya que no depende solo de la destreza técnica del equipo, sino de la cultura y la disposición de toda la estructura organizativa para trabajar de una manera radicalmente distinta.

## Lo que tenemos hasta aca

Secuenciales: Waterfall
Iterativas: RUP, desarrollo de sistemas dinámicos
Agiles: XP, Scrum, Kanban

XP no es un framework de produccion de software, sino que fue creado como "software-development discipline that organizes people to produce higher-quality software more productively". Son un conjunto de disciplinas (todas validas) para producir codigo de mayor calidad.

Waterfall va por un lado, de manera secuencial y no es agile. Mientras que todos los demas forman una rama aparte de las llaamdas "metodologias agiles". Todas las metodologias agiles son iterativas, pero no todas las metodologias iterativas son agiles.

Las metodologias de trabajo nacen de los problemas que tienen otras metodologias anteriiores y ninguna es perfecta. 

> Nota: Muchos sistemas como el espiral o el v-model quedaron afuera de este estudio.

[graph-001](/assets/graph-001.svg)

Lo que planteamos en este libro es que el manual de las metodologias agiles todavia no termino de escribirse. Agile todavia deja sin resolver un monton de problemas que muchos desarrolladores en todo el mundo tienen cada dia.

---


* In 2012 the [disciplined agile delivery framework](https://en.wikipedia.org/wiki/Disciplined_agile_delivery) was released, a hybrid framework that adopts and extends strategies from unified process, scrum, extreme programming, and other methods.

https://es.wikipedia.org/wiki/Top-down_y_bottom-up <- Lectura ESCENCIAL. Biblia.
https://en.wikipedia.org/wiki/Toyota_Production_System
https://en.wikipedia.org/wiki/Lean_software_development
https://en.wikipedia.org/wiki/Barry_Boehm
https://es.wikipedia.org/wiki/Desarrollo_en_cascada
https://en.wikipedia.org/wiki/Extreme_programming
https://en.wikipedia.org/wiki/Software_development_process
https://medium.com/@tjmaher1/what-was-software-development-like-before-waterfall-cd344c79956a
https://javiergarzas.com/2012/04/agilistas-influyentes.html <- Excelente
https://www.amazon.es/gp/product/0321413091/ref=as_li_tf_tl?ie=UTF8&tag=wwwjaviergarz-21&linkCode=as2&camp=3626&creative=24790&creativeASIN=0321413091
https://en.wikipedia.org/wiki/Disciplined_agile_delivery
https://it.wikipedia.org/wiki/Modello_di_sviluppo_del_software
https://en.wikipedia.org/wiki/Dynamic_systems_development_method
* Software Engineering Economics (paper) 1983 - Barry W. Boehm
https://www.amazon.com/DSDM-Dynamic-Systems-Development-Practice/dp/0201178893#:~:text=About%20the%20Author,satisfaction%20for%20the%20end%2Duser.

Libro DSDM: Dynamic Systems Development Method: The Method in Practice, by Jennifer Stapleton (1997) 9 euros es amazon 163 paginas

https://www.amazon.com/Software-Engineering-Economics-Barry-Boehm/dp/0138221227

Software Engineering Economics 1st Edition by Barry W. Boehm (Author) 42 euros. 767 pages


Una gran diferencia entre las metodologías es el grado en que las fases son secuenciales frente a iterativas. Las metodologías ágiles, como XP y scrum, se centran en procesos ligeros que permiten cambios rápidos.[5] Las metodologías iterativas, como el Proceso Unificado Racional y el método de desarrollo de sistemas dinámicos, se centran en estabilizar el alcance del proyecto y expandir o mejorar iterativamente los productos. Los modelos secuenciales o de gran diseño por adelantado (BDUF), como la cascada, se centran en una planificación completa y correcta para guiar proyectos más grandes y limitar los riesgos a resultados exitosos y predecibles.[6] El desarrollo anamórfico se guía por el alcance del proyecto y las iteraciones adaptativas. En scrum,[7]por ejemplo, se podría decir que una historia de un solo usuario pasa por todas las fases del SDLC dentro de un sprint de dos semanas. Por el contrario, la metodología de cascada, donde todos los requisitos comerciales[Cita requerida] se traduce en descripciones de características/funcionales que luego se implementan típicamente durante un período de meses o más.[Cita requerida]


* **Waterfall** (1956 - Herbert D. Benington - Secuencial)
* **Toyota Production System** (1970 - Toyota)
* **Dynamic systems development method** (1994 - Jennifer Stapleton -Iterative)
* **UP (Unified Process)** - (1999) The Unified Software Development Process (ISBN 0-201-57169-2) and published in 1999 by Ivar Jacobson, Grady Booch and James Rumbaugh.
* **Agile** (2001) el Manifiesto Ágil, firmado por Kent Beck, Mike Beedle, Arie van Bennekum, Alistair Cockburn, Ward Cunningham, Martin Fowler, James Grenning, Jim Highsmith, Andrew Hunt, Ron Jeffries, Jon Kern, Brian Marick, Robert C. Martin, Steve Mellor, Ken Schwaber, Jeff Sutherland y Dave Thomas,
* **disciplined agile delivery framework** (2012 -Scott Ambler and Mark Lines- Agile)

[Continuar leyendo](003-contexto-actualmd)

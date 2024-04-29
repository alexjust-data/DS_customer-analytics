#### Introducción:

1) Los sistemas de recomendación pretenden emular en un canal en línea de comercio electrónico, el papel que ejerce un vendedor experto en un local comercial físico con sus sugerencias apropiadas al perfil del cliente. Con ello, el sistema de recomendación cumple dos objetivos de negocio:
   1) fidelizar al cliente mejorando la experiencia de compra, y
   2) aumentar el flujo de ventas.
<br>
2) Técnicamente, podemos considerar el sistema de recomendación como un sistema de filtrado de información, basado en filtrar y estructurar datos de productos y clientes y en hacer el correspondiente matching. Según la situación y la disponibilidad de datos, el sistema puede estar basado principalmente o bien en datos del cliente, o bien en datos de los productos. Los sistemas más avanzados son generalmente híbridos entre ambas opciones.
<br>
3) En muchos de estos sistemas de recomendación se usan métricas de dis- tancia para calcular la similitud entre clientes, y después se aplica un algorit- mo de vecindad para calcular el cliente más próximo.


#### Contexto de negocio

La oferta de productos a través de internet es cada vez más diversa. Las plataformas de venta de comercio electrónico, algunas de ellas, empezaron vendiendo productos de mercados muy específicos, libros o componentes informáticos, por ejemplo. Pero hoy en día han integrado horizontalmente multitud de mercados en su oferta, ofreciendo libros, componentes informáticos, electrodomésticos, productos no perecederos y, más recientemente, incluso perecederos, como en el caso del líder digital en distribución, Amazon.

Este hecho ha provocado que sea imposible para un consumidor habitual en- contrar los productos que necesita mediante búsquedas por menú. En su lu- gar, para optimizar el proceso de compra y minimizar el tiempo que el usua- rio necesita hasta que encuentra lo que busca, las empresas han optado por incorporar recomendadores de productos digitales. Estos algoritmos pretenden sustituir el rol clásico del vendedor físico en las tiendas, en lo que atañe a formular sugerencias según el perfil del cliente. Este vendedor asume, en el canal físico, el papel de acelerar las compras, incidiendo positivamente en la satisfacción de los clientes de las tiendas tradicionales. Su función es la de recomendar o encontrar los productos más interesantes para los compradores que acuden a sus tiendas sin tener claro lo que buscan. Del mismo modo, los algoritmos de recomendación buscan automatizar estas funciones ofreciendo un conjunto de posibilidades reducido: una selección de productos que pue- dan llegar a resultar verdaderamente interesantes para los internautas que acceden a la tienda en línea. Estos procesos cubren, de esta forma, dos necesida- des interesantes para el vendedor:

* en primer lugar, se consigue fidelizar a los clientes mediante un servicio que les asesora de forma rápida y a menudo eficaz, y
<br>
* en segundo lugar, se incrementa el número de ventas gracias a la aceleración del proceso de compraventa.
Como es de esperar, este tipo de sistema se ha convertido en un factor determinante para llevar a una plataforma en línea a convertirse en líder del mer- cado. Las distribuidoras tradicionales, viendo el éxito obtenido por sus competidores de venta en línea, optan en la actualidad por adoptarlos también y perfeccionarlos. Viendo la demanda, las propias empresas en línea empiezan a ofrecer servicios de consultoría en este tipo de proyectos.
<br>

    > Amazon, por ejemplo, ofrece servicios de consultoría para implementar sistemas de recomendación en empresas de todo tipo, aprovechando su saber hacer y creando también sinergias que le permitan implantar en paralelo otros tipos de servicios que también les ofrecen cuantiosas ganancias, como las plataformas nube y las herramientas autoML como Sagemaker.

#### Qué es un sistema de recomendación

Son métodos que emplean filtrado y tabulación de datos históricos para encontrar similitudes entre usuarios con perfiles de compra similares y productos no coincidentes entre ellos, que servirán como recomendaciones.

##### Aplicaciones

Estos sistemas suelen utilizarse para recomendar productos tangibles, pero hay muchos tipos de aplicaciones en otros mercados, como las plataformas de mú- sica, los juegos de ordenador, los vídeos en streaming, los sitios web de citas, etc. Pueden emplearse en cualquier tipo de escenarios donde el consumidor pueda elegir entre un conjunto grande de opciones.

> Las principales aplicaciones podríamos clasificarlas en fidelización, generación de ventas adicionales y ayuda al usuario en el proceso de decisión.

La empresa fideliza mejorando la experiencia de compra si el consumidor encuentra habitualmente lo que busca y se minimiza la probabilidad de que este recurra a la competencia. Genera ventas adicionales porque se recomiendan productos que el cliente no buscaba de manera activa pero que al verlos percibe que podrían interesarle y los compra sin haber tenido una necesidad previa a la visita. Ayudan al usuario porque le ahorran tiempo y en ocasiones dinero poniendo a su alcance de manera eficiente lo que necesita.


#### Tipos de sistema según filtro

Podemos subdividir los tipos de sistemas de recomendación en los siguientes dos grandes grupos:

* **Sistemas de recomendación de filtros colaborativos basados en clientes**: estos sistemas utilizan el histórico de compras y opiniones de la ba- se de datos de clientes y, basándose en las características de sus hábitos de consumo y opinión, buscan similitudes y diferencias respecto a otros clientes para recomendar productos de interés.
<br>
* **Sistemas de recomendación basados en contenidos**: estos parten de las características de los productos y sobre la base de estas encuentran pro- ductos de interés para determinados consumidores.

Los segundos se basan en características de los productos y en encontrar sus similitudes, autor, temática, público objetivo, etc., para así ofrecer productos similares a los que un cliente ha comprado previamente. En estos sistemas se puede prescindir del histórico de compras del consumidor y serían útiles para recomendaciones a nuevos clientes. Los primeros sistemas son adecuados para recomendaciones a clientes de los que disponemos de registros de compras que se remontan mucho en el tiempo (clientes habituales) y también en situaciones en las que no se dispone de calidad en los datos referidos a las características de los productos.
A partir de estos dos grandes grupos también encontramos otros sistemas híbridos que combinan ambas dimensiones para encontrar ránquines de pro- ductos o productos específicos, con el propósito de recomendar tanto a con- sumidores habituales como a nuevos consumidores.

Más recientemente también encontramos en la literatura sistemas de recomendación basados en descomposición matricial y redes neuronales.

* Entre los primeros encontramos los de **descomposición matricial U V**, que calculan la matriz de utilidad y permiten obtener una escala de valores de todos los clientes de manera relativamente rápida.
<br>
* El segundo tipo son los basados en redes neuronales, que consiguen obtener un ranquin de puntuaciones para cada cliente basados en la **función softmax**, que se encuentra en la última capa de un modelo de predicción con redes neuronales. Estos ránquines permiten distinguir clientes o productos afines sobre la base del histórico de compras de cada usuario.

Ambos casos se emplean en las mismas condiciones y tienen la misma finalidad que los métodos más tradicionales, pero suelen proporcionar resultados más acertados.

También podemos subdividir los sistemas de recomendación en función del tipo de personalización:
* **No personalizados**: siempre ofrecen el mismo resultado. Basados en listas, datos estadísticos, etc.
* **De personalización actual**: ofrecen un resultado según la información del momento o la sesión de navegación actual del usuario.
* **De personalización persistente**: utilizan el perfil del usuario.
  
Los sistemas de recomendación necesitan entradas y salidas, el método usado para generar la recomendación y el grado de personalización. Para poder ofrecer las recomendaciones, los sistemas pueden recolectar la in- formación de diferentes maneras, tales como preguntas directas al usuario, la recogida de información de su navegación, el histórico de productos adquiri- dos o los sistemas de valoración por puntos.

#### Instrumentos relacionados: métricas y algoritmos

Dos instrumentos clave para muchos sistemas de recomendación:

1. Las métricas para hallar el grado de similitud entre clientes y
2. los algoritmos para hallar el cliente más próximo.

##### Métricas de agregación y distancia

La mayoría de los sistemas de recomendación se basan en encontrar las simi- litudes y diferencias entre los clientes en lo que respecta a sus hábitos de consumo. Por tanto, es esencial para este tipo de técnica definir de manera óptima cuál será la expresión matemática ideal para ese concepto de similitud. En la literatura encontramos diferentes opciones en lo que respecta a métricas de agregación basadas en distancias. La distancia es un concepto muy próximo al de la similitud. Lo mismo podríamos decir, por ejemplo, de la independencia o dependencia y la correlación. En este sentido se definen una serie de métricas de agregación que según el problema son más o menos convenientes. A continuación, definiremos algunas de las más conocidas:

1. **Distancia euclídea**: se basa en la expresión matemática de la recta que separa a dos puntos. Su expresión matemática es la siguiente:
   
   $$\text{dist}(X, Y) = \sqrt{\sum_{i=1}^{n} (x_i - y_i)^2}$$

2. **Distancia de Minkowski:**
   Es una generalización de la anterior también conocida como distancia de regularización LR. En función del valor que tome el parámetro $P$ la expresión coincidirá con la distancia euclidiana ($P = 2$), la distancia de Manhattan ($P = 1$) o la distancia maximal ($P = \infty$):

   $$\text{dist}(X, Y) = \left( \sum_{i=1}^{n} |x_i - y_i|^P \right)^{\frac{1}{P}}$$

3. **Distancia de Hamming:**
   La distancia entre el usuario A y el usuario B es el número de componentes en los que ambos se diferencian. Se utiliza con componentes binarios. Solo resulta útil en situaciones donde la información es completa, algo que no siempre sucede.
$$\text{dist}(X, Y) = \begin{cases} 
   0 & \text{si } x = y \\
   1 & \text{si } x \neq y 
   \end{cases}$$

   Donde $\text{dist}(X, Y)$ es la suma del número de posiciones en las que los correspondientes símbolos son diferentes.
<br>

4. **Distancia de Coseno:**
   $d \in [0,180]$ La similitud entre dos clientes se mide por el ángulo que forman. Los ángulos grandes indican menor similitud, mientras que los ángulos cercanos a cero indican mayor similitud. La similitud puede darse incluso en vectores distintos; solo es necesario que tengan la misma dirección. Es una distancia útil en situaciones donde la información no es completa.

   $$\text{dist}(X, Y) = 1 - \cos(X, Y) = 1 - \frac{\sum_{i=0}^{n-1} x_iy_i}{\sqrt{\sum_{i=0}^{n-1} (x_i)^2} \sqrt{\sum_{i=0}^{n-1} (y_i)^2}}$$

5. **Distancia de Jaccard:**
   Es un tipo de distancia que se utiliza con datos binarios. En general, los conteos pueden transformarse en datos binarios, por ejemplo, haber comprado más de cero productos puede tomar el valor 1; tomaría el valor 0 en caso contrario. La distancia entre el usuario A y el usuario B es:

   $$J_{\text{dist}}(X, Y) = 1 - J_{\text{index}}(X, Y) = 1 - \frac{X \cap Y}{X \cup Y}$$


##### Búsqueda del vecino más próximo

En los métodos más tradicionales, tras encontrar la métrica de distancia óptima para cada caso, el investigador posteriormente suele emplear algoritmos de búsqueda de vecino más próximo, partiendo de las matrices de distancias obtenidas en el punto anterior.

Básicamente, este tipo de algoritmos busca en la matriz de distancias aquellos individuos con distancia mínima basándose dichas distancias en las similitudes que presentan en sus hábitos de compra. O, dicho de otro modo, basándose en las similitudes entre los productos que hayan comprado en el pasado. Una vez localizado el individuo más similar, se buscan aquellos productos que no tengan en común, que serán aquellos que el sistema acabará recomendando.

El algoritmo más habitual es el K-nearest neighbor (KNN), que veremos con más detalle en otros materiales de la asignatura.
# IA class notes

## Agentes de IA

Existen diferentes tipos de agentes, desde agentes basados en un sistema de reglas predefinidas hasta agentes impulsados por LLM, los cuales aprenden, se adaptan y mejoran con el tiempo.
Estos se clasifican en función de su nivel de "inteligencia", proceso de toma de decisiones y cómo interactuan con su entorno para alcanzar resultados deseados.

Diferentes tipos de agentes:

Agentes según sus caracteristicas:
- Determinista, estático, observable, discreto
    - S = f(a)
    - S = (s<sub>1</sub>, ..., s<sub>n</n>) ∈ D<sub>1</sub> x ... x D<sub>n</sub> = S
    - a∈A, a∈A(s) acciones legales en s.
    - Dado un conjunto de reglas predefinidas (reglas de condición-acción), toma decisiones sin considerar experiencias pasadas o consecuencias futuras.
 
- Determinista, dinámico, observable, discreto
    - S<sub>k+1</sub> = f(S<sub>k</sub>, a<sub>k</sub>)
    - En este tipo de agente, el entorno va cambiando, por lo cual, se necesita la noción del estado en el que se encuentra y la acción que se realizo para poder llegar a un nuevo estado.

- Determinista, dinámico, parcialmente observable, discreto
    - S<sub>k+1</sub> = f(S<sub>k</sub>, a<sub>k</sub>)
    - P<sub>k</sub> = g(S<sub>k</sub>)
    - En este tipo de agebte, es necesario mantener un modelo interno del estado del entorno, ya que el estado real no es completamente observable. El agente utiliza el estado previo, la acción realizada y la percepción actual para estimar el nuevo estado y así poder tomar decisiones correctas.

- Determinista, dinámico, observable / parcialmente observable, continuo.
    - ẋ<sub>t</sub> = f(x<sub>t</sub>, a<sub>t</sub>)
    - P<sub>t</sub> = g(x<sub>t</sub>)
    - En este tipo de agente, al tener un entorno dinámico y continuo que esta en constante cambio con respecto al tiempo, se modela mediante ecuaciones diferenciales, cuando el entorno es parcialmente observable, el agente recibe percepciones como funciones del estado real, por lo que debe mantener y actualizar una estimación del estado interno para seleccionar acciones que permitan alcanzar objetivos o maximizar una función de utilidad.

- Estocástico, discreto, estático, observable
$$
A =
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{pmatrix}
$$



<!--- 
    prueba
    Agentes reflejo simple
    - Este tipo de agente debe ser completamente observable.
        - Determinista, estatico, observable, discreto.
        - S = f(a)
        - S = (s<sub>1</sub>, ..., s<sub>n</n>) ∈ D<sub>1</sub> * ... * D<sub>n</sub> = S
        - a∈A, a∈A(s) acciones legales en s.
        - Dado un conjunto de reglas predefinidas (reglas de condición-acción), toma decisiones sin considerar experiencias pasadas o consecuencias futuras.

        Ejemplo de este tipo de agente:
        - Un termostato
            - Enciende la calefacción si la temperatura desciende por debajo de un determinado umbral y la apaga si se alcanza la temperatura deseada.
        - Un semáforo
            - Cambia las señales en función de las entradas de los sensores de tráfico, sin recordar estados anteriores.

    Este tipo de agente 
- Agentes reflejo basados en modelos
    - A diferencia de un agente reflejo simple, este tipo mantiene un modelo interno del entorno, que le permite rastrear un estado estimado y predecir cambios futuros. Esto le permite tomar decisiones más inteligentes cuando el entorno no es completamente observable.    
    - S<sub>k+1</sub> = f(S<sub>k</sub>, a<sub>k</sub>)
    - P<sub>k</sub> = g(S<sub>k</sub>)
    - Esta capacidad de mantener un estado interno permite que el agente funcione efectivamente en entornos parcialmente observables.

    Ejemplo de este tipo de agente:
    - Un robot que navega por una habitación
        - No solo reacciona a los obstáculos inmediatos, sino que también tendria en cuenta sus movimientos previos y las ubicaciones de los obstáculos que ya ha pasado.
-->

# IA class notes

## Agentes de IA

Existen diferentes tipos de agentes, desde agentes basados en un sistema de reglas predefinidas hasta agentes impulsados por LLM, los cuales aprenden, se adaptan y mejoran con el tiempo.
Estos se clasifican en función de su nivel de "inteligencia", proceso de toma de decisiones y cómo interactian con su entorno para alcanzar resultados deseados.
Existen 5 tipos principales de agentes:

- Agentes reflejo simple
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

- Agentes reflejo basados en modelos
    -


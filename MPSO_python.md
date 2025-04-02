# MPSO migrado al lenguaje de programación Python

### Índice
- [PSO_simulacion_original_python.wbt](#pso_simulacion_original_pythonwbt)

El método implementado para la paralelización en Python fue el de hilos (threads). Un hilo representa una secuencia de instrucciones que el procesador (CPU) ejecuta dentro de un programa o aplicación. Cuantos más hilos pueda manejar el CPU, más tareas se podrán ejecutar. Esta técnica mejora el rendimiento al permitir que múltiples hilos se ejecuten simultáneamente en uno o varios núcleos (cores) del procesador, lo que aumenta la velocidad y eficiencia del sistema.

## PSO_simulacion_original_python.wbt
Este mundo contiene la simulación del algoritmo MPSO migrado al lenguaje de Python, con el fin de poder comparar el rendimiento del algoritmo vectorizado. Además, contiene la simulación del algoritmo MPSO migrado a Python implementando paralelización.

**Experimento 1: Funciónd de costo Schaffer con MPSO migrado a Python.**
<br><div align="center">
    <img src="Figuras/mpso_py_schaffer.gif" width="750" height="auto" alt="Experimento con función de costo Schaffer y MPSO migrado a Python"><br>
</div>

**Experimento 2: Funciónd de costo Schaffer con MPSO migrado a Python implementando paralelización.**
<br><div align="center">
    <img src="Figuras/mpso_py_paral_schaffer.gif" width="750" height="auto" alt="Experimento con función de costo Schaffer y MPSO migrado a Python implementando paralelización"><br>
</div>

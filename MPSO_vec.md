# MPSO modificado
### Índice
- [MPSO_modified](#mpso_modified)
- [PSO_simulacion_4.wbt](#pso_simulacion_4wbt)

La vectorización consiste en optimizar operaciones, como los bucles for, mediante el uso de operaciones matriciales y vectoriales, tales como suma, resta, funciones trigonométricas (seno, coseno), operaciones de algebra lineal (cálculo de norma), entre otras. Esta técnica permite realizar dichas operaciones de manera simultánea sobre un conjunto de valores organizados en forma de vector o matriz.

Para mejorar el rendimiento del algoritmo se implementó el método de vectorización en el cálculo de las funciones de costo, parámetro de inercia del PSO y el controlador PID.

### MPSO_modified
El script **MPSO_modified** presenta el algoritmo MPSO vectorizado. Se utilizaron las funciones de costo Sphere, Booth y Schaffer y se midió el tiempo de convergencia de los agentes robóticos pololu 3pi+.

### Experimento con función Booth vectorizada
<br><div align="center">
    <img src="Figuras/booth_fitness_1.gif" width="700" height="auto" alt="Experimento función Booth vectorizada"><br>
</div>

### Experimento con factor de inercia vectorizado 
<br><div align="center">
    <img src="Figuras/boot_inercia.gif" width="700" height="auto" alt="Experimento parámetro de inercia vectorizado"><br>
</div>

### Experimento con controlador PID vectorizado
<br><div align="center">
    <img src="Figuras/sphere_pid.gif" width="700" height="auto" alt="Experimento función Booth vectorizada"><br>
</div>


## Webots 
### PSO_simulacion_4.wbt
Este mundo contiene la simulación del algoritmo MPSO implementando vectorización en el cálculo de la función de costo, el factor de inercia y el controlador PID.

<br><div align="center">
    <img src="Figuras/sphere_pid.gif" width="700" height="auto" alt="Experimento función Sphere con controlador PID vectorizado"><br>
</div>


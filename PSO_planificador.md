# PSO como planificador de trayectorias 

### Índice
- [PSO_APF_planificador.m](#pso_apf_planificadorm)
- [PSO_simulacion_planificador.wbt](#pso_simulacion_planificadorwbt)

## PSO_APF_planificador.m
Este script presenta la implementación del algoritmo PSO como planificador de trayectorias utilizando campos potenciales artificiales. Es importante mencionar que este planificador cálcula de primero las trayectorias libres de obstáculos para luego poder implementarlas en los agentes robóticos pololu 3pi+.

**Experimento 1: Un obstáculo rectangular**
<br><div align="center">
    <img src="Figuras/pso_planificador_1.gif" width="600" height="auto" alt="Experimento con un obstáculo rectangular"><br>
</div>

**Experimento 2: Dos obstáculos rectangulares**
<br><div align="center">
    <img src="Figuras/pso_planificador_2.gif" width="600" height="auto" alt="Experimento con dos obstáculos rectangulares"><br>
</div>

**Experimento 3: Tres obstáculos rectangulares**
<br><div align="center">
    <img src="Figuras/pso_planificador_3.gif" width="600" height="auto" alt="Experimento con tres obstáculos rectangulares"><br>
</div>

**Experimento 4: Cuatro obstáculos rectangulares**
<br><div align="center">
    <img src="Figuras/pso_planificador_4.gif" width="600" height="auto" alt="Experimento con cuatro obstáculos rectangulares"><br>
</div>

**Experimento 5: Seis obstáculos rectangulares**
<br><div align="center">
    <img src="Figuras/pso_planificador_5.gif" width="600" height="auto" alt="Experimento con seis obstáculos rectangulares"><br>
</div>

## PSO_simulacion_planificador.wbt
En este mundo se implementan las trayectorias encontradas por el planificador por medio de un seguimiento de trayectoria utilizando un controlador PID y los agentes robóticos pololu 3pi+ en el entorno de simulación Webots.

**Experimento 1: Trayectorias encontradas por el planificador con un obstáculo rectangular**
<br><div align="center">
    <img src="Figuras/pso_planificador_1_wb.gif" width="600" height="auto" alt="Experimento con un obstáculo rectangular"><br>
</div>


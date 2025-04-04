# _Modified Particle Swarm Optimization_ (MPSO)
### Experimento función optimización Schaffer 4 con el MPSO original
<br><div align="center">
    <img src="Figuras/schaffer_4.gif" width="700" height="auto" alt="Experimento función Schaffer 4"><br>
</div>

### Índice
- [MPSO_pololu_original](#mpso_pololu_original)
- [MPSO_simulado](#mpso_simulado)
- [PSO_simulacion_original.wbt](#pso_simulacion_originalwbt)

### MPSO_pololu_original
El script **MPSO_pololu_original** contiene la implementación física del algoritmo de optimización _Particle Swarm Optimization_ (PSO) utilizando los robots diferenciales Pololu 3pi+ dentro del ecosistema Robotat. Este código se divide en tres partes: conexión al Robotat y a los robots pololu 3pi+, cálculo del algoritmo PSO y controlador PID.

Para establecer la conexión al Robotat es necesario conectarse a la red llamada _Robotat_. Luego, se utiliza la función _robotat_connect_(), que permite crear un objeto TCP con una IP y puerto específicos. Una vez establecida la conexión con el Robotat, se procede a conectar los robots pololu 3pi+, cada robot posee un número de identificación (ID). Es importante mencionar que en este script deben usarse los robots con IDs consecutivos por ejemplo: pololu 2, pololu 3 y pololu 4.

Para conectar los robots pololu 3pi+, se utiliza la función _robotat_3pi_connect_(), la cual recibe como argumento el ID de cada robot.

**Modificaciones realizadas al MPSO**
Se realizaron ajustes al algoritmo MPSO, debido que en las primeras pruebas los agentes no lograban llegar a la meta. Las modificaciones incluyeron ajustes en el controlador PID y la incorporación de un radio de convergencia.

- **Controlador PID**
    - Distancia entre ruedas: Se consideró la distancia entre las ruedas desde el punto de instalación.
    
    <br><div align="center">
        <img src="Figuras/pololu_wheel.png" alt="Distancia entre ruedas Pololu 3pi+" width="250"><br>
    </div>

    - Ángulo de rotación: Hace que el offset entre el eje del marker y el eje x+ del robot diferencial sea 0, alineando ambos ejes. Los ángulos de rotación se utilizan en grados.
    (imagen)
- **Radio de convergencia**
    Se definió este radio para medir si los agentes logran llegar a un área cercana a la meta. Si el radio es menor al radio máximo se considera que está dentro del área de convergencia y se detiene el algoritmo.

  <br><div align="center">
        <img src="Figuras/radio_convergencia.png" width="300" height="auto" alt="Radio de convergencia"><br>
    </div>
    

### MPSO_simulado
El script **MPSO_simulado** presenta la simulación del algoritmo MPSO con cantidad de partículas modificable y permite definir el objetivo del enjambre sin utilizar funciones de costo.

**Experimento función de optimización hacia una meta en específico**
<br><div align="center">
    <img src="Figuras/PSO_simulado.gif" width="400" height="auto" alt="Experimento función Schaffer 4"><br>
</div>

## Webots 
### PSO_simulacion_original.wbt 
Este mundo contiene la simulación del algoritmo MPSO original utilizando el entorno _Webots_. Esta simulación permitió validar los experimentos y algoritmos implementados.

**Experimento función de costo Schaffer**
<br><div align="center">
    <img src="Figuras/PSO_webots.gif" width="600" height="auto" alt="Experimento función Schaffer 4"><br>
</div>


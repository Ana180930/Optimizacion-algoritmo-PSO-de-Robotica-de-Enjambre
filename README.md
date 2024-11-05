# Optimización del algoritmo de robótica de enjambre *Particle Swarm Optimization* para su implementación con agentes robóticos físicos en escenarios con obstáculos en el ecosistema Robotat 
A continuación, se muestra una guía de como utilizar el algoritmo MPSO modificado, con campos potenciales artificiales para la evasión de obstáculos en el ecosistema Robotat. Y las modificaciones que se realizaron para la optimización del mismo.

## Tabla de Contenidos
- [Videos demostrativos](#videos-demostrativos)
- [Códigos y guía de uso](#códigos_y_guía_de_uso)
- [Software y hardware](#software-y-hardware)
- [Información adicional](#información-adicional)

## Videos demostrativos
Al darle click a la imagen podrás ver una lista de videos sobre los experimentos realizados en la optimización del algoritmo MPSO y el funcionamiento del algoritmo PSO con campos potenciales artifiales para la evasión de obstáculos.

## Códigos y guía de uso
En la carpeta *Códigos* en OneDrive se encuentran los códigos principales que se utilizaron en esta tesis. A continuación, se da mayor detalle al funcionamiento y el uso de algoritmos.

### Matlab
- [MPSO_pololu_original.lxs](#MPSO_pololu_original.lxs)
- [MPSO_modified.lxs](#MPSO_modified.lxs)
- [MPSO_simulado.lxs](#MPSO_simulado.lxs)
- [MPSO_APF_simulado.lxs](#MPSO_APF_simulado.lxs)
- [MPSO_APF_pololu.lxs](#MPSO_APF_pololu.lxs)

### MPSO_pololu_original.lxs
El live script **MPSO_pololu_original.lxs** presenta un algoritmo de optimización llamado _Particle Swarm Optimization_ conocido por sus siglas como PSO, para encontrar la mejor posición de un enjambre de robots Pololu 3pi+, este live script explica de forma detallada cada parte del código. Es importante mencionar algunas modificaciones realizadas para el correcto funcionamiento del MPSO:

- **Controlador PID**
    - Distancia entre ruedas: Se consideró la distancia entre las ruedas desde el punto de instalación.

    <br><div align="center">
        <img src="Figuras/pololu_wheel.png" alt="Distancia entre ruedas Pololu 3pi+" width="200"><br>
    </div>

    - Ángulo de rotación: Hace que el offset entre el eje del marker y el eje x+ del robot diferencial sea 0, alineando ambos ejes. Los ángulos de rotación se utilizan en grados.
    (imagen)
- **Radio de convergencia**
    Se definió este radio para medir si los agentes lograron llegar a un área cercana a la meta. 
    (agregar imagen)

- **No colisiones entre los agentes robóticos**
<br><div align="center">
    <img src="Figuras/schaffer_4.gif" width="750" height="auto" alt="Experimento función Schaffer 4">
</div>

### MPSO_modified.lxs
El live script **MPSO_modified.lxs** describe las modificaciones que se realizaron al algoritmo MPSO utilizando vectorización para el cálculo del costo y el cálculo de las incercias.

### MPSO_simulado.lxs
El live script **MPSO_simulado.lxs** presenta la simulación del algoritmo MPSO utilizando cierta cantidad de partículas. 

### MPSO_APF_simulado.lxs
El **MPSO_APF_simulado.lxs** presenta la simulación del algoritmo MPSO utilizando campos artificiales potenciales para la evasión de obstáculos con cierta cantidad de partículas.

### MPSO_APF_pololu.lxs
El **MPSO_APF_pololu.lxs** presenta el algoritmo PSO con campos artificiales potenciales modificado para su funcionamiento con los agentes robóticos Pololu 3pi+ y el ecosistema Robotat.

### Webots 
- [PSO_simulacion_original.wbt](#PSO_simulacion_original.wbt)
- [PSO_simulacion_4.wbt](#PSO_simulacion_4.wbt)
- [PSO_simulacion_original_apf.wbt](#PSO_simulacion_original_apf.wbt)

### PSO_simulacion_original.wbt 
Este mundo contiene la simulación del algoritmo MPSO original utilizando el entorno _Webots_. La simulación está formada por:

## Software y hardware
Detalles sobre software y hardware...

## Información adicional
Información adicional del proyecto...

### Webots 


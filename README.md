# Optimización del algoritmo de robótica de enjambre *Particle Swarm Optimization* para su implementación con agentes robóticos físicos en escenarios con obstáculos en el ecosistema Robotat 
A continuación, se muestra una guía de como utilizar el algoritmo MPSO modificado, con campos potenciales artificiales para la evasión de obstáculos en el ecosistema Robotat. Y las modificaciones que se realizaron para la optimización del mismo.

## Tabla de Contenidos
- [Videos demostrativos](#videos-demostrativos)
- [Guía de uso](#guía-de-uso)
- [Software y hardware](#software-y-hardware)
- [Información adicional](#información-adicional)

## Videos demostrativos
Al darle click a la imagen podrás ver una lista de videos sobre los experimentos realizados en la optimización del algoritmo MPSO y el funcionamiento del algoritmo PSO con campos potenciales artifiales para la evasión de obstáculos.

## Guía de uso
En la carpeta *Códigos* en OneDrive se encuentran los códigos principales que se utilizaron en esta tesis. A continuación, se da mayor detalle al funcionamiento y el uso de algoritmos.

### Matlab
- [MPSO_pololu.m](#MPSO_pololu.m)
- [MPSO_modified.m](#MPSO_modified.m)
- [MPSO_simulado.m](#MPSO_simulado.m)
- [MPSO_APF_simulado_4.m](#MPSO_APF_simulado_4.m)
- [MPSO_APF_pololu.m](#MPSO_APF_pololu.m)

### MPSO_pololu.m
El script **MPSO_pololu.m** utiliza un algoritmo de optimización llamado _Particle Swarm Optimization_ conocido por sus siglas como PSO, para encontrar la mejor posición de un enjambre de robots Pololu 3pi+. Algunas modificaciones realizadas para el correcto funcionamiento del MPSO son las siguientes:

- **Controlador PID**
    - Distancia entre ruedas: Se consideró la distancia entre las ruedas desde el punto de instalación.

    <div align="center">
        <img src="Figuras/pololu_wheel.png" alt="Distancia entre ruedas Pololu 3pi+" width="300">
    </div>








## Software y hardware
Detalles sobre software y hardware...

## Información adicional
Información adicional del proyecto...


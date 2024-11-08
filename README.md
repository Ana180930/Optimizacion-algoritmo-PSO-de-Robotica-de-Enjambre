# Optimización del algoritmo de robótica de enjambre *Particle Swarm Optimization* para su implementación con agentes robóticos físicos en escenarios con obstáculos en el ecosistema Robotat 
El algoritmo PSO se inspira en el comportamiento colectivo de ciertos animales para localizar alimento. A continuación, se presenta una optimización del algoritmo PSO mediante técnicas de vectorización y paralelización, así como su implementación con campos artificiales potenciales para la evasión de obstáculos.

## Tabla de Contenidos
- [Videos demostrativos](#videos-demostrativos)
- [Códigos y guía de uso](#códigos-y-guía-de-uso)
- [Software y hardware](#software-y-hardware)
- [Información adicional](#información-adicional)

## Videos demostrativos
Al darle click en la imagen, podrás acceder a una lista de videos que muestran los experimentos realizados en la optimización del algoritmo MPSO y el funcionamiento del algoritmo PSO con campos potenciales artifiales para la evasión de obstáculos.
<br><div align="center">
    <a href="https://www.youtube.com/playlist?list=PLzFnfpUH2HcghOW6Uw1g37CLO4F0z6kMn">
        <img src="Figuras/robotat.JPEG" alt="Imagen en el repositorio" width="800"/>
    </a>
</div>



## Códigos y guía de uso
En la carpeta *Códigos* en OneDrive se encuentran los códigos principales que se utilizaron en esta tesis. A continuación, se da mayor detalle de los códigos implementados.

### Matlab
## Índice
- [MPSO_pololu_original.lxs](#mpso_pololu_originallxs)
- [MPSO_modified.lxs](#mpso_modifiedlxs)
- [MPSO_simulado.lxs](#mpso_simuladolxs)
- [MPSO_APF_simulado.lxs](#mpso_apf_simuladolxs)
- [MPSO_APF_pololu.lxs](#mpso_apf_pololulxs)

### MPSO_pololu_original.lxs
El live script **MPSO_pololu_original.lxs** presenta un algoritmo de optimización llamado _Particle Swarm Optimization_ conocido por sus siglas como PSO, para encontrar la mejor posición de un enjambre de robots Pololu 3pi+, este live script explica de forma detallada cada parte del código. Es importante mencionar algunas modificaciones realizadas para el correcto funcionamiento del MPSO:

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
    

- **No colisiones entre los agentes robóticos**

**Experimento función optimización Schaffer 4**
<br><div align="center">
    <img src="Figuras/schaffer_4.gif" width="700" height="auto" alt="Experimento función Schaffer 4"><br>
</div>

Puedes encontrar el script en la carpeta _MPSO_pololu_original_ 

### MPSO_modified.lxs
El live script **MPSO_modified.lxs** presenta las modificaciones que se realizaron al algoritmo MPSO, utilizando vectorización para el cálculo de la función de costo, el factor de incercia y el controlador PID.

### MPSO_simulado.lxs
El live script **MPSO_simulado.lxs** presenta la simulación del algoritmo MPSO con cierta cantidad de partículas. En este script puede definirse el objetivo o meta del enjambre.

**Experimento función de optimización meta**
<br><div align="center">
    <img src="Figuras/PSO_simulado.gif" width="400" height="auto" alt="Experimento función Schaffer 4"><br>
</div>

### MPSO_APF_simulado.lxs
El **MPSO_APF_simulado.lxs** presenta la simulación del algoritmo MPSO implementando campos potenciales artificiales para la evasión de obstáculos con cierta cantidad de partículas. Este script también incluye un planificador que determina la mejor trayectoria, con menor costo, encontrada por el enjambre mediante el PSO y los campos potenciales.

**Experimento obstáculo rectangular con MPSO y APF**
<br><div align="center">
    <img src="Figuras/PSO_APF_simulado.gif" width="400" height="auto" alt="Experimento función Schaffer 4"><br>
</div>

### MPSO_APF_pololu.lxs
El **MPSO_APF_pololu.lxs** presenta el algoritmo PSO con campos artificiales potenciales modificado, para su funcionamiento con agentes robóticos Pololu 3pi+ y el ecosistema Robotat.

### Webots 
- [PSO_simulacion_original.wbt](#PSO_simulacion_original.wbt)
- [PSO_simulacion_APF.wbt](#PSO_simulacion_APF.wbt)
- [PSO_simulacion_4.wbt](#PSO_simulacion_4.wbt)

### PSO_simulacion_original.wbt 
Este mundo contiene la simulación del algoritmo MPSO original utilizando el entorno _Webots_. La estructura de la simulación se muestra a continuación:

**Experimento función de costo Schaffer**
<br><div align="center">
    <img src="Figuras/PSO_webots.gif" width="500" height="auto" alt="Experimento función Schaffer 4"><br>
</div>



### PSO_simulacion_4.wbt
Este mundo contiene la simulación del algoritmo MPSO implementando un controlador PID vectorizado.

### PSO_simulacion_APF.wbt
Este mundo contiene la simulación del algoritmo PSO con campos potenciales artificiales para la evasión de obstáculos. Este algoritmo implementa cierta cantidad de partículas y agentes robóticos diferenciales.

<br><div align="center">
    <img src="Figuras/APF_PSO_webots.gif" width="500" height="auto" alt="Experimento función Schaffer 4"><br>
</div>


### Software y hardware
**Software**
Los programas utilizados fueron Matlab y Webots, en la siguiente tabla se presentan las versiones que se utilizaron: 

| **Matlab** | **Webots** | 
|--------|--------|
| R2022b | 2023b  | 

**Hardware**
El hardware que se utilizó fueron los agentes robóticos pololu 3pi+, las cámaras de movimiento OptiTrack y la mesa del Robotat.

<br><div align="center">
    <img src="Figuras/pololu.png" alt="Imagen robot pololu 3pi+" width="250"><br>
</div>

## Información adicional
- Correo eléctronico: analbflores2001@gmail.com
- Celular: 30021157
 



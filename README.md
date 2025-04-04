# Optimización del algoritmo de robótica de enjambre *Particle Swarm Optimization* para su implementación con agentes robóticos físicos en escenarios con obstáculos en el ecosistema Robotat 
El algoritmo PSO se inspira en el comportamiento colectivo de ciertos animales para localizar alimento, este permite la colaboración en grupo para alcanzar un objetivo en común. A continuación, se presenta una optimización del algoritmo PSO mediante técnicas de vectorización, paralelización y migración al lenguaje de programación Python, así como su implementación con campos artificiales potenciales para la evasión de obstáculos y la creación de un planificador de trayectorias.

## Tabla de Contenidos
- [Videos demostrativos](#videos-demostrativos)
- [Códigos](#códigos)
- [Software y hardware](#software-y-hardware)
- [Información adicional](#información-adicional)

## Videos demostrativos
Al darle click en la imagen, se podrá acceder a una lista de videos que muestran los experimentos realizados en la optimización del algoritmo MPSO, los experimentos del algoritmo PSO con campos potenciales artifiales para la evasión de obstáculos y el planificador de trayectorias.

<br><div align="center">
    <a href="https://www.youtube.com/playlist?list=PLzFnfpUH2HcghOW6Uw1g37CLO4F0z6kMn">
        <img src="Figuras/robotat.JPEG" alt="Imagen en el repositorio" width="800"/>
    </a>
</div>

## Códigos
### Algoritmo MPSO 
El algoritmo _Particle Swarm Optimization_ conocido por sus siglas como PSO, es un método de optimización que utiliza un enjambre de partículas para encontrar la mejor trayectoria hacia una meta en específico. El algoritmo _Modified Particle Swarm Optimization_ (MPSO) fue adaptado para implementar el PSO con agentes robóticos físicos, específicamente los robots pololu 3pi+, dentro del ecosistema Robotat. 

[Ver documentación](MPSO.md)

### Algoritmo MPSO vectorizado
El primer objetivo de este trabajo fue evaluar el algoritmo MPSO e identificar posibles puntos de mejora en el código, lenguaje de programación y métodos de comunicación con el ecosistema Robotat, con el fin de optimizar el rendimiento, reduciendo el tiempo de convergencia y ejecución del algoritmo. La primera mejora consistió en la implementación de vectorización sin la necesidad de utilizar ciclos for.  

[Ver documentación](MPSO_vec.md)

### Algoritmo MPSO migrado a Python
Otra posible solución para mejorar el tiempo de ejecución fue migrar el algoritmo MPSO al lenguaje de programación Python. Posterior a eso se implementó paralelización para evaluar si el rendimiento del algoritmo era mejor que el MPSO original. El método utilizado para la paralelización en Python es mediante el uso de hilos (threads).

[Ver documentación](MPSO_python.md)

### Algoritmo PSO con Campos potenciales artificiales
Se realizaron las mejoras mencionadas anteriormente, con el objetivo de implementar el algoritmo PSO para la evasión de obstáculos utilizando el método de campos potenciales artificiales. El algoritmo PSO dirige al enjambre de agentes robóticos pololu 3pi+, donde los robots son atraídos hacia la meta mediante el campo atractor y evitan los obstáculos debido a la fuerza repulsiva del campo repulsor. Es importante mencionar que este algoritmo encuentra las trayectorias libres de obstáculos en tiempo real.

[Ver documentación](MPSO_APF.md)

### Algoritmo PSO como planificador de trayectorias
El algoritmo PSO fue implementado como planificador de trayectorias con el fin de comparar su rendimiento con el algoritmo PSO con campos potenciales artificiales en tiempo real. Este también implementa campos potenciales artificiales, realizando primero la planificación de trayectorias libres de obstáculos, para luego realizar un seguimiento de trayectorias con los agentes robóticos.

### Software y hardware
**Software**
<br> Los programas utilizados para el desarrollo de los algoritmos fueron Matlab y Webots. Las versiones utilizadas se presentan en la siguiente tabla: 

| **Matlab** | **Webots** | 
|--------|--------|
| R2022b | 2023b  | 

Los experimentos se realizaron utilizando la computadora Lenovo Legion 5 16IRX9 con las siguientes especificaciones:

|**Especificaciones**| 
|--------------------|
| Intel Core i7-14650HX |
| NVIDIA Geforce RTX 4060 |
| Memoria RAM 16 GB |
| Disco duro 500 GB |


**Hardware**
<br> El hardware que se utilizaron fueron los agentes robóticos pololu 3pi+, las cámaras de movimiento OptiTrack y la plataforma del Robotat.

<br><div align="center">
    <img src="Figuras/pololu.png" alt="Imagen robot pololu 3pi+" width="250"><br>
</div>

## Información adicional
- Celular: 30021157
- Correo eléctronico: analbflores2001@gmail.com
 



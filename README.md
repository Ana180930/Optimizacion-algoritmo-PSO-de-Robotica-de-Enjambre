# Optimización del algoritmo de robótica de enjambre *Particle Swarm Optimization* para su implementación con agentes robóticos físicos en escenarios con obstáculos en el ecosistema Robotat 
El algoritmo PSO se inspira en el comportamiento colectivo de ciertos animales para localizar alimento. A continuación, se presenta una optimización del algoritmo PSO mediante técnicas de vectorización y paralelización, así como su implementación con campos artificiales potenciales para la evasión de obstáculos.

## Tabla de Contenidos
- [Videos demostrativos](#videos-demostrativos)
- [Códigos y guía de uso](#códigos)
- [Software y hardware](#software-y-hardware)
- [Información adicional](#información-adicional)

## Videos demostrativos
Al darle click en la imagen, podrás acceder a una lista de videos que muestran los experimentos realizados en la optimización del algoritmo MPSO y el funcionamiento del algoritmo PSO con campos potenciales artifiales para la evasión de obstáculos.
<br><div align="center">
    <a href="https://www.youtube.com/playlist?list=PLzFnfpUH2HcghOW6Uw1g37CLO4F0z6kMn">
        <img src="Figuras/robotat.JPEG" alt="Imagen en el repositorio" width="800"/>
    </a>
</div>

## Códigos 
En la carpeta *Códigos* en OneDrive se encuentran los códigos principales que se utilizaron en esta tesis. A continuación, se da mayor detalle de los códigos implementados.

## Matlab
### Algoritmo MPSO 
El algoritmo _Particle Swarm Optimization_ conocido por sus siglas como PSO, es un método de optimización que utiliza un enjambre de partículas para encontrar la mejor trayectoria hacia meta. El algoritmo _Modified Particle Swarm Optimization_ (MPSO) fue adaptado para implementar el PSO con agentes robóticos físicos, específicamente los robots pololu 3pi+, dentro del ecosistema Robotat. 

[Ver documentación](MPSO.md)


### Algoritmo MPSO vectorizado
Se realizaron varias mejoras al algoritmo MPSO, comenzando con la incorporación de la vectorización en el código. La implementación del controlador PID se modificó para que funcionara de forma vectorial, sin la necesidad de ciclos for. Además, se añadió vectorización al cálculo de la función de costo y al parámetro de inercia del PSO. 

[Ver documentación](MPSO_vec.md)

### Algoritmo PSO con Campos potenciales artificiales
Se implementaron campos potenciales artificiales para la evasión de obstáculos. El algoritmo PSO dirige al enjambre de robots pololu 3pi+, en el cual los robots son atraídos hacia la meta mediante el campo atractor y evitan los obstáculos debido a la fuerza repulsiva del campo repulsor.

[Ver documentación](MPSO_APF.md)

### Software y hardware
**Software**
<br> Los programas utilizados fueron Matlab y Webots, las versiones utilizadas se presentan en la siguiente tabla: 

| **Matlab** | **Webots** | 
|--------|--------|
| R2022b | 2023b  | 

Todos los experimentos se realizaron utilizando la computadora Lenovo Legion 5 16IRX9 con las siguientes especificaciones:

|**Especificaciones**| 
|--------------------|
|                    | 

**Hardware**
<br> El hardware que se utilizó fueron los agentes robóticos pololu 3pi+, las cámaras de movimiento OptiTrack y la mesa del Robotat.

<br><div align="center">
    <img src="Figuras/pololu.png" alt="Imagen robot pololu 3pi+" width="250"><br>
</div>

## Información adicional
- Celular: 30021157
- Correo eléctronico: analbflores2001@gmail.com
 



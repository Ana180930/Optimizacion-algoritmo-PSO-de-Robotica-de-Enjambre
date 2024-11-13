# Guía de uso documentación: Optimización del algoritmo de robótica de enjambre *Particle Swarm Optimization* para su implementación con agentes robóticos físicos en escenarios con obstáculos en el ecosistema Robotat 
A continuación, se presenta una guía de uso de la documentación, que incluye los códigos, documentos implementados, el enlace al repositorio en Github y los videos de los experimentos realizados.

## Tabla de Contenidos
- [Código](#código)
- [Documentos](#documentos)
- [Enlaces, repositorios externos, etc.](#enlaces-repositorios-externos-etc)
- [Multimedia](#multimedia)

## Código
En esta sección se incluyen los códigos desarrollados durante la realización de la tesis, organizados tres carpetas, facilitando la navegación y el acceso a los archivos.
- [Matlab](#matlab)
- [Python](#python)
- [Webots](#webots)

## Matlab
En esta carpeta se encuentran los códigos implementados para el algoritmo _Particle Swarm Optimization_ (PSO) y los campos potenciales artificiales en Matlab. Cada carpeta contiene un live script (extensión .mlx) que incluye mayor detalle a la implementación y modificaciones realizadas.

- **MPSO original**: Dentro de esta carpeta se encuentra el algoritmo _Modified Particle Swarm Optimization_ (MPSO) original implementado de forma física en el ecosistema Robotat (MPSO_pololu_original.mlx). También se incluye la simulación del algoritmo PSO en Matlab (MPSO_simulado.mlx).
- **MPSO APF**: Dentro de esta carpeta se encuentra el algoritmo PSO con campos potenciales artificiales para la evasión de obstáculos, implementado de forma física (MPSO_APF_pololu.m). También se incluye la simulación del algoritmo PSO con los campos artificiales en Matlab (MPSO_APF_simulado.mlx).

## Python
En esta carpeta se encuentra la migración del código MPSO al lenguaje de Python.

## Webots
En esta carpeta se encuentran las simulaciones de los algoritmos mencionados anteriormente, en el entorno de simulación Webots. 

- **controllers**: En esta carpeta se encuentran los controladores de los mundos creados.
    - **PSO_simulacion_4**: Mundo creado para la implementación del algoritmo PSO vectorizado. El controlador  del robot supervisor (más información en el repositorio de Github) implementado es main_controller_4 y el controlador para los robots diferenciales es pololu_pso_4.
    - **PSO_simulado_original**: Mundo creado para la implementación del algoritmo MPSO original. El controlador para el robot supervisor es main_controller_original y para los agentes robóticos es pololu_pso_original.
    - **PSO con APF**: Controlador creado para la implementación del algoritmo PSO con los campos artificiales potenciales para la evasión de obstáculos. El controlador para el robot supervisor es main_controller_apf y para los agentes robóticos es pololu_controller_apf.

## Documentos
En esta sección se incluyen los documentos utilizados durante el desarrollo de esta tesis, protocolo, tesis, póster y presentación final. Estos documentos se encuentran ordenados de la siguiente forma:

- **Póster, presentación**: En esta carpeta se encuentra el póster creado para la presentación final y las presentaciones realizadas durante el semestre para el curso de Diseño e Innovación.
- **Protocolo y tesis**: En esta carpeta se encuentran el protocolo y tesis final. 
- **Referencias**: En esta carpeta se encuentran los documentos utilizados durante el desarrollo de la tesis.

## Enlaces, repositorios externos, etc
En esta sección se presentan los enlaces que se consideraron importantes durante el desarrollo de esta tesis. También se presenta el enlace al repositorio externo de Github. 

## Multimedia
En esta sección se presentan la documentación visual de la tesis como: imágenes, videos de los experimentos y video final de la presentación de la tesis.







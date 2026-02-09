# Mobile Robotics Portfolio - Jair Vásquez Torres

Este repositorio contiene mi trabajo desarrollado en el curso "Robots Móviles" durante mi estancia en la UNAM (2024-2). He implementado módulos clave de autonomía, desde la planeación de rutas hasta la manipulación robótica.

## 🛠 Contribuciones Técnicas Destacadas

A continuación, resumo los algoritmos y sistemas que implementé y sintonicé exitosamente:

### 1. Planeación y Navegación Autónoma
* **Algoritmos de Ruta:** Implementación de **A*** (basado en grafos) y **RRT** (árboles aleatorios) para navegación global.
* **Suavizado de Rutas:** Optimización de trayectorias mediante algoritmos de descenso de gradiente para obtener curvas ejecutables por la base.
* **Seguimiento de Rutas:** Implementación de leyes de control de velocidad lineal y angular ($v, \omega$) para seguimiento preciso de trayectorias.
* **Campos Potenciales:** Desarrollo de métodos reactivos de evasión de obstáculos mediante fuerzas atractivas y repulsivas en tiempo real.



### 2. Localización y Percepción
* **Filtro de Partículas (Monte Carlo):** Implementación en C++ de la generación, movimiento y remuestreo de partículas para localización probabilística con LIDAR.
* **Filtro de Kalman Extendido (EKF):** Modelado matemático y cálculo de Jacobianos para la fusión de sensores.
* **Redes Neuronales:** Programación de algoritmos de **Backpropagation** desde cero para clasificación de patrones.
* **Representación del Entorno:** Generación de mapas de costo inflados y Diagramas de Voronoi (GVD) para navegación segura.



### 3. Proyecto Integrador: Robot de Servicio
Desarrollo de una máquina de estados para un robot móvil con manipulador:
* **HRI:** Integración de comandos por voz para tareas de búsqueda y transporte.
* **Manipulación:** Implementación de cinemática inversa para el agarre de objetos (Pringles, manzana).
* **Análisis de Robustez:** Evaluación experimental del sistema, identificando áreas de mejora en la precisión final del posicionamiento y la tasa de éxito del reconocimiento de voz (60%).

## Requerimientos

* Ubuntu 20.04 https://releases.ubuntu.com/focal/ubuntu-20.04.6-desktop-amd64.iso
* ROS Noetic http://wiki.ros.org/noetic/Installation/Ubuntu

## Instalación

Nota: se asume que ya se tiene instalado Ubuntu y ROS.

* $ cd
* $ git clone https://github.com/mnegretev/Mobile-Robots-2024-2
* $ cd Mobile-Robots-2024-2
* $ ./Setup.sh
* $ cd catkin_ws
* $ catkin_make -j2 -l2
* $ echo "source ~/Mobile-Robots-2024-2/catkin_ws/devel/setup.bash" >> ~/.bashrc
* $ source ~/.bashrc

## Pruebas

Para probar que todo se instaló y compiló correctamente:

* $ cd 
* $ source Mobile-Robots-2024-2/catkin_ws/devel/setup.bash
* $ roslaunch surge_et_ambula movement_planning.launch

Si todo se instaló y compiló correctamente, se debería ver un visualizador como el siguiente:
![rviz](https://github.com/mnegretev/Mobile-Robots-2024-2/blob/main/Media/rviz.png)

Un ambiente simulado como el siguiente:
![gazebo](https://github.com/mnegretev/Mobile-Robots-2024-2/blob/main/Media/gazebo.png)

Y una GUI como la siguiente:
![GUIExample](https://github.com/mnegretev/Mobile-Robots-2024-2/blob/main/Media/gui.png)


## Contacto
Dr. Marco Negrete<br>
Profesor Asociado C<br>
Departamento de Procesamiento de Señales<br>
Facultad de Ingeniería, UNAM <br>
marco.negrete@ingenieria.unam.edu<br>

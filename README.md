# Robot-hospitalario
Respositorio de vehículo autónomo con capacidad de navegación autónoma, por medio de establecimiento y ejecución de tareas o "misiones".

## Modos de operación (_deployment modes_)

* **Teleoperado**: El vehículo es dirigido mediante un mando a distancia.
* **Automatic**: El usuario introduce un grupo de coordenadas o asigna alguna tarea al vehículo.

## Tareas 

* **Navegación**: El vehículo se dirige a una coordenada específica.
* **Manipulación**: El robot despliega y utiliza el brazo robótico.
* **Tracking**: El robot localiza los objetos : [Puerta, Manillar, Humano, Cara]

_Nota_ : Versiones de ROS --> ROS 1 **Noetic** & ROS 2 **Foxy**.

## Arquitectura

# Setup ROS
Setup your robot for different tasks

## Robot Bringup
In Intel Nuc PC do (2 terminals)
* roscore
* ./catkin_ws/src/peacetolero_demo_2022_03_9/launch/config_script.bash bringup

In Jetson Orin nano do:
* roslaunch zed_wrapper zed.launch

## Robot 2D Slam (Visual Odometry + 2D laser)
* ./catkin_ws/src/peacetolero_demo_2022_03_9/launch/config_script.bash slam2d

## Robot 3D Slam (RBGD-Camera)
* ./catkin_ws/src/peacetolero_demo_2022_03_9/launch/config_script.bash slam3d

To check the map with the robot urdf in your pc:
* roslaunch urdf_tutorial display.launch





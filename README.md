# Trabajo practico N1 - Sistemas graficos

![image](https://user-images.githubusercontent.com/50753891/197894500-152d376b-1c4b-4ce9-b006-b61c3da946f0.png)

## Modelos:
- Castllo
- Escena
- Camaras
- Rendering
  - Orbital general
  - Orbital catapulta
  - Primera persona

## Menu
Implementado con la libreria [dat.gui](https://github.com/dataarts/dat.gui)

## Algoritmos y Funciones requeridos para la implementación 
- Curvas de Bezier/Bspline cúbicas: a partir de un arreglo de puntos de control, las 
funciones deben poder evaluar un punto de la curva en base al parámetro “u”. 
Además, es necesario que pueda evaluar el vector tangente y normal a la curva 
 
- Discretizador de curvas: dada una curva Bezier o Bspline y un “delta u” devuelve una 
secuencia de puntos correspondientes a la posición, tangente o normal 
 
- Constructor Objeto 3D: debe ser capaz de crear instancias transformables (posición, 
traslación y escala) que puedan vincularse jerárquicamente (padre/hijo). Estas pueden 
tener o no buffers asociados (por ejemplo, en el caso de contenedores) 
 
- Superficie de Barrido: debe ser capaz de recibir como parámetros la forma y el 
recorrido y devolver los buffers correspondientes a la superficie. Varias piezas del 
vehículo requieren formas que varían de escala a lo largo del recorrido. La forma más 
simple de implementar esta capacidad es poder tener múltiples formas ubicadas en 
distintos puntos del recorrido. La única condición necesaria es que todas las formas 
posean la misma cantidad de vértices 
 
- Superficie de revolución: idem barrido, pero en lugar de un recorrido, recibe el 
parámetro “eje” 
![image](https://user-images.githubusercontent.com/50753891/197895069-a01668f9-b8e1-4e6c-8e0a-80cd2c79f876.png)
![image](https://user-images.githubusercontent.com/50753891/197895100-20c4de14-8771-4873-94ab-339041901f91.png)

 

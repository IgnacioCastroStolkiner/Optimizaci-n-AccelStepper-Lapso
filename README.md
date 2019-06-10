# Optimizacion-AccelStepper-Cristales-Sonicos
Proyecto para optimizar la librería AccelStepper para que pueda alcanzar mayor velocidad.

AccelStepper-master es la librería

Cristal_Steppers.ino es el código de las arduino.

Necesitamos controlar 5 motores paso a paso con driver desde una Arduino Mega. Actualmente nos encontramos con la 
limitación de que a más de 200 micropasos/s (para 5 motores a la vez) la Arduino deja de responder de forma lineal y poco después deja
de crecer. La reducciòn entre el eje del motor y la base circular de las columnas es muy grande y el procesador de la Arduino no llega a enviar la cantidad de pulsos necesarios para que los 5 motores se muevan rápido a la vez. 

Este proyecto busca investigar la forma de conseguir modificar la librería AccelStepper o el programa actual para
conseguir velocidades mayores dentro de las limitaciones de procesamiento de la arduino. 

Prueba 1: Probamos mover motores sueltos bastante mayor velocidad, así que deducimos que probablemente no sea una limitación del driver
ni de torque de los motores.

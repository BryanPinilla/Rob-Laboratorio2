Realización del código

Para la realización de código fue necesario cambiar algunos aspectos del código de la guía de Epson, pues se hizo uso de un robot diferente.

Se deben encender los motores del robot por código tal como se aprecia y la potencia también.

Se creó una cuadrícula para que el robot siguiera un patrón programado, la aceleración y la velocidad se ajustaron a los valores máximos para la simulación pero luego se cambiaron a los valores mínimos para mover el robot por motivos de seguridad recomendados por el encargado.

Hay dos funciones de paletizado pletizado_z y paletizado_s, la primera hace que el robot siga el patrón en las casillas 1,2,3,4,5,6,7,8 y 9 en ese orden y la segunda hace que el robot siga el patrón en las casillas 1,2,3,6,5,4,7,8 y 9 en ese orden.

En el caso de las funciones Go, Move y Jump solo fue necesario usa la función Go pues el encargado aconsejó que así fuera pues las trayectorias realizadas con esta función son curvas, mientras que las trayectorias realizadas con la función Move son lineales lo que implica una mayor cantidad de cálculos y posibles singularidades en el robot, en el caso de la función Jump no se usó pues esta no existía para el modelo de robot que fue utilizado por lo que se reemplazó por la orden "Go Pallet(1, i) :Z(200)" que se encuentra en los ciclos For para que el robot se posicionara sobre una de las casillas y bajara 20 centímetros y luego volviera a subir (demostrado en los videos adjuntos). 

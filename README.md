#  **Obligatorio 1 FIS**

Docente: Alejandro Adorjan
Grupo: M4B
Estudiantes: Facundo Cambra (242462), Bruno Quagliata (254256)

https://github.com/facuCambra/Obligatorio-algoritmos2.git

## Repositorio y versionadonado 
Para tener un almacenamiento compartido y con un buen sistema de versionados utilizamos la herrameitna GitHub. Lo que se hizo fue crear un repositorio privado en la web de GitHub y posteriormente compartirlo. De forma tal que cada integrante realizara un "init" en su pc y clonara el repositorio remoto. De esta forma todos los desarrolladores contaban con una versión local y a su vez estaba el repo online. Por lo que se aprovecho la caracteristica de descentralizacion de git. Ya que cada persona trabaja de forma local y cuando realiza cambios los puede subir (con un pusn pusal repositorio remoto para que los demas developers puedan ver las actualizaciones. Esto tambien se da de forma contraria ya que un developer puede hacer un "pull" para actualizar su repo local.

Utilizamos 2 ramas, una en la cual se ve enfocada en subir todas las actualizaciones llamada "develop" y otra donde solo se incluyen las versiones estables, cuyo nombre es "main"

Para el versionado utilizamos "conventional commits".




## Elicitacion
### Entrevistas
Para lograr un primer acercamiento a lo que significaron los usuarios de nuestra aplicación, decidimos realizar entrevistas a distintos compañeros para tener una idea general de las experiencias de cada uno y en base a eso enfocar el proyecto a partir de las necesidades de los mismos.

#### Conclusiones de entrevistas
Nos encontramos con respuestas muy diversas en cada uno de los participantes. Sin embargo, notamos que todos comprenden a la aplicación como algo de suma utilidad para mantener un registro de los gastos de cada uno y así tener mayor control del presupuesto que se disponga.
Visualizamos también como la aplicación sería de mayor utilidad para aquellas personas que gastan montos elevados de dinero mensualmente ya que muchos llegaban a la conclusión que perdían referencia de la plata gastada en una noche al no tener un control apropiado de sus gastos. 
Por otro lado, vimos que aquellas personas que disponían de montos más bajos eran mucho más conscientes de los gastos totales.
Otro aspecto interesante que notamos fue la amplia diferencia en cuanto a los gastos en función de qué actividad fueran a realizar, ya sea salir a un bar, una fiesta, un asado, entre otros. Cada actividad supone montos distintos.
Otro factor aparente surgió a partir del Covid, los usuarios coinciden en que las actividades recreativas tuvieron un cambio rotundo a lo que solían hacer años atrás, actividades como los locales bailables, bares, cerraron sus puertas por lo que muchos usuarios debieron adaptarse a las circunstancias. Surgen conceptos nuevos como los de fiestas clandestinas que traen consigo gastos de insumos que antes no eran recurrentes y ahora eran fundamentales en todas las noches.


### Lluvia de ideas
Para poder tener un panorama de las funcionalidades del sistema que se pueden implementar realizamos una lluvia de ideas, de la cual determinamos las siguientes funcionalidades como candidatas a ser implementadas: 
- Almacenamiento de los gastos en actividades nocturnas
- Almacenar las bebidas,comidas y otros productos que el usuario adquirió 
- Sugerencias de lugares
- Sugerencias de bebidas
- Desplegar información sobre actividades pasadas
- Tener una puntuación de lugares,actividades, bebidas, comidas.
- Permitir ingresar un monto destinado a las actividades de un rango de tiempo, para así tener un seguimiento en tiempo real del dinero que dispone el usuario. 
- Permitir al usuario seleccionar el tipo de actividad que vaya a concurrir ya sea bar, fiesta, asado, etc
- Permitir al usuario ingresar un monto tentativo de gasto para una actividad  y en función de esto el sistema mostrará sugerencias. 
- Permitir buscar actividades según criterios de búsqueda a definir (ubicación, tipo de actividad, horario, etc.)
- Exista un registro colectivo de información de todos los usuarios


## Idealizacion de usuarios del sistema
![](https://i.imgur.com/YOBacmi.png)

![](https://i.imgur.com/6FwQiNr.png)


# ESPECIFICACIÓN:

## Requerimientos funcionales  
### Actores: 
* Admin local recreativo
* Persona	

### Requerimientos Funcionales:
1. Asistir a un actividad
1. Organizar un actividad
1. Ingreso de presupuesto total 
1. Ingreso de gastos en una actividad
1. Puntuar una actividad asistida
1. Mostrar listado de gastos 
1. Gráfica de gastos en función del tiempo u otros parámetros
1. Listado de actividades a las que se asistió según (Dinero gastado sobre diversión)
1. Alerta de presupuesto bajo
1. Listado de actividades de interés
1. Reparto de gastos entre participantes

### Requerimientos No Funcionales:
1. Disponible en idioma español
1. El sistema debe funcionar en Windows 10. 
1. La aplicación debe poder funcionar en dispositivos móviles; en ios 15.02 y android 12. 
1. Se tendrá documentación del proceso de desarrollo del sistema.

### Descripcion de requerimientos funcionales 
**RF 1**: Asistir a una actividad

Actor: asistente 

Descripción: el sistema deberá permitir que el usuario seleccione una actividad previamente creada para así poder inscribirse a la misma. 

Prioridad : alta 

**RF 2**: Organizar una actividad 

Actor: todos

Descripción: el Sistema permite a un usuario crear un evento. Si es dueño de un local se le permite crear un evento relacionado al mismo. Si es una persona solo podrá crear actividades a locales de otros dueños o lugares públicos.

Prioridad : alta  

**RF 3**: Ingreso de presupuesto 

Actor: persona

Descripción: el usuario podrá ingresar un monto de dinero y se le permitirá seleccionar si el mismo está destinado a una actividad particular o a un rango de tiempo que deberá definir.

Prioridad: alta 

**RF 4**: ingreso de gastos en una actividad 

Actor: persona 

Descripción : el sistema permitirá al usuario seleccionar una tarea a la que ya asistió o está asistiendo al momento de la operación. Para así permitir que ingrese un gasto realizado en la misma. Dicho gasto debe tener un monto y descripción. Se podrá seleccionar de qué categoría es (bebida, comida, entrada, etc) 

Prioridad: alta 

**RF 5**: Puntuar una actividad asistida

Actor: persona

Descripción: el sistema admitirá que un usuario seleccione una tarea a la que ya asistió, para así permitir que el mismo la califique. La calificación va a ser un número en el rango de 0 a 5 estrellas. También se permitirá dejar un comentario de no más de 100 caracteres. 

Prioridad : media 

**RF 6**: Mostrar gastos 

Actor: persona 

Descripción: el sistema mostrará al usuario un listado de gastos. Los formatos de listado serán 2, mostrar todos los gastos de forma individual con referencia a que actividad está asociado y por otro lado se podrá listar las actividades y su suma de gastos, permitiendo acceder a la actividad para ver el detalle de gastos. 

Prioridad: media 

**RF 7**: Graficar en función de parámetros 

Actor: persona 

Descripción: el sistema deberá mostrar una gráfica según los siguientes posibles parámetros :
Dinero en función del tiempo 
Calificaciones en función del dinero 
Promedio de calificaciones respecto al tipo de actividad 
Cantidad de actividades a las que se asistió en función del tiempo (meses) 

Prioridad: baja 

**RF 8**: listar actividades según calificaciones 

Actor : persona 

Descripción: el sistema listará las actividades a las que usuario asistió, ordenandolas en función de las calificaciones de las mismas. Las de mayor calificación irán primero. 

Prioridad: media 


**RF 9**: Alerta de presupuesto  bajo 

Actor: persona 

Descripción: el sistema deberá notificar al usuario cuando se halla gastado un 80% del presupuesto fijado para una actividad o un rango de tiempo 

Prioridad: media 

**RF 10**:  Listado de actividades de interés 

Actor: persona 

Descripción: el sistema deberá mostrar al usuario las actividades próximas a realizarse que el mismo determine que puede ser de interés del usuario. Esto se realizará en función de actividades pasadas. 

Prioridad: media 

**RF11**: Reparto de gastos entre participantes 

Actor: persona 

Descripción: se permitirá que los asistentes de una determinada actividad repartan los gastos que se realizaron en la misma. Se podrá repartir el gasto total o seleccionar individualmente cada gasto y asignalro a uno o varios asistentes. 

Prioridad: media 

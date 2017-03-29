# Requerimientos

## 1. Características Generales del Proyecto

+ 50x50 celdas de 10px cada una.
+ Añadir/Eliminar células.
+ Configuración de colores (hasta 8 colores).
+ Generación finita e infinita de pasos.
+ Control de pasos (100 mil pasos).
+ Control de tiempo (hasta 5 segundos por paso).
+ Control de reproducción (pausa/iniciar/detener/reiniciar).
+ Exportar generación en pausa (en formato JSON).

## 2. Historias de usuario.

+ [ ] Como usuario, quiero ver una grilla cuadrada de 50 celdas de longitud, donde cada celda sea cuadrada de 10 píxeles de longitud.
+ [ ] Como usuario, quiero indicar las células(celdas) que estarán vivas en la generación inicial, haciendo click sobre cualquier celda. Una vez para indicar que está viva y otra vez para indicar que está muerta
+ [ ] Como usuario, quiero señalar las células que estarán vivas con un color y las que estarán muertas con otro color distinto, personalizable (entre un máximo de 8 colores precargados). Las celdas vacías, siempre estarán marcadas de color blanco
+ [ ] Como usuario, quiero ver un grupo de botones con acciones correspondientes al control de reproducción de las células, es decir:
  + Un botón de iniciar, que comience la reproducción celular en el estado en que se encuentre la grilla.
  + Un botón de pausar, que detiene temporalmente la reproducción celular, pero al volver a hacer click en dicho botón debe empezar nuevamente la reproducción desde el estado anterior
  + Un botón de detener, que detiene la reproducción, pero no debe permitir volver al estado anterior.
  + Un botón de reiniciar, que limpia toda la grilla.
+ [ ] Como usuario, quiero configurar el tiempo que transcurre entre generación y generación (desde 300ms hasta 5000ms).
+ [ ] Como usuario, quiero tener un control de generaciones celulares, por lo que debe permitir decidir si se quiere generación finita (desde 100 hasta 100 mil generaciones) o infinita (hasta que la grilla esté **estable**).
+ [ ] Como usuario, quiero que incluso al iniciar la reproducción, me permita incluir nuevas células a la grilla.
+ [ ] Como usuario, quiero que al pausar la reproducción, no permita el ingreso de nuevas células, tampoco al detener la reproducción.
+ [ ] Como usuario, quiero que, por cualquiera de las posibles causas que pudieran presentarse, el juego emita una notificación indicando que la generación es **estable**, esto es, si no existen más reproducciones posibles.
+ [ ] Como usuario, quiero que el juego mantenga las normas del juego de la vida original de John Conway, las cuales son:
  + La vecindad entre células se cuenta por lados (arriba, izquierda, abajo y derecha) y por vértices (esquinas, superior e inferior derecha e izquierda correlativamente).
  + Si una célula tiene menos de 2 vecinos vivos, muere por soledad en la próxima generación.
  + Si una célula tiene más de 3 vecinos vivos, muere por sobrepoblación en la próxima generación.
  + Si una célula tiene exactamente 2 ó 3 vecinos vivos pueden ocurrir dos casos:
    + Si la célula está viva, se mantiene con vida en la próxima generación.
    + Si la célula está muerta, revive en la próxima generación.

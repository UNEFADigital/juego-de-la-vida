# Requerimientos

## 1. Características Generales del Proyecto

+ Tabla de registro de estudiantes (hasta 8 estudiantes).
+ CRUD completo de datos de los estudiantes.
+ Registro y modificación de notas (4 por estudiante).
+ Posibilidad de ordenar alfabéticamente los datos.
+ Persistencia (LocalStorage).
+ Cálculo automático del promedio de notas equivalente.
+ Colores alusivos al estatus de un estudiante.
+ Validación completa de los campos de registro.

## 2. Historias de usuario.

+ [ ] Como usuario, quiero ver una tabla donde se liste la información de los estudiantes regstrados en una sección (hasta 8 estudiantes).
+ [ ] Como usuario, quiero registrar los siguientes datos por estudiante:
  + Apellido, Nombre
  + Cédula de Identidad
  + Correo Electrónico
  + Estatus (Reprobado, Aprobado, Cursando)
+ [ ] Como usuario, quiero poder registrar hasta 4 notas numéricas correspondientes a los cortes (de 25%) de la nota de cada estudiante.
+ [ ] Como usuario, quiero poder ordenar alfabéticamente todos los estudiantes por apellido y nombre.
+ [ ] Como usuario, quiero ver las notas de un estudiante en una ventana modal aparte, correspondientes a sus cortes. Estas notas podrán ser modificadas una vez registradas, pero no pueden ser eliminadas a menos que se elimine al estudiante del registro. La nota mínima es 0 y la máxima es 25.
+ [ ] Como usuario, quiero ver la nota calculada en base a 20 puntos por el propio registro, haciendo la conversión respectiva (1 corte de 25% = 5 puntos).
+ [ ] Como usuario, quiero buscar por apellido o nombre o cédula de identidad a un estudiante en particular.
+ [ ] Como usuario, quiero poder eliminar estudiantes del registro, con sus respectivas notas del almacén.
+ [ ] Como usuario, quiero ver que un estudiante pueda tener 3 estatus durante el registro:
  + "Cursando", estatus por defecto y se asigna a un estudiante que no tiene al menos un corte de notas registrado (color azul).
  + "Aprobado", estatus que se le asigna a un estudiante cuando todas sus notas han sido registradas y el cálculo promedio resulta mayor a 10 puntos (color verde).
  + "Reprobado", estatus que se le asigna a un estudiante cuando todas sun notas han sido registradas y el cálculo promedio resulta menor a 10 puntos (color rojo).
+ [ ] Como usuario, quiero que el registro notifique adecuadamente los mensajes respectivos a las respuestas devueltas por el sistema.
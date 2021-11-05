# IEEE TEST PLAN TEMPLATE

## 1) Test Plan Identifier 
```plan_calidad_v0_1```

Fecha: 05/11/2021
Autores: equipo 404NotFound

## 2) References 
Usaremos el plan de requermientos para saber qué se buscaba lograr con la funcionalidad de la lista de espera. También usaremos la documentación del código para entender la forma en que fue implementado. Será importante ver los casos de uso para identificar el tipo de pruebas que se harán para ver el funcionamiento de la funcionalidad.

## 3) Introduction 
El propósito de este plan es verificar la nueva funcionalidad para la página de inscripción de materias en el ITAM. Dentro de la nueva funcionalidad, cabe mencionar: 
* Listas de espera para los alumnos
* Visualización de lista de espera para los profesores
* Capacidad de los profesores para aceptar o rechazar estudiantes en la lista de espera
* Notificación al cambiar el estado de la lista de espera de los alumnos

El proceso de pruebas se describe a continuación.

## 5) Software Risk Issues
Algunos de los posibles riesgos son:
* que la información le llegue a las personas equivocadas. Tanto que a los profesores les lleguen otras listas de esperas, no les lleguen o a los alumnos no les llegue su confirmación o le llegue a otras personas;
* que el traspaso de información sea inseguro y pueda filtrarse fácilmente, revelando información personal de los alumnos o profesores;
* que un error en la funcionalidad de las listas de espera afecte el funcionamiento general de la página y afecte el sistema de horarios;
* que el mal manejo de la base de datos pueda modificar erróneamente las bases de datos de horarios.

## 6) Features to be Tested 
Se va a probar que se dé de alta correctamente una lista de espera, que el profesor pueda visualizar todas las listas de espera por materia, que pueda aceptar o rechazar las listas de espera y que al alumno se le notifique cuando se aceptó o rechazó su lista de espera. 

## 7) Features not to be Tested 
No vamos a probar lo que ya se estaba usando correctamenete en la versión 1 del sistema de inscripciones; por ejemplo: el login, la tira de materias, que al registrarte exitosamente te muestre tu horario al final, etc.

## 8) Approach 
Se va a probar mediante librerías las funciones relacionadas a los alumnos directamente involucrados, es decir, los que hacen peticiones para ingresar a una lista de espera o para meter automáticamente una materia en cuanto se pueda. Por otro lado, se probará de forma manual que los otros usuarios no reciban notificaciones que no le corresponden, y hacer una prueba en general del sistema para ver si hay algún tipo de fallo no identificado. 

También vamos a probar manualmente que un profesor pueda aceptar o rechazar alumnos en la lista de espera. Para esto, solicitaremos la participación de unos 5 profesores y les pediremos que utilicen el software. Posteriormente, por medio de una encuesta de satisfacción, les preguntaremos si esta nueva metodología les pareció más fácil de usar y, sobre todo, si le vieron alguna falla (ya sea de seguridad o de funcionalidad).


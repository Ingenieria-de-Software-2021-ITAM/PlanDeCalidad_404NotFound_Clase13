# IEEE TEST PLAN TEMPLATE

## 1) Test Plan Identifier 
```plan_01```

Fecha: 05/11/2021

## 2) References 
Usaremos el plan de requermientos para saber que se buscaba lograr con la funcionalidad de la lista de espera. Tambien usaremos la documentación del codigo para entender la forma en que fue implementado. Será importante ver los casos de uso para identificar el tipo de pruebas que se harán para ver el funcionamiento de la funcionalidad. 

## 3) Introduction 
El propósito de este plan es verificar la nueva funcionalidad para la página de inscripción de materias en el ITAM. Dentro de la nueva funcionalidad, cabe mencionar: 
* Listas de espera para los alumnos
* Visualización de lista de espera para los profesores
* Capacidad de los profesores para aceptar o rechazar estudiantes en la lista de espera
* Notificación al cambiar el estado de la lista de espera de los alumnos

El proceso de pruebas se describe a continuación.

## 5) Software Risk Issues 
1. Que la información le llegue a las personas equivocadas. Tanto que a los profesores les lleguen otras listas de esperas, no les lleguen o a los alumnos no les llegue su confirmación o le llegue a otras personas. 
2. Que el traspaso de información sea inseguro y pueda filtrarse fácilmente, revelando información personal de los alumnos o profesores. 
3. Que un error en la funcionalidad de las listas de espera afecte el funcionamiento general de la página y afecte el sistema de horarios.
4. Que el mal manejo de la base de datos pueda modificar erróneamente las bases de datos de horarios.

## 6) Features to be Tested 
Se va a probar que se de alta correctamente una lista de espera, que el profesor pueda visualizar todas las listas de espera por materia, que pueda aceptar o rechazar las listas de espera, que al alumno se le notifique cuando se aceptó o rechazó su lista de espera. 

## 7) Features not to be Tested 
No vamos a probar lo que ya se estaba usando correctamenete en la versión 1 del sistema de inscripciones, por ejemplo, el login, la tira de materias, que al registrarte exitosamente te muestre tu horario al final, etc.

## 8) Approach 

# HICAPPS Technical Test

La presente prueba técnica pretende evaluar sus habilidades y competencias para el cargo de **Desarrollador Full Stack**.
El test consta del desarrollo de un micro-proyecto los cuales debe resolver en un periodo máximo de 96hrs. desde que ha sido presentado este repositorio vía email.

# Descripción de la prueba
Se debe crear una función serverless utilizando Cloud Functions de Firebase que permita leer y escribir en una base de datos de pacientes usando RTDB de Firebase. Cada paciente debe estar almacenado en un nodo llamado `pacientes` y debe poseer un identificador único (UUID) con los siguientes atributos:

* Nombre
* Apellido Paterno
* Apellido Materno
* Número de seguridad social (inventado, cualquiera sirve)

Se debe desplegar una Cloud Function que permita:

* Leer todos los pacientes en el nodo de `pacientes`.
* Obtener los datos de un paciente en particular
* Crear un nuevo registro en el nodo de `pacientes`.

### Requisitos previos
* Crear un nuevo proyecto de Firebase. Nombrarlo de la siguiente manera: `hicapps-<NOMBRE>-<APELLIDO>`
* Instalar en su máquina local Firebase CLI: `npm install -g firebase-tools`

### Requerimientos funcionales
* La Cloud Function debe poseer un recurso llamado `/pacientes` donde se ejecutaran las llamadas HTTP.
* Se debe poder obtener los datos de todos los pacientes (no es necesario que estén paginados) llamando por GET a `/pacientes`.
* Se debe poder obtener los datos de un paciente en particular llamando por GET a `/pacientes/:id_paciente`
* Se debe poder crear un nuevo paciente llamando por POST a `/pacientes`.

### Requerimientos no funcionales
* Debe crear un proyecto de Cloud Functions con ESLint
* El projecto debe utilizar JavaScript (no TypeScript)
* El proyecto debe tener correctamente ignorados los secretos y variables de ambiente que vaya a utilizar

# Entregables
El candidato debe realizar entrega de lo siguiente:

* URL con el repositorio al código de la solución (público)
* URL a Cloud Function deployeada en su proyecto de Firebase
* JSON con estructura de la base de datos (utilizar el export de Firebase)

# Criterios de evaluación
| Evaluación                                      | Puntos |
|-------------------------------------------------|--------|
| Cumplir todos los requerimientos funcionales    | 10 pts |
| Cumplir todos los requerimientos no funcionales | 10 pts |
| Modelamiento adecuado de base de datos          | 5 pts  |
| Indentación adecuada del código                 | 5 pts  |

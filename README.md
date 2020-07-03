# comafi-challenge

## challenge requirements

Se desea realizar un servicio Rest para gestionar becas y cupos de estudios de cursos en diferentes categorías y empresas.

Los cursos son publicados en la app por empresas que deben estar registradas en el sistema y aprobadas por un usuario de tipo administrador. Mientras la empresa no tenga dicha aprobación, no podrá tener cursos asociados.

Los datos de la empresa en el sistema deben ser:

* nombre de empresa
* cuil
* tipo de empresa
* dirección fiscal
* categoría de la empresa (rubro al que se dedica)
* año de fundación
* número(s) de contacto

A su vez, la empresa debe registrar un representante encargado para ingresar los cursos que ofrecerá en la plataforma. Los datos del respresentante son:

* nombre y apellido
* tipo y numero de documento
* cargo dentro de la empresa
* email

Los datos de los cursos que los representantes van a ofrecer, son:

* nombre del curso
* descripción del curso
* modalidad de cursada
* costo del curso
* horas de duración del curso
* categoria a la que pertenece el curso
* total de cupos para el curso
* cantidad de cupos para becas

La cantidad de cupos de becas, están contempladas en el total de cupos del curso.

Por otro lado, el sistema admite registro de usuarios de tipo participantes (alumnos), los datos de esto deben ser:

* nombre y apellido
* tipo y número de documento
* fecha de nacimiento
* email
* dirección de vivienda

Los participantes pueden realizar una postulación a un curso por 2 modalidades: por compra directa o por solicitud de becas. Al hacer una solicitud por compra directa, se le asigna un cupo en el curso, y cuando hace una solicitud por beca, esta debe ser aprobada por un usuario de tipo administrador para asignarle el cupo en el curso. 

Para realizar una postulacion por beca, el participante debe tener la información de su estudio socio-economico en el sistema, dicha información consta de lo siguiente:

* ¿Estudia?
* ¿Trabaja?
* En caso de que trabaje, ingresos mensuales
* ¿Tiene carga familiar?
* En caso que tenga carga familiar, ¿De cuánto es?

El usuario administrador puede aprobar o rechazar las postulaciones de becas, en el caso de aprobación, debe indicar el porcentaje de aprobacion de becas, las cuales son: 50%, 75% y 100%.

## Motor de busqueda

El motor de búsqueda de la app debe contemplar los siguientes criterios:

* listar todo los cursos con cupos disponibles
* listar todo los cursos con cupos disponibles y por categoria de curso
* listar todo los cursos con cupos disponibles y por empresa
* listar los participantes con cupos aprobados por curso
* listar los cursos de un participantes (curso aprobados)

# Challenge_QA_CleverIT

Ejercicio 1 (QAA-01) API Temperatura.

1- Enviar el request con la fecha correctamente seteada, con las 5 conbinaciones correctas de los headers. Probar (Happy Path): a- Status code 200 Ok. b- Tiempo de respuesta Ok. (parámetro indicado) c- Que ambos datos del response sea de tipo double. d- Con los datos de Temperatura de una fecha específica validar que los datos del response correspondan a los antes consultados a la fecha indicada. e- Probar que no venga ningun dato del response vacío. f- Estresar la API con una cierta cantidad de consultas una tras otra usando un archiveo .csv.

2- Con las 5 combinaciones incorrectas de los headers, probar: a- Client error.

3- Enviar el request con uno de los headers vacío.

5- Desconectar la API y probar el Server Error.

6- Probar con nombres de paises y ciudad incorrectas.

7- Probar ingresando fecha inexistente.

8- Probar fecha con formato incorrecto.

/////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

Ejercicio 3 (QAA-03) Explicación de técnicas.

En todos los tests se visualiza la URL en una variable de entorno. En el "Put modificacion de posts" se observan tecnicas de Carga de datos por parametros, reutilización de los tests usando variable anónima. En el "Post a posts con variables dinamicas" utilicé variables aleatorias dinámicas. Siempre es neceasario en principio probar los flujos principales a ver si funcionan, por ello se evalua el codigo de respuesta 200 o 201, Que los values de los atributos del response que son obligatorios no vengan vacíos, Que tenga el tipo de dato correcto segun lo indica el modelado de datos. En segundo lugar probaria la performance de los servicios y por último (y no menos importante) las pruebas negativas, donde la API si o si debe fallar.

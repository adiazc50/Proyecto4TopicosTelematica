*Modelo PCAM:*

*REALIZADO POR:*  ALEJANDRO DIAZ CANO

*PROBLEMA:* 

Uno de los inconvenientes mas grandes que tenemos en la actualidad es la seguridad de los datos, para ello se a recurrido a múltiples algoritmos que se usan para cifrar palabras, documentos y archivos con la finalidad de mantener la integridad de los datos de la manera mas segura posible entre un emisor y un remitente.
En este proyecto buscamos crear un cifrador de palabras o textos usado antiguamente y reconocido como “el cifrado de cesar”. con el cual buscamos con un mensaje inicial obtener un mensaje final seguro, que alguien sin la clave no va a lograr leerlo o descífralo fácilmente.

*PARTICIÓN:*

como entrada pueden ingresar palabras, las cuales se deben operar en diversos pasos como el paso de salteado de las letras entre la letra original y el valor de la letra a ser modificada, la modificación de la letra por el valor de la letra encriptada y el envió del mensaje, adicionalmente a la encriptación el proceso de desencriptación que contiene los mismos pasos al revés.
Si se encripta:
T1 -> Leer palabra de entrada
T2-> Pararme en una letra de la palabra
T3-> Reemplazar letra por otra en base a la clave.
T4->Avanzar a la siguiente letra almacenando el valor en una nueva palabra
T5-> Regresar a la T3 hasta que se termine la palabra
Si se desencripta: 
T1 -> Leer palabra de entrada
T2-> Pararme en una letra de la palabra
T3-> Regresar letra por otra en base a la clave almacenando el valor en una nueva palabra
T4->Avanzar a la siguiente letra
T5-> Regresar a la T3 hasta que se termine la palabra

*COMUNICACIÓN:*

Todas las tareas vienen dadas por la palabra que ingrese, esta palabra que ingresa entra a la T1, la tarea uno lo que hace es que empieza a recorrer la frase letra a letra(T2) y empieza a reemplazar esa letra por una cantidad de letras que se encuentran adelante o atrás dependiendo del valor de la clave del cifrado(T3), Avanza a la siguiente letra(T4) y volvemos a la T3 hasta terminar la palabra. 


*AGLOMERACIÓN:*

Se pueden aglomerar las tareas T1 y T2, -> para iniciar la encriptación con T3 y T4 y terminar en T5 hasta que no queden mas palabras por ser encriptadas.
MAPEO: Las tareas son enviadas a unos esclavos, uno para encriptar y otro para desencriptar principalmente para maximizar procesos disminuyendo los costos en la comunicación y operación de los datos.




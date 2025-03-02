1. ¿Qué es y para qué sirve el mapa de memoria de un microprocesador?

El mapa de memoria de un microprocesador es una representación gráfica o esquemática de la distribución de la memoria en el sistema. Indica qué rangos de direcciones corresponden a la RAM, la ROM, los registros de entrada/salida y otros periféricos. Su propósito es definir cómo se organizan y acceden los datos en el sistema, asegurando que el procesador pueda leer y escribir información en los lugares correctos.  

2. Basándote en la figura 3, responde:
    1. ¿Cuántos pines del bus de direcciones del MC6802 se utilizan en esta conexión? ¿Cuáles son los nombres utilizados para representarlos?

        El MC6802 es un microprocesador de 8 bits con un bus de direcciones de 16 bits. Los pines del bus de direcciones suelen representarse como A0 - A15. Dependiendo de la conexión, se podrían estar utilizando los 16 pines si se accede a toda la memoria direccionable.

    2. ¿De qué valor es la memoria total de almacenamiento del MC6846? Incluye los cálculos que realizaste. 
        El MC6846 es un circuito periférico que incluye memoria y funciones de entrada y salida. Su capacidad de almacenamiento depende de la cantidad de líneas de dirección que maneje. 

    3. ¿Cuántos bits ocupa cada dato al que se puede acceder en la memoria MC6846? ¿Cómo lo dedujiste?

        El MC6846 maneja datos de 8 bits (1 byte) por cada dirección de memoria. Esto se deduce porque los microcontroladores de esa época trabajaban con buses de datos de 8 bits, lo que significa que cada acceso a la memoria lee o escribe 8 bits a la vez.


3. ¿Cuáles son las características más relevantes de la arquitectura von Newman y Harvard?

Arquitectura von Neumann

    1.  Usa un bus único para datos e instrucciones.
    2.  Accede a la memoria de manera secuencial, lo que puede causar cuellos de botella (problema de velocidad).
    3.  Es más flexible porque permite que los programas modifiquen datos y código en la misma memoria.
    4.  Se utiliza en computadoras tradicionales y muchos microprocesadores generales.

Arquitectura Harvard

    1.  Tiene buses separados para datos e instrucciones, permitiendo acceso simultáneo.
    2.  Es más rápida y eficiente, reduciendo el cuello de botella en la transferencia de datos e instrucciones.
    3.  Se usa en microcontroladores y DSPs (procesadores de señal digital), donde la velocidad es crucial.

4. ¿Cuáles son las características más relevantes de la arquitectura CISC y RISC?

CISC (Complex Instruction Set Computing)
Conjunto de instrucciones complejo con muchas operaciones especializadas.
Cada instrucción puede realizar múltiples tareas, reduciendo la cantidad de líneas de código.
Usa menos memoria para almacenar programas, pero las instrucciones son más lentas.
Ejemplo: Intel x86.

5. ¿Cuál es tu opinión sobre los tipos de arquitecturas que se observan en los microprocesadores?

 La arquitectura von Neumann es más fácil de implementar y flexible, mientras que la Harvard es más rápida para sistemas embebidos. Por otro lado, la diferencia entre CISC y RISC es clave en el rendimiento: CISC es ideal para computadoras de propósito general, mientras que RISC domina en dispositivos móviles y sistemas de alto rendimiento.




 1. ¿Cuántos pines del bus de direcciones del MC6802 se utilizan en esta conexión? ¿Cuáles son los nombres utilizados para representarlos?

 el microprocesador MC6802 tiene un bus de direcciones de 16 bits etiquetado como A0-A15. Sin embargo, en la conexión con el MC6846, se observa que se utilizan únicamente 11 líneas de dirección, etiquetadas como A0-A10, por lo tanto, en esta conexión específica, se utilizan 11 pines del bus de direcciones del MC6802.

2. ¿De qué valor es la memoria total de almacenamiento del MC6846? Incluye los cálculos que realizaste.

El MC6846 tiene una ROM interna de 2 KB, como se indica en el diagrama.

Podemos confirmar este valor utilizando el número de líneas de dirección:

Cálculo del tamaño de memoria direccionable
Se tienen 11 líneas de dirección (A0 - A10).
La cantidad de direcciones posibles en la memoria es:
2^{11}=2048
2048  direcciones
Como cada dirección almacena 1 byte, el tamaño total de la memoria es:
2048 bytes = 2KB

3. ¿Cuántos bits ocupa cada dato al que se puede acceder en la memoria MC6846? ¿Cómo lo dedujiste?

La memoria del MC6846 usa un bus de datos de 8 bits, lo que se indica en la conexión de los pines D0 - D7 entre el MC6802 y el MC6846, esto significa que cada dirección de memoria almacena 8 bits (1 byte), lo que es común en microprocesadores de 8 bits.

Se dedujo de la siguiente manera: 
    1.  En la imagen se muestra que los datos se transfieren a través del bus D0-D7, lo que indica que el ancho de palabra es de 8 bits.
    2.  Esto confirma que cada acceso a la memoria recupera o almacena 8 bits (1 byte) a la vez.

    
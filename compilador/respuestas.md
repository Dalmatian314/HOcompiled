EJERCICIO 1/2

1) Pre-processing:

-obtenemos el archivo: calculator.pp_c
-errores de escritura, sintaxis semantica, todo en orden

En el archivo :declara las funciones y a me dice que funciones son externas y que en un futuro habra que linkear

2)Primera compilacion

---traduce a assembler---es un lenguaje intermedio
se realizan optimizaciones(elimina cosas de mas, lengiaje mas sencillo)

En el archivo: se observa el programa en otro lenguaje assembler


3)Segunda compilacion 

---assembler a lenguaje de maquina
controles y optimizaciones  de memory management

crea el objeto---> genera los objetos en binario

Del archivo: tipeamos nm calculator.o y obtenemos que add_numbers y main están definidas, mientras que printf NO.

4) Link (exe)


tiene librerias, ahora traer toda la informacion que necesito
Tomar decision de como linkear dinamica o estatico

Cuando ejecutamos : I know how to add! 31 + 11 is 42

estatico---mas rapido


EJERCICIO 3

En el archivo calculator.asm identificamos:


call    add_numbers
call    printf


EJERCICIO 4


Se obtienen descriptor y entrada:


000000000000003c T add_numbers
0000000000000000 T main
                 U printf


printf sigue siendo U pero està linkeada a una librería (soname)

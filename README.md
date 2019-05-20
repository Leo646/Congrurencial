                                            Introducción
     
   En el siguiente documento se va a describir el funcionamiento de lo generadores congruenciales lineales, específicamente el generador “Congruencial mixto” a través de un  programa realizado en el lenguaje de programación Java.
Se explicara paso a paso en funcionamiento del programa así como el resultado que  arroja.
 
                                                  Desarrollo 
Generadores Congruenciales Lineales
   Estos son capaces de generar una secuencia de números pseudoaleatorios en el cual el próximo número pseudoaleatorio es determinado a partir del último número generado, es decir, el número pseudoaleatorio ![image](https://user-images.githubusercontent.com/33529768/57994095-29abb700-7a81-11e9-8d91-e16b55edf464.png) es derivado a partir del número pseudoaleatorio![image](https://user-images.githubusercontent.com/33529768/57994110-421bd180-7a81-11e9-9dde-c8ba0fef7c53.png)
	
 Para el caso particular del generador congruencial mixto, la relación de recurrencia es la siguiente ![image](https://user-images.githubusercontent.com/33529768/57994142-5e1f7300-7a81-11e9-8920-2035d44b8896.png)

Donde: 
	X0 = es la semilla. 
	a = es el multiplicador.
	c = es la constante aditiva.
	m = es el modulo.

Funcionamiento del  Programa del generador congruencial mixto
Para desarrollar el programa Congruencial mixto, se empieza creando clase que se va  a llamar “public class CongruencialMixto”. Dentro de la clase, se declaran la variables que se van a utilizar para el funcionamiento del programa y almacenamiento de los resultados, en este caso las variables para la semilla (X0),  el multiplicador (a), la constante aditiva (c), el modulo (m), el resultado del seudocódigo ![image](https://user-images.githubusercontent.com/33529768/57994095-29abb700-7a81-11e9-8d91-e16b55edf464.png) (Xn1) y el resultado del seudocódigo ![image](https://user-images.githubusercontent.com/33529768/57994110-421bd180-7a81-11e9-9dde-c8ba0fef7c53.png)  (xn).


![i](https://user-images.githubusercontent.com/33529768/57993554-244d6d00-7a7f-11e9-9104-de682b6b2ed5.jpg)

A continuación es necesario importa la clase Scanner,


![i2](https://user-images.githubusercontent.com/33529768/57993732-ddac4280-7a7f-11e9-9a79-cac44fd60884.jpg)

esta Clase permitirá ingresar datos a través del teclado y almacenarlas  en la variables anteriormente declaradas.

![i3](https://user-images.githubusercontent.com/33529768/57993781-06343c80-7a80-11e9-863a-a5a2efc289e3.jpg)

Una vez realizado los pasos anteriores, para que el programa funcione correctamente es necesario emplear un ciclo repetitivo, en este caso un ciclo for. Este permitirá que arroje una serie de resultado varias veces, hayas que se cumpla la condición que se le impuso en esta caso que inicie en 0 y sea menor a 8, es decir que imprima 7 veces los resultado deseados.  

![i4](https://user-images.githubusercontent.com/33529768/57993833-3bd92580-7a80-11e9-8e86-0bf8e626f367.jpg)


Dentro del ciclo for se escribe el código que dará funcionamiento al programa. Como ya se declararon las variable anteriormente, ahora solo se procede al desarrollo de las formulas.
En “xn1” se almacena el resultado de la fórmula:

![image](https://user-images.githubusercontent.com/33529768/57993876-717e0e80-7a80-11e9-9d41-708b915ea6af.png)
				
En “xn” se almacena el resultado del residuo de la formula

![image](https://user-images.githubusercontent.com/33529768/57993911-8fe40a00-7a80-11e9-8d2b-1747221c4aab.png)
			
En “nf” se almacena el resultado de xn1/m (modulo).

![image](https://user-images.githubusercontent.com/33529768/57993959-b73ad700-7a80-11e9-8db7-c4a995742767.png)

Todo este ciclo repetitivo permitirá imprimir, mediante un System.out.println, los resultados deseados, es decir cuando a=5, c7, X0=4, m=8, el programa arroja el siguiente resultado.

![image](https://user-images.githubusercontent.com/33529768/57994024-e3565800-7a80-11e9-94d2-aa0a502c981a.png)


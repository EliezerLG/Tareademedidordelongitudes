# Aplicaciones 
#### Este programa Calcula de centimetros a la siguentes medidas:
1. triple de pitagoras
2. Juego del ahorcado
###  Para ello se a basado en 3 codigos
*   Pseudocodigo
*   C++
*   Python
# Triple de Pitagoras
# Pseudocodigo
---
``` 
Proceso Triples_De_Pitagoras_menoresa_500
	//definimos nuestras variables que utilizaremos
    Definir limite, lado1, lado2, hipotenusa Como Entero
    limite <- 500
	
    Escribir "Triples de Pitagoras menores o iguales a ", limite, ":"
	//indicamos que lado1 es igual a 1
    lado1 = 1
	// minestras lado1 sea menor a nuestra variable limite
    mientras lado1 <= limite Hacer
		// debe de darle valor a lado2 con lado1 + 1
        lado2 = lado1 + 1
		// si el resulado de nuestra variable 2 es menor a limie
        mientras lado2 <= limite Hacer
			// el valor de hipotenusa debe de ser lado2+1
            hipotenusa = lado2 + 1
			// evaluamo hipotenusa que sea menor a limite 
            mientras hipotenusa <= limite Hacer
				//agregamos una condición donde comparara la suma de los cuadrados de los dos lados y el resultado hipotenusa al cuadrado
                Si lado1^2 + lado2^2 = hipotenusa^2 Entonces
					// si la condicion se cumple nos va Imprimir  el triple de pitagoras
                    Escribir "Lado1: ", lado1, ", Lado2: ", lado2, ", Hipotenusa: ", hipotenusa
                FinSi
				// acá indicamos que los valore deben ir aumentando de uno en uno.
                hipotenusa = hipotenusa + 1
            FinMientras
            lado2 = lado2 + 1
        FinMientras
        lado1 = lado1 + 1
    FinMientras
	//indicamos un mensaje cuando el programa alla terminado
    Escribir "Estos son los resultados encontrados. Gracias."
FinProceso

```
---
# C++
```
//Calculador de triple de pitagoras menores o iguales a 500
#include <iostream>
using namespace std;
int main() {
    //Variable limite en este caso hasta 500
    int limite = 500;
    //Imprimimos en pantalla el mensaje donde el usuario visualice el limite que tiene para generar las triples de pitagoras
    cout << "Triples de Pitagoras menores o iguales a " << limite << ":" << endl;
    // usamos un for en lado 1 que comience con valor "1" y le indicamos que si lado1 es menor o igual a nuetra variable limite osea "500"
    // que que aumente de 1 en 1   
    for (int lado1 = 1; lado1 <= limite; lado1++) {
        // anidamos un segundo for que nos va servir para el lado 2 el cual va comenzar con el valor de "lado1 + 1", para que lado 1 y lado 2
        // no sean iguales
        for (int lado2 = lado1 + 1; lado2 <= limite; lado2++) {
            //acá indicamos que el valor de la hipotenusa, es lado2 + 1; para compararlo con la suma de los lados
            for (int hipotenusa = lado2 +1; hipotenusa <= limite; hipotenusa++) {
                //aquí es donde comparamos la suma de los 2 lados sea igual al cuadrado de hipotenusa es decir hipotenusa por hipotenusa
                if (lado1 * lado1 + lado2 * lado2 == hipotenusa * hipotenusa ) {
                    // si se cumple la condición imprimimos el mensaje en pantalla del resultado encontrado,
                    cout << "Lado1: " << lado1 << ", Lado2: " << lado2 << ", Hipotenusa: " << hipotenusa << endl;
                }
            }
        }
    }
    // indicamos al usuario cuando allá terminado el calculo de la de los triples de pitagoras
    cout <<"Estos fueron los resultados encontrados Gracias."<< endl;

    return 0;
}


```
---
# Python
```
# Calculador de triples de Pitágoras menores o iguales a 500
limite = 500

# Imprimimos un mensaje donde el usuario ve el límite para generar los triples de Pitágoras
print("Triples de Pitagoras menores o iguales a", limite, ":")

# Usamos un for para lado1 que comience con el valor "1" y aumente de 1 en 1 hasta el límite (500)
for lado1 in range(1, limite + 1):
    # Anidamos un segundo for para lado2, que comienza con el valor de "lado1 + 1", para que lado1 y lado2 no sean iguales
    for lado2 in range(lado1 + 1, limite + 1):
        # en un 3ser for Indicamos que el valor de la hipotenusa es lado2 + 1 para compararlo con la suma de los lados
        for hipotenusa in range(lado2 + 1, limite + 1):
            # en un if Comparamos si esta condición que es la suma de los cuadrados de los lados es igual al cuadrado de la hipotenusa
            if lado1**2 + lado2**2 == hipotenusa**2:
                # Si se cumple la condición, imprimimos un mensaje con los resultados encontrados
                print(f"Lado1: {lado1}, Lado2: {lado2}, Hipotenusa: {hipotenusa}")

# Indicamos al usuario que se han encontrado todos los resultados
print("Estos son los resultados encontrados. Gracias.")
```
---

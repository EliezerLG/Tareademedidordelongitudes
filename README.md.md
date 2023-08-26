# Aplicacion para Calcular Longitudes
#### Este programa Calcula de centimetros a la siguentes medidas:
1. Metros
2. Yardas
3. Varas
4. Pulgadas
5. Pies
###  Para ello se a basado en 3 codigos
*   Pseudocodigo
*   C++
*   Python
# Pseudocodigo
``` PSEINT
Algoritmo calculador_centimetros_a_diferente_medidas
	Definir Centimetros, resultado Como Real
    Definir opciom, Otravez Como Caracter
	Repetir
		Escribir "Ingrese la cantidad de Centímetros (cm) que desea medir: "
		Leer Centimetros
		Escribir "Opciones para calcular:"
        Escribir "1. Metros"
        Escribir "2. Yardas"
        Escribir "3. Varas"
        Escribir "4. Pulgadas"
        Escribir "5. Pies"
		Escribir "Elija el número de opción que desee calcular: "
        Leer opciom
		Si opciom = "1" Entonces
			resultado = Centimetros / 100
			Escribir "El cálculo de ", Centimetros, " centímetros a metros es de: ", resultado, " metros"
		Fin Si
		Si opciom = "2" Entonces
			resultado = Centimetros / 91.44
            Escribir "El cálculo de ", Centimetros, " centímetros a yardas es de: ", resultado, " yardas"
		Fin Si
		Si opciom = "3" Entonces
			resultado = Centimetros / 83.5905
            Escribir "El cálculo de ", Centimetros, " centímetros a varas es de: ", resultado, " varas"
		Fin Si
		Si opciom = "4" Entonces
			resultado = Centimetros / 2.54
            Escribir "El cálculo de ", Centimetros, " centímetros a pulgadas es de: ", resultado, " pulgadas"
		Fin Si
		Si opciom = "5" Entonces
			resultado = Centimetros / 30.48
            Escribir "El cálculo de ", Centimetros, " centímetros a pies es de: ", resultado, " pies"
		Fin Si
		Escribir "¿Desea realizar otro cálculo? Presione (S) para continuar o cualquier tecla para salir: "
        Leer Otravez
	Hasta Que Otravez <> "S" Y Otravez <> "s"
FinAlgoritmo
```
---
# C++
```
//Calulador de centimetros a diferentes longitudes.
# include <iostream>
using namespace std;
int main () {
    double Centimetros, resultado, opcion;
    char Otravez;
    do {
            cout <<"Ingrese la cantidad de Centrimetros (cm), que desea medir.";
    cin >> Centimetros;
    //Le indicamos al usuario la opciones que tine para calcular
    cout << "Opciones para calcular: \n";
    cout << "1. Metros \n";
    cout << "2. Yardas \n";
    cout << "3. Varas \n";
    cout << "4. Pulgdas \n";
    cout << "5. Pies \n";
    cout << "Elija el numero de opcion que desee calcular: \n";
    cin >> opcion;
    //Aca es donde calculamos las opciones que alla elegido el usuario
    if (opcion == 1) {
        resultado = Centimetros / 100;
        cout <<"El calculo de " << Centimetros <<  " Centimetros a Metros es de : " << resultado << " Metros \n";
    }
     else if (opcion == 2) {
        resultado = Centimetros / 91.44;
       cout <<"El calculo de " << Centimetros <<  " Centimetros a Yardas es de : " << resultado << " Yardas \n";
    }
     else if (opcion == 3) {
        resultado = Centimetros / 83.5905;
        cout <<"El calculo de " << Centimetros <<  " Centimetros a Varas es de : " << resultado << " Varas \n";
    }
     else if (opcion == 4) {
        resultado = Centimetros / 2.54;
        cout <<"El calculo de " << Centimetros <<  " Centimetros a Pulgadas es de : " << resultado << " Pulgadas \n";
    }
     else if (opcion == 5) {
        resultado = Centimetros / 30.48;
        cout <<"El calculo de Centimetros " << Centimetros << "a Pies es de : " << resultado << " Pies \n";
    }
    else{
        cout <<"Debe de tomar un curso de lectura intensivo\n";
    }
    //para realizar otro calculo
    cout << "¿Desea realizar otro calculo? Presione(S) de lo contrario presione cualquier tecla diferente para salir: ";
    cin >> Otravez;
    } while (Otravez == 'S' || Otravez == 's'); 
    cout << "Gracias por utilizar el programa.\n";
    return 0;
}
```
---
# Python
```
while True:
    Centimetros = float(input("Ingrese la cantidad de Centímetros (cm) que desea medir: "))
    
    print("Opciones para calcular:")
    print("1. Metros")
    print("2. Yardas")
    print("3. Varas")
    print("4. Pulgadas")
    print("5. Pies")
    
    opcion = int(input("Elija el número de opción que desee calcular: "))
    
    if opcion == 1:
        resultado = Centimetros / 100
        print(f"El cálculo de {Centimetros} centímetros a metros es de: {resultado} metros")
    elif opcion == 2:
        resultado = Centimetros / 91.44
        print(f"El cálculo de {Centimetros} centímetros a yardas es de: {resultado} yardas")
    elif opcion == 3:
        resultado = Centimetros / 83.5905
        print(f"El cálculo de {Centimetros} centímetros a varas es de: {resultado} varas")
    elif opcion == 4:
        resultado = Centimetros / 2.54
        print(f"El cálculo de {Centimetros} centímetros a pulgadas es de: {resultado} pulgadas")
    elif opcion == 5:
        resultado = Centimetros / 30.48
        print(f"El cálculo de {Centimetros} centímetros a pies es de: {resultado} pies")
    else:
        print("Debe de tomar un curso de lectura intensivo ")
    
    Otravez = input("¿Desea realizar otro cálculo? Presione (S) para continuar o cualquier tecla para salir: ")
    if Otravez.upper() != 'S':
        break

print("Gracias por utilizar el programa Python.")
```
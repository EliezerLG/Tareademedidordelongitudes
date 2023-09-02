# Aplicaciones 
#### Este programa Calcula de centimetros a la siguentes medidas:
1. Triangulo Rectangulo
###  Para ello se a basado en 3 codigos
*   C++
# Triangulos Rectangulos
---
# C++
```
//asi arriba
#include <iostream>
using namespace std;

int main() {
    int altura;

    cout << "Ingrese la altura del triángulo: ";
    cin >> altura;

    for (int i = 1; i <= altura; i++) {
        for (int j = 1; j <= i; j++) {
            cout << "* ";
        }
        cout << endl;
    }

    return 0;
}


```
```
//asia abajo
#include <iostream>
using namespace std;

int main() {
    int altura;

    cout << "Ingrese la altura del triángulo: ";
    cin >> altura;

    for (int i = altura; i >= 1; i--) {
        for (int j = 1; j <= i; j++) {
            cout << "* ";
        }
        cout << endl;
    }

    return 0;
}

```
```
//asi la derecha
#include <iostream>
using namespace std;

int main() {
    int altura;

    cout << "Ingrese la altura del triángulo: ";
    cin >> altura;

    for (int i = 1; i <= altura; i++) {
        for (int j = 1; j <= altura - i; j++) {
            cout << "  ";
        }
        for (int k = 1; k <= i; k++) {
            cout << "* ";
        }
        cout << endl;
    }

    return 0;
}

```
```
//asia la izquierda
#include <iostream>
using namespace std;

int main() {
    int altura;

    cout << "Ingrese la altura del triángulo: ";
    cin >> altura;

    for (int i = 1; i <= altura; i++) {
        for (int j = 1; j <= i; j++) {
            cout << "* ";
        }
        cout << endl;
    }

    return 0;
}

```
---

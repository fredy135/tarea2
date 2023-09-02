### triangulos en pseudocodigo

    Algoritmo triangulos
        Definir i,j,n Como Entero
        Escribir "ingresa un numero entero positivo"
        leer n
        Escribir "ingresa el numero de opcion que desees"
        Escribir "opcion 1"
        Escribir "opcion 2"
        Leer op
        Si op >= 1 y op <= 4 Entonces
            si op = 1 Entonces
                Para i = 1 Hasta n Con Paso 1 Hacer
                    Para j = 1 Hasta i Con Paso 1 Hacer
                        Escribir "*"," " Sin Saltar
                    FinPara
                    Escribir ""
                FinPara
            FinSi
            si op = 2 Entonces
                para i = n Hasta 1 con paso -1 Hacer
                    para j = 0 Hasta n Con Paso -1 Hacer
                        escribir " " Sin Saltar
                    FinPara
                    para j = 1 Hasta i Con Paso 1 Hacer
                        escribir "*"," " Sin Saltar
                    FinPara
                    Escribir ""
                FinPara
            FinSi
        FinSi
    FinAlgoritmo
___

### triangulos en c++

    #include <iostream>

    int main() {
        int i, j, n, op;

        std::cout << "Ingresa un número entero positivo: ";
        std::cin >> n;

        std::cout << "Ingresa el número de opción que desees:\n";
        std::cout << "1. Opción 1\n";
        std::cout << "2. Opción 2\n";
        
        std::cin >> op;

        if (op >= 1 && op <= 2) {
            if (op == 1) {
                for (i = 1; i <= n; i++) {
                    for (j = 1; j <= i; j++) {
                        std::cout << "* ";
                    }
                    std::cout << "\n";
                }
            } else if (op == 2) {
                for (i = n; i >= 1; i--) {
                    for (j = 0; j < n - i; j++) {
                        std::cout << "  ";
                    }
                    for (j = 1; j <= i; j++) {
                        std::cout << "* ";
                    }
                    std::cout << "\n";
                }
            }
        } else {
            std::cout << "Opción no válida. Debes seleccionar 1 o 2.\n";
        }

        return 0;
    }
___
### triangulos en python

    n = int(input("Ingresa un número entero positivo: "))
    print("Ingresa el número de opción que desees:")
    print("1. Opción 1")
    print("2. Opción 2")
    op = int(input())

    if 1 <= op <= 2:
        if op == 1:
            for i in range(1, n + 1):
                for j in range(1, i + 1):
                    print("* ", end="")
                print()
        elif op == 2:
            for i in range(n, 0, -1):
                for j in range(0, n - i):
                    print("  ", end="")
                for j in range(1, i + 1):
                    print("* ", end="")
                print()
    else:
        print("Opción no válida. Debes seleccionar 1 o 2.")
___
___

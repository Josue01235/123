#include <iostream>

using namespace std;

int main()
{
    double centimeters;
    std::cout << "Ingrese la longitud en centimetros: ";
    std::cin >> centimeters;

    int choice;
    std::cout << "Elija la unidad a la que desea convertir:\n";
    std::cout << "1. Metros\n";
    std::cout << "2. Yardas\n";
    std::cout << "3. Varas\n";
    std::cout << "4. Pulgadas\n";
    std::cout << "5. Pies\n";
    std::cout << "Ingrese su elección: ";
    std::cin >> choice;

    double result;
    
    switch (choice) {
        case 1:
            result = centimeters * 0.01;
            std::cout << result << " metros." << std::endl;
            break;
        case 2:
            result = centimeters * 0.0109361;
            std::cout << result << " yardas." << std::endl;
            break;
        case 3:
            result = centimeters * 083.59;
            std::cout << result << " varas." << std::endl;
            break;
        case 4:
            result = centimeters * 0.393701;
            std::cout << result << " pulgadas." << std::endl;
            break;
        case 5:
            result = centimeters * 0.0328084;
            std::cout << result << " pies." << std::endl;
            break;
        default:
            std::cout << "Opción no válida." << std::endl;
    }

    return 0;
}


-------------------------------------------------------------------

```python
centimeters = float(input("Ingrese la longitud en centimetros: "))

print("Elija la unidad a la que desea convertir:")
print("1. Metros")
print("2. Yardas")
print("3. Varas")
print("4. Pulgadas")
print("5. Pies")
choice = int(input("Ingrese su elección: "))

result = 0

if choice == 1:
    result = centimeters * 0.01
    print(result, "metros.")
elif choice == 2:
    result = centimeters * 0.0109361
    print(result, "yardas.")
elif choice == 3:
    result = centimeters * 0.8359
    print(result, "varas.")
elif choice == 4:
    result = centimeters * 0.393701
    print(result, "pulgadas.")
elif choice == 5:
    result = centimeters * 0.0328084
    print(result, "pies.")
else:
    print("Opción no válida.")

-------------------------------------------------------------------

## Convertidor de Longitud en Pseudocódigo  

1. Definir `centimeters` y `result` como números reales.
2. Definir `choice` como número entero.
   
3. Escribir "Ingrese la longitud en centímetros: "
4. Leer `centimeters`
   
5. Escribir "Elija la unidad a la que desea convertir:"
   - 1. Metros
   - 2. Yardas
   - 3. Varas
   - 4. Pulgadas
   - 5. Pies
6. Escribir "Ingrese su elección: "
7. Leer `choice`
   
8. Si `choice` es igual a 1 Entonces
     - `result` = `centimeters` * 0.01
     - Escribir `result`, " metros."
   
9. Sino Si `choice` es igual a 2 Entonces
     - `result` = `centimeters` * 0.0109361
     - Escribir `result`, " yardas."
   
10. Sino Si `choice` es igual a 3 Entonces
      - `result` = `centimeters` * 0.8359
      - Escribir `result`, " varas."
   
11. Sino Si `choice` es igual a 4 Entonces
      - `result` = `centimeters` * 0.393701
      - Escribir `result`, " pulgadas."
   
12. Sino Si `choice` es igual a 5 Entonces
      - `result` = `centimeters` * 0.0328084
      - Escribir `result`, " pies."
   
13. Sino
      - Escribir "Opción no válida."
   
14. Fin Si

Fin Algoritmo

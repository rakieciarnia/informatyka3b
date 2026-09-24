# Sprawdzian 1 – Typy danych i instrukcje warunkowe

Rozwiązania zadań spakuj do pliku `.zip` i prześlij na adres: `sprawdzian@rakieciarnia.pl`.
Zadanie 3\* jest dla chętnych na ocenę 6. Możesz je zrobić zamiast zadania 2.

---

### Zadanie 1
Znajdź 3 błędy w poniższym kodzie. Załącz poprawiony kod z komentarzem wyjaśniającym, co zostało poprawione.

```cpp
#include <iostream>
using namespace std;

int main() {
    int x = 5.5;
    char znak = "A";
    
    if (x = 10) {
        cout << "X wynosi 10" << endl;
    }
    
    return 0;
}
```

---

### Zadanie 2
Napisz program, który pobierze od użytkownika dwie liczby zmiennoprzecinkowe oraz jeden znak operacji arytmetycznej (`+`, `-`, `*`, `/`). Użyj instrukcji `switch`, aby w zależności od wybranego znaku wykonać odpowiednie działanie i wypisać wynik. Zabezpiecz program przed dzieleniem przez zero – jeśli druga liczba wynosi `0` przy dzieleniu, wypisz komunikat: `"Nie można dzielić przez zero!"`. Dodaj przypadek `default`, który obsłuży podanie nieznanego znaku operacji.

---

### Zadanie 3\* *(dla chętnych)*
Napisz program, który wczytuje numer miesiąca (`1-12`) oraz rok i zwraca liczbę dni w danym miesiącu. Za pomocą instrukcji `switch` określ, ile dni ma podany miesiąc. Jeśli podanym miesiącem jest **luty (2)**, program musi sprawdzić, czy podany rok jest przestępny. Rok jest przestępny, jeśli jest **podzielny przez 4 i nie jest podzielny przez 100**, **LUB** jest **podzielny przez 400**.

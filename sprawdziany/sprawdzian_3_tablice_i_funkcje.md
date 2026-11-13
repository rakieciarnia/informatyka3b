# Sprawdzian 3 – Tablice i funkcje

Rozwiązania zadań (tylko pliki `.cpp`) prześlij na adres: `sprawdzian@rakieciarnia.pl` po uprzednim zgłoszeniu, że kod jest gotowy i przystępujesz do wysyłania.
Możesz używać kompilatora i swoich programów napisanych na poprzednich lekcjach. Nie korzystaj z internetu i telefonu - przyłapanie skutkuje natychmiastową oceną niedostateczną bez możliwości poprawy, nawet jeśli nie było to korzystanie w celu pomocy z rozwiązaniem sprawdzianu.
Zadanie 3\* jest dla chętnych na ocenę 6. Możesz je zrobić zamiast zadania 2. 

---

### Zadanie 1
Znajdź 3 błędy w poniższym kodzie. Załącz poprawiony kod z komentarzem wyjaśniającym, co zostało poprawione.

```cpp
#include <iostream>
using namespace std;

void zmienLiczbe(int x) {
    x = 100;
}

int main() {
    int tablica[3] = {10, 20, 30};
    
    zmienLiczbe(tablica[3]);
    
    cout << "Nowa wartosc: " << tablica[3] << endl;
    
    return 0;
}
```

---

### Zadanie 2
Napisz program, który sprawdzi, czy podana tablica dwuwymiarowa o wymiarach $4 \times 4$ (wypełniona liczbami całkowitymi) jest **symetryczna względem głównej przekątnej**.

**Jak to rozumieć?**
Wyobraź sobie przekątną biegnącą od lewego górnego rogu tablicy do prawego dolnego rogu. Tablica jest symetryczna wtedy, gdy elementy leżące lustrzanie po obu stronach tej przekątnej są sobie równe (czyli element z pierwszego wiersza i drugiej kolumny musi być taki sam jak element z drugiego wiersza i pierwszej kolumny, itd.).

**Przykład tablicy symetrycznej:**
```text
1  5  3  8
5  2  0  4
3  0  7  9
8  4  9  6
```

**Wymagania:**
- Wczytaj dane do tablicy od użytkownika lub wpisz je na sztywno w kodzie do przetestowania.
- Podziel program na funkcje (osobna funkcja do wyświetlania tablicy i osobna funkcja sprawdzająca warunek symetrii).
- Wyświetl tablicę w konsoli oraz wypisz jednoznaczny komunikat, czy jest ona symetryczna.

---

### Zadanie 3\*
Napisz program realizujący **mnożenie dwóch macierzy** (tablic dwuwymiarowych) o wymiarach $3 \times 3$, którego wynikiem jest trzecia tablica o tych samych wymiarach.

**Jak oblicza się wartości w tablicy wynikowej?**
Aby obliczyć pojedynczą komórkę w nowej tablicy (na przecięciu wybranego wiersza i wybranej kolumny), bierzesz cały odpowiadający jej **wiersz z pierwszej tablicy** oraz całą odpowiadającą jej **kolumnę z drugiej tablicy**. Mnożysz kolejne liczby z tego wiersza przez kolejne liczby z tej kolumny, a następnie sumujesz te iloczyny.

**Wizualizacja obliczenia komórki w 1. wierszu i 2. kolumnie:**

```text
   Tablica A (wiersz 1)       Tablica B (kolumna 2)        Tablica Wynikowa
  ┌────────────────────┐     ┌────────────────────┐      ┌────────────────────┐
  │ [2]    [3]    [4]  │     │  1     [5]     2   │      │  .     [13]    .   │
  │  1      0      2   │  x  │  3     [1]     4   │  =   │  .      .      .   │
  │  4      1      3   │     │  2     [0]     1   │      │  .      .      .   │
  └────────────────────┘     └────────────────────┘      └────────────────────┘

  Obliczenie dla zaznaczonej komórki [13]:
  (2 * 5) + (3 * 1) + (4 * 0) = 10 + 3 + 0 = 13
```

**Wymagania:**
- Przygotuj dwie tablice $3 \times 3$ wypełnione liczbami całkowitymi oraz trzecią tablicę na wynik.
- Zaprojektuj program z podziałem na funkcje (wyświetlanie tablicy oraz obliczanie wyniku mnożenia).
- Wyświetl na ekranie obie tablice wejściowe oraz obliczoną tablicę wynikową.

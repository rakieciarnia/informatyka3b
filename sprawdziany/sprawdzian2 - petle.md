# Sprawdzian 2 – Pętle

Rozwiązania zadań (tylko pliki `.cpp`) prześlij na adres: `sprawdzian@rakieciarnia.pl` po uprzednim zgłoszeniu, że kod jest gotowy i przystępujesz do wysyłania.
Możesz używać kompilatora i swoich programów napisanych na poprzednich lekcjach. Nie korzystaj z internetu i telefonu - przyłapanie skutkuje natychmiastową oceną niedostateczną bez możliwości poprawy, nawet jeśli nie było to korzystanie w celu pomocy z rozwiązaniem sprawdzianu.
Zadanie 3\* jest dla chętnych na ocenę 6. Możesz je zrobić zamiast zadania 2. 

---

### Zadanie 1
Opisz krótko co robi poniższy program.
```cpp
#include <iostream>
using namespace std;

int main() {
    int a = -7;

    if (a < 0) {
        a = a * (-1);
    }

    cout << a << endl;

    return 0;
}
```

---

### Zadanie 2
Napisz program, który pobiera od użytkownika 10 liczb całkowitych. Program powinien:
- policzyć, ile wprowadzonych liczb jest podzielnych przez 3,
- policzyć, ile liczb jest większych od 0,
- obliczyć sumę liczb ujemnych,
- wyświetlić najmniejszą spośród wprowadzonych liczb,
- po zakończeniu wczytywania wyświetlić wszystkie obliczone wyniki.

---

### Zadanie 3\*
Napisz program, który wypisze wszystkie liczby dwucyfrowe, których suma cyfr wynosi 10. Program powinien dodatkowo policzyć, ile takich liczb znaleziono.
Nie wypisuj liczb ręcznie, znajdź je za pomocą pętli.

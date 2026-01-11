# Metody numeryczne — mapa myśli
**Na samym dole jest notatka o stabilności oraz zbieżności - nie ma tego na mapie myśli**

<img width="1524" height="1142" alt="image" src="https://github.com/user-attachments/assets/7f0737e0-400c-4440-978f-bb253456566c" />


## Po co metody numeryczne?
Metody numeryczne służą do rozwiązywania problemów matematycznych, dla których:
- nie istnieje rozwiązanie analityczne,
- rozwiązanie analityczne jest zbyt skomplikowane,
- interesuje nas rozwiązanie przybliżone z kontrolowanym błędem.

Stosowane m.in. w:
- całkach,
- równaniach algebraicznych i różniczkowych,
- macierzach,
- analizie funkcji (miejsca zerowe, ekstrema).
---

## Błędy numeryczne

Każde rozwiązanie numeryczne obarczone jest błędem.

### Rodzaje błędów:
- błąd bezwzględny  
- błąd względny  

### Przyczyny błędów:
- błędy zaokrągleń  
- zaszumione dane wejściowe  
- dyskretyzacja problemu  
- niestabilność algorytmu  

---

## Równania

### Równania liniowe (Ax = b)
- Eliminacja Gaussa  
- Rozkład LU  

### Równania nieliniowe (f(x) = 0)
- metoda bisekcji  
- metoda stycznych (Newtona)  
- metoda siecznych  

### Równania różniczkowe (y' = f(x, y))
- metoda Eulera  
- metoda Rungego–Kutty  
- metoda trapezów  

---

## Całki

**Całkowanie numeryczne** – przybliżone obliczanie całki jako sumy pól pod wykresem.

### Metody:
- metoda prostokątów  
- metoda trapezowa  
- metoda Simpsona  

---

## Macierze

Metody numeryczne macierzy służą do obliczeń, które są kosztowne lub niemożliwe analitycznie.

- liczenie wyznacznika  
- odwracanie macierzy  
- eliminacja Gaussa-Jordana  

---

## Interpolacja

**Interpolacja** – wyznaczanie funkcji, która **dokładnie przechodzi przez wszystkie dane punkty**.

Stosowane metody:
- interpolacja wielomianowa Newtona  
- interpolacja wielomianowa Lagrange’a  

---

## Aproksymacja

**Aproksymacja** – wyznaczanie funkcji, która **najlepiej przybliża dane**, minimalizując błąd i **nie przechodząc dokładnie przez wszystkie punkty**.

Metody:
- aproksymacja średniokwadratowa  
- aproksymacja macierzowa  
- metody gradientowe  

---

## Stabilność algorytmu

**Stabilność numeryczna** oznacza, że:
> małe błędy danych wejściowych lub zaokrągleń nie powodują dużych błędów w wyniku.

Algorytm stabilny:
- nie wzmacnia błędów obliczeń,
- daje podobne wyniki dla lekko zmienionych danych.

Algorytm niestabilny:
- może gwałtownie zwiększać błąd,
- prowadzi do całkowicie błędnych wyników mimo poprawnych danych.

---

## Zbieżność algorytmu

**Zbieżność** oznacza, że:
> kolejne przybliżenia rozwiązania coraz bardziej zbliżają się do rozwiązania dokładnego.

Algorytm zbieżny:
- przy zwiększaniu liczby iteracji daje coraz dokładniejszy wynik,
- dąży do rozwiązania dokładnego.

Algorytm niezbieżny:
- oscyluje,
- rozbiega się,
- nie prowadzi do poprawnego rozwiązania.

---

## Relacja: stabilność vs zbieżność
- Algorytm może być zbieżny, ale niestabilny.
- Algorytm stabilny daje wiarygodne wyniki numeryczne.
- W praktyce potrzebna jest **zarówno zbieżność, jak i stabilność**.

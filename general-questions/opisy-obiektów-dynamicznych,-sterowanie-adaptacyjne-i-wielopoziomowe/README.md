# 1. Obiekt dynamiczy

**Obiektem dynamicznym** nazywa sie uklad fizyczny, techniczny lub abstrakcyjny, ktorego stan oraz wyjscie w danej chwili czasu zaleza nie tylko od aktualnych wartosci sygnalow wejsciowych, lecz rowniez od ich historii, a takze od stanu poczatkowego ukladu.

Innymi slowy, obiekt dynamiczny posiada *pamiec* – jego zachowanie jest determinowane przez cala przeszlosc sygnalow wejsciowych, a nie tylko przez ich wartosc biezaca.

**Przykład:**

Obiekt statyczny
- rezystor
  - wejście - napięcie podane
  - wyjście - prąd zmierzony na nim
    
*nie musimy czekać jego odpowiedź następuje natychmiastowo a jego poprzedni stan czy stan początkowy jest nie istotny (mówiąc o idealnym rezystorze)*

Obiekt dynamiczny 
- obiekt cieplny (np. pomieszczenie)
  - wejście - moc na grzejniku
  - wyjście - temperatura pomieszczenia
*chwile czasu zajmuje by temperatura grzejnika i pomieszczenia się ustabilizowała*


*Poniżej przykładowa (real szit badanie) odpowiedź skokowa obiektu dynamicznego cieplnego*
<img width="1200" height="500" alt="skok_zoom" src="https://github.com/user-attachments/assets/d431bb58-6d88-4318-9b18-f9ca2b30b5fa" />

## 1.1 Klasyfikacja obiektów dynamicznych

- Liniowe - Nieliniowe
  - ze względu na spełnienie zasady superpozycji
- Stacjonarne - Niestacjonarne
  - ze względu an to czy parametry obiektu się zmieniają w czasie
- Deterministyczne - Niederministyczne
  - ze względu na to czy obiekt posiada elementy losowości (np. szum)
- Ciągłe - Dyskretne
  - ze względu na dziedzinę czasu
- Jednowymiarowe - Wielowymiarowe
  - ze względu na liczbę sygnałów (SISO - single input single output, MIMO - multiple input multiple output, SIMO, MISO)


### Zasada superpozycji *na szybko*

Obiekt (uklad) jest **liniowy**, jezeli spelnia **zasade superpozycji**, ktora sklada sie z dwoch wlasnosci:
1. **skalowalnosc (jednorodnosc)**
   
   <img width="196" height="35" alt="Zrzut ekranu 2026-01-12 202735" src="https://github.com/user-attachments/assets/0a9524ac-ba47-4d0c-be8c-ebed2788cce5" />
3. **sumowanie sygnalow (addytywnosc)**
   
   <img width="349" height="37" alt="Zrzut ekranu 2026-01-12 202746" src="https://github.com/user-attachments/assets/784f74ce-c19d-4b36-b02a-aeb70efd408f" />

**funkcje nieliniowe**
-naturalnie obiekt nie może składać się z funkcji nieliniowych np. trygonometrycznych czy wykładniczych


## 1.2 Sterowanie adaptacyjne

**Sterowanie adaptacyjne** to metoda sterowania, w której regulator dopasowuje parametry (które
ulegają zmianie lub na początku są niepewne). Przykładowo podczas lotu masa samolotu, na skutek
zużycia paliwa, powoli zmniejsza się - potrzebna jest wiec zasada sterowania, która sama się dostosuje do takich zmiennych warunków.

**Przykład:**
Parametry PID zmieniają się w czasie bo obiekt jest jakiś dziwny (przez to że np. jest nieliniowy lub obiekt jest niestacjonarny) i to poprawia jego sterowanie

## 1.3 Sterowanie wielopoziomowe

**Sterowanie wielopoziomowe** to koncepcja zarządzania złożonymi systemami polegająca na
podziale zadania sterowania na warstwy o różnym stopniu decyzyjności i różnych horyzontach czasowych.

Z tym pojęciem często wiąże się pojęcie dekompozycji czyli rozdzielenia obiektu na pomniejsze (np. nieliniowego na pomniejsze liniowe lub takie które poprostu łatwiej nam ogarnąć)

**Przykład:**

Manipulator

1. Decyzja o trajektorii
2. Regulacja ruchu (położenia)
3. Sterowanie niskopoziomowe (regulacja PWM, przyśpieszenie itp.)

## 1.4 Dodatek dla przypomnienia bo ostrzegała nas prowadząca seminaria

**Układ sprzężenia zwrotnego**

*poniżej przykład schematu blokowego układu z zamkniętym ujemnym sprzężeniem zwrotnym (w tym przypadku w miejscu regulatora można dać PID)*
<img width="1462" height="368" alt="Zrzut ekranu 2026-01-08 162422" src="https://github.com/user-attachments/assets/f398c476-3b89-46d4-b051-db317c1448de" />

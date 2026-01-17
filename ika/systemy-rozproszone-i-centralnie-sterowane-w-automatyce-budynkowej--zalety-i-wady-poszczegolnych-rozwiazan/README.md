# 1. Systemy centralnie sterowane

Jedno centralne urządzenie sterujące (sterownik / serwer), do którego podłączone są wszystkie czujniki i elementy wykonawcze.

Zalety:

- prosta koncepcja
- łatwe zarządzanie
- tańsze
- prosta diagnostyka

Wady:

- utrata urządzenia sterującego powoduje zatrzymanie pracy
- słaba skalowalność
- duża ilość okablowania (topologia gwiazdy)
- duże obciążenie sieci (np. dane trafiają najpeirw z czujnika do centrali potem do aktuatora)

Wykorzystania:

- PLC - jako główny sterownik
- tanie smart home


# 2. Systemy rozproszone

Sterowanie realizowane jest przez wiele autonomicznych urzadzen, ktore komunikuja sie między sobą

Zalety:

- przy awarii jednego urządzenia rezsta działa
- dobrze skalowalny
- mniej okablowania
- mniejsze obciążenie sieci

Wady:

- każde pojedyncze urządzenie ma dość duży koszt
- cięższa konfiguracja
- trudniejsze zarządzanie

Wykorzystania:

- KNX - rozproszony
- BACnet (DDC) - centralny lub rozproszony

# 3. Systemy hybrydowe

W praktyce stosowane są jednak modele hybrydowe łączące plusy obydwu rozwiązań

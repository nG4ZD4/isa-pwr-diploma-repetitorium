# 1. Przewodowe

Protokoły przewodowe charakteryzują się duża przpustowością, niezawodnością, oraz bezpieczeństwem

### Przemysł:

EtherCAT

- Ethernet zmodyfikowany (EtherCAT)
- Prędkość bardzo wysoka
- czas rzeczywisty
- Master/Slave

**Modbus**

- Prosta implementacja
- Brak mechanizmów bezpieczeństwa
- Master/Slave
- Brak sztywnej topologii
- Prędkość niska

wariant RTU

- Bajty binarnie osmiobitowo (dwa znaki ASCII)
- Odstęp między ramkami mniej niż sekunda

wariant ASCII

- Bajty wysyłane szesnastkowo
- Odstęp między ramkami 3,5 czas znaku

wariant TCP/IP

- Wykorzytuje Ethernet i niesię za sobą jego plusy i minusy

**Profibus**

- Mster/slave
- Czas rzeczywisty
- Max 127 sterowników
- Topologia magistrali
- Prędkosć średnia

**Profinet**

- Ethernet przemysłowy
- prędkość niska
- Czas rzeczywisty

### Automatyka budynkowa:

**KNX**

- Multimaster
- Magistrala/Drzewo
- Prędkość niska
- Bardzo popularny standard europejski

**Modus**

wykorzystywany wa automatyce budynkowej jako protokół pomocniczy nie systemowy

- liczniki energii
- Falowniki
- Pompy
- Kotły

**DALI**

- Master/Slave
- Wolna komunikacja
- Jest zazwyczaj podsystemem do oświetlenia
- Zasilanie i komunikacja tym samym przewodem

# 2. Bezprzewodowe

Protokoły bezprzewodowe mają mniejszą przepustowość są mniej bezpieczne, a jakosć sygnału zależna jest od rodzaju pomieszczenia i przeszkód

**Przemysł:**

dyskusyjna technologia z racji na wysokie ryzyko utraty danych w procesie co w przemyśle może być kluczowe

**WirelessHART**

- czujniki w trudnodostępnych miejscach
- wysoka niezawodność (jak na bezprzewodówkę)
- Niskie zużycie energii
- Niskie prędkości
- Nie nadaje się do sterowania
- Drogi

**WiFi**

- wykorzystanie przy HMI
- wysoka przepustowość
- powszechny standard
- słaba niezawodność

LoRa WAN

- Bardzo duży zasięg
- Minimalny pobór energii
- Bardzo niska prędkość

**Automatyka budynkowa:**

**Zigbee**

- Radio 2.4 GHz
- Niska prędkość
- Zasięg średni

**WiFi**

- Radio
- Wysoka prędkość
- Zasięg średni

**KNX RF**

- Radio sub-GHz
- Pod sieć KNX
- Zasięg bardzo niski

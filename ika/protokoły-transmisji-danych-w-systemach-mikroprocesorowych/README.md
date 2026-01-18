# Co to są protokoły

Zestaw zasad określających:
- sposób kodowanie
- synchronizacja nadajnik-odbiornik
- kolejność bitów/bajtów (little/small endian)
- wykrywanie błędów

# Podział:

## Szeregowe:

- dane bit po bicie
- mało linii sygnałowych

### Najważniejsze protokoły szeregowe:

**UART** - 

- asynchroniczny
- brak zegara
- prosty i tani
- brak adresowania i korekscji błędów

Linie:
RX - receive
TX - transmit

**SPI** - Special periferial interface

- synchroniczny
- bardzo szybki
- master-slave

Linie:

MOSI - master wysyłą dane
MISO - slave odpowiada
SCK - master -> zegar
CS - wybiera urządzenie (tyle wyjsć ile urządzeń)

**I2C**

- synchroniczny
- adresowanie urządzeń
- wielu slave najednej magistrali
- wolniejszy niż SPI

Linie:

SDA - dane
SCL - zegar

**CAN**

- deterministyczny
- wysoka odpornmość na zakłócenia
- wykrywanie błędów (detekcja i korekcja)
- arbitraż priorytetowy
- magistrala

Linie:

*Skrętka czyli przeciwny sygnał między przewodami w celu redukcji pomiaru różnicy sygnałów co pomaga zniwelować wpływ zakłóceń*

CAN Hi 
CAN lo 

Rownoległe:

- dane przesyłane jednosześnie wieloma liniami
- szybkie, ale dużo pinów
- rzadko stoswane

**GPIO**

- można wykorzystać całe rejestry portów do włąsnego protokołu równoległego (np. PORTA, PORTB)
- pojedyncze wyjścia (np. porty w arduiono do zapalenia LED)

**Magistrala danyc pamięci**

- RAM
- ROM

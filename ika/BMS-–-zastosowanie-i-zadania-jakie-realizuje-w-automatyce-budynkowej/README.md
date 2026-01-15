**BMS** - Building Management System to system pozwalający na centralne zarządzanie instalacjami 
budynkowymi w biurowcach czy hotelach (nie mylić ze smart home)

**Systemy zamknięte:** system automatyki budynkowej zaprojektowany przez jednego producenta dający 
gwarancję kompatybilności firmowych sprzętów` z ograniczonymi możliwościami łączności z innymi systemami.

**Systemy otawrte:** Wykorzystujące otwarte protokoły co zwiększa elastyczności. Wadą jest skomplikowana konfiguracja.

Zastosowania:

- oświetlenie
- ogrzewanie
- wentylacja
- HVAC
- systemy alarmowe
- monitoring zużycia energii

Zadania:

- zwiększenie komfortu użytkowników
- poprawa bezpieczeństwa
- poprawa efektywności energetycznej
- optymalizację kosztów użytkowych
- ciągłe monitorowanie i kontrola elementów systemu

Typy urządzeń:

- pomiarowe
  - czujniki wszelkiego rodzaju
- przetwarzające
  - regulatory temperatury
  - PLC
  - HVAC
- wykonawcze
  - aktuatory wszelkiego rodzaju
- protokoły komunikacji
  - KNX
  - Modbus
  - OPC UA
  - Ethernet TCP/IP
  - DALI
  - BACnet
  - Zigbee
- panel sterowania
  - aplikacje mobilne
  - systemy komputerowe

| Protokol | Typ / warstwa | Medium | Zastosowanie w BMS | Zalety | Wady |
|---|---|---|---|---|---|
| KNX | Automatyka budynkowa (field level) | KNX TP, KNX IP, KNX RF | Oswietlenie, rolety, HVAC strefowe | Standard miedzynarodowy, interoperacyjnosc, stabilnosc | Niska przepustowosc, konfiguracja przez ETS |
| Modbus | Integracja urzadzen | RS-485, Ethernet | Liczniki energii, centrale HVAC, falowniki | Prostota, powszechnosc | Brak bezpieczenstwa, brak semantyki danych |
| OPC UA | Warstwa nadrzedna / integracyjna | Ethernet TCP/IP | Integracja BMS z SCADA, IT | Bezpieczenstwo, model danych, skalowalnosc | Zlozonosc, wieksze wymagania sprzetowe |
| Ethernet TCP/IP | Infrastruktura komunikacyjna | Skretka, swiatlowod | Transport danych BMS | Wysoka przepustowosc, standard IT | Brak deterministycznosci |
| DALI | Sterowanie oswietleniem | Magistrala 2-przewodowa | Oprawy oswietleniowe, sciemnianie | Precyzyjne sterowanie, adresowanie opraw | Tylko oswietlenie, mala skala |
| BACnet | Automatyka budynkowa / nadrzedna | RS-485, Ethernet | HVAC, BMS, SCADA | Otwarty standard, interoperacyjnosc | Rozne implementacje producentow |
| Zigbee | Bezprzewodowy (field level) | RF 2.4 GHz | Czujniki, oswietlenie | Niski pobor mocy, siec mesh | Zaklocenia, mniejsza niezawodnosc |

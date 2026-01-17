# 1. Architektura systemów IoT i ich elementy składowe

IoT nie ma twardo określonej architektury, przedstawimy sobie kluczowy model cztero-warstwowy

1. **Urządzeń** – czujniki, aktuatory

2. **Komunikacji** – protokoły i transmisja (MQTT, CoAP, HTTP, LoRa, BLE, Zigbee, WiFi)

3. **Przetwarzania** – bazy danych, chmura, analiza

4. **Aplikacji** – zarządzanie urządzeniami, bezpieczeństwo, API, wizualizacja

## Warstwa Urządzeń

wszelkie czujniki i aktuatory, do tej warstwy dodać możemy edge computing który czasami zaliczany jest jako osobna warstwa

**Edge computing** - obliczenia wstępne lub działania nie koniecznie wykonywane informując o tym chmurę, dane przed wysyłką mogę potrzebować ówczesnego przetworzenia lub skompresowania.
Urządzenia końcowe (czyli elementy warstwy percepcji jak np. komputer raspberry) mogą przygotowywać dane w celu zmniejszenia natłoku w sieci itp. Urządzenia końcowe dodatkowo mogą same wykonywać 
zadania, przykładowo by system bezpieczeństwa wezwał ochronę nie potrzebuje tego robić przez chmurę, być może sam ma kartę sim i dokona telefonu.

## Warstwa Komunikacji

do tej warstwy zaliczamy protokoły i sposoby transmisji danych oraz gate'y, w tej warstwie również może nastąpić edge computing (procesy w gate'cie)

*Gate* - urządzenie pośredniczące między urządzeniami IoT a siecią wyższego poziomu (Internet, chmura, serwery)
zbiera dane z wielu urządzeń IoT. Co robi gate(brama):

- tłumaczy protokoły (np. Zigbee → IP/MQTT)

- agreguje i filtruje dane (nie wysyła wszystkiego do chmury)

- zapewnia bezpieczeństwo (autoryzacja, szyfrowanie)

- umożliwia sterowanie urządzeniami w druga stronę

## Warstwa przetwarzania

warstwa ta odpowiada za przechowywanie i przetwarzanie dużych ilości danych

**Przykładowe platformy IoT:** AWS IoT(Amazon), Azure IoT, Google Cloud IoT
**Przetwarzanie:** Apache Spark, AWS Lambda
**Magazyn danych:** AWS DynamoDB, MongoDB, MySQL

## Aplikacyjne

warstwa pozwalająca na interakcję użytkownika z urządzeniami (np. webapp, aplikacje mobilne, SMI, SCADA), warstwa realizuje także logikę systemu (za duża temperatura to włącz klimę)

# 1. Komunikacja

Komunikacja w IoT realizowana jest przez:

Protokoły takie jak:
| Cecha           | MQTT                       | HTTPS                  | WebSocket                        |
| --------------- | -------------------------- | ---------------------- | -------------------------------- |
| Model           | publish/subscribe          | request/response       | full-duplex (push/pull)          |
| Narzut          | bardzo niski               | wysoki                 | średni                           |
| Zużycie energii | niskie                     | wysokie                | średnie/wysokie                  |
| Skalowalność    | bardzo dobra               | średnia                | średnia                          |
| Opóźnienia      | niskie                     | średnie/wysokie        | bardzo niskie (po połączeniu)    |



Warstwę fizyczną:

| Cecha           | LoRaWAN                                          | Zigbee                             | BLE (Bluetooth Low Energy)                   | WiFi                                                     | Ethernet                                     |
| --------------- | ------------------------------------------------ | ---------------------------------- | -------------------------------------------- | -------------------------------------------------------- | -------------------------------------------- |
| Narzut          | bardzo niski (krótkie ramki)                     | niski/średni                       | niski                                        | średni/wysoki                                            | niski                                        |
| Zużycie energii | bardzo niskie (urządzenia bateryjne, lata pracy) | niskie                             | bardzo niskie (sensor)                       | średnie/wysokie                                          | wysokie (zasilanie przewodowe)               |
| Skalowalność    | bardzo wysoka (setki → tysiące urządzeń)         | średnia / wysoka (mesh)            | średnia (kilkadziesiąt urządzeń w gwieździe) | średnia (do kilkudziesięciu urządzeń)                    | wysoka, zależna od switchy                   |
| Opóźnienia      | wysokie (kilka sekund)                           | średnie (ms → setki ms)            | niskie (ms)                                  | bardzo niskie (ms)                                       | bardzo niskie (ms)                           |
| Zasięg          | bardzo długi (kilometry)                         | krótki/średni (10–100 m)           | krótki (10–50 m)                             | średni (50–100 m)                                        | przewodowy, zależny od kabla                 |

# 2. Akwizycja

**Akwizycja** to proces zbierania, rejestrowania i przesyłąnia danych

# 3. Przetwarzanie danych

Prócz przetwarzania danych w celu efektywnego przetransportowania ich. Niektóre dane mogą służyć do modelowania obiektów w celu wyznaczania trendów, planowania dalszych działań i optymalizacji sterowania

Dane przetwarzena mogą być na dwóch poziomach:

**Edge** (computing): przetwarzanie na urządzeniach konćowych (blisko czujnika), przetwarzanie na gate'cie. Tutaj przetworzone dane pozwalają na sprawniejsze przesyłanie ich dalej, szybszą reakcję i oszczędzanie mocy chmury.

*Przykład: W systemach alarmowych szybciej jest by urządzenie końcowe wykryło i powiadomiło służby zamiast robić to przez chmurę, urządzenie końcowe może także dokonywać kompresji np. obrazów by możliwe zminimalizować obciążenie sieci.*

**Cloud** (computing): Wykorzystujemy do przetwarzania dużej ilości danych. Na chmurze także generujemy raporty, analizy, modele itp.

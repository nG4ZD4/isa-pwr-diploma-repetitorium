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

może i trzeba rozpisać całą trogę jaką dane przebywają przez IoT od czujnika do wizualizacji?

# 3. Przetwarzanie danych

Prócz przetwarzania danych w celu efektywnego przetransportowania ich. Niektóre dane mogą służyć do modelowania obiektów w celu wyznaczania trendów, planowania dalszych działań i optymalizacji sterowania

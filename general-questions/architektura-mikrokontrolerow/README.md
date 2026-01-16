# Architektura mikrokontrolerów
<img width="1014" height="749" alt="image" src="https://github.com/user-attachments/assets/8881e4f8-c639-48b9-a354-a44b8e03030a" />

## 1. Definicja:
* **Mikrokontroler:** układ scalony zawierający mikroprocesor oraz wszystkie niezbędne układy peryferyjne, zdolny do autonomicznej pracy. 

## 2. Architektura pod względem budowy:
* **CPU:** mikroprocesor
* **Pamięć programu:** pamięć przechowująca kod programu, często flash, EPROM lub EEPROM.
* **Pamięć RAM:** pamięć operacyjna, tymczasowa, przechowuje zmienne i dane podczas pracy mikrokontrolera
* **Układy wejścia/wyjścia** służy do komunikcji między urządzeniami w systemach mikroprocesorowych
* **Pozostałe układy peryferyjne** takie jak przetworniki DAC i ADC, liczniki, timery itp.

## 3. Architektura pod względem pamięci
* **Architektura von Neumana:** jedna, wspólna szyna danych dla danych i programu. Prosty proces pisania programów, ale wolne wykonywanie. Przykład: RP2040 (ARM Cortex-M0+)
* **Architektura harwardzka:** oddzielna pamięć dla danych i rozkazów. Szybka, ale złożona, wymaga dwóch magistral. Przykład: Atmega328P.
* **Architektura mieszana (zmodyfikowana harwardzka):** oddzielna pamięć dla danych i rozkazów w procesorze (cache l1), które bierą dane z łączonej pamięci (RAM). Większość współczesnych komputerów tak działa. Przykład: Rodzina STM32.

## 4*. Architektura pod względem zestawu instrukcji
* **CISC (complex instruction set computing) :** złożone, specjalistyczne rozkazy. Jedna instrukcja może być wykonywana przez kilka cykli zegara procesora.
* **RISC (reduced instruction set computing) :** liczba rozkazów zredukowana do minimum. Jedna instrukcja na cykl.

## 5. Podsumowanie
Ciężko powiedzieć pod jakim względem rozumieć to pytanie. Pierwsze dwa punkty najbardziej sensowne, * jako coś co istnieje, ale na wykładach (chyba) nie było.

# 1. Układ regulacji
**Układ regulacji** to zbiór elementów mających na celu ustanowić wyjście układu na pożądanej przez nas wartości.

**Przykład:**

*Chcemy by w pomieszczeniu było 29°C, ustawiamy na termostacie a układ regulacji (jakiś) tak grzeje by tą temperaturę w pomieszczeniu utrzymać automatycznie*

## 1.2 Podstawowe algorytmy
- regulator dwustawny
- regulator trójstawny
- regulator PID
  - anty-windup
  - ograniczenia górne i dolne
- regulacja pogodowa

### Regulator dwustawny

*poniżej przykłąd regulacji dwustawnej - PV to np. temperatura, czerwony sygnał to załączenie pieca, SP to temperatura jaką chcemy osiągnąć, a zielony to wyłącznik całego sterowania który jest tutaj ekstra, ale nie znalazłem lepszego wykresu*

<img width="1200" height="600" alt="skok_zoom" src="reg-dwustawny.png" />

**Histereza** na powyższym obrazku zaznaczona Hys jest to przedział wartości sterowanej w którym temperatura jest akceptowalna przez nasz układ regulacji

*można jeszcze się spotkać z takim rysunkiem który przedstawia charakterystykę regulatora dwustanego z histerezą*

<img width="200" height="200" alt="skok_zoom" src="reg dwustawny charakt.png" />

### Regulator trójstawny

Można by powiedzieć że to samo co dwustawny tylko poniżej pewnego zakresu grzejemy, a powyżej pewnego chłodzimy wtedy histerezy są wtedy dwie

<img width="200" height="200" alt="skok_zoom" src="reg trojstawny.png" />

### Regulator PID

Regulator **PID** jest najpopularniejszym regulatorem składającym się z członów:

- P - proporcjonalnego - reaguje na bieżący błąd
- I - całkującego - eliminuje skumulowane błędy z przeszłości
- D - różniczkującego - przewiduje przyszłe błędy

*Tutaj jeżeli ktoś nmie pamięta/nie czuje odsyłam do [wszechboga elektroniki](https://www.youtube.com/watch?v=ecOGDeYjt0M) itp.: *

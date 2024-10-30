## Opis projektu

### Cel:

Projekt "Calendar" ma na celu dostarczenie użytkownikom prostego, minimalistycznego kalendarza internetowego, dostępnego bezpośrednio w przeglądarce. Widget pozwala na przeglądanie miesięcy, zarządzanie wydarzeniami oraz zmianę motywu interfejsu na biały lub czarny. Dzięki intuicyjnemu układowi, aplikacja ułatwia organizację dnia i przypomina o ważnych terminach.

### Opis funkcji:

- **Wyświetlanie kalendarza:** Użytkownik może przeglądać dni, tygodnie oraz miesiące i uzyskać podgląd wydarzeń.
- **Dodawanie wydarzeń:** Funkcja umożliwia dodawanie, edytowanie i usuwanie wydarzeń na określone dni.
- **Zmiana motywu:** Możliwość przełączania między motywem czarnym i białym, aby dopasować wygląd widgetu do preferencji użytkownika.
- **Przypomnienia:** Opcja ustawiania przypomnień dla nadchodzących wydarzeń.

## Analiza wymagań:

### Wymagania funkcjonalne:

- **Wyświetlanie kalendarza:** Użytkownik ma możliwość przeglądania miesięcznego widoku kalendarza, z podglądem na dni tygodnia oraz dni wolne.
- **Dodawanie i edycja wydarzeń:** Użytkownik może dodawać wydarzenia z możliwością edycji lub usunięcia.
- **Motyw kolorystyczny:** Możliwość zmiany motywu kalendarza pomiędzy czarnym a białym, co zapewnia wygodę użytkowania w różnych warunkach oświetleniowych.
- **Przypomnienia:** Opcja dodawania przypomnień, które mogą wyskakiwać na ekranie lub w formie powiadomień przeglądarkowych.

### Wymagania niefunkcjonalne:

- **Minimalistyczny interfejs:** Czysty i estetyczny wygląd kalendarza, który pozostaje spójny zarówno w wersji białej, jak i czarnej.
- **Responsywność:** Dostosowanie do różnych rozdzielczości ekranów, aby kalendarz wyświetlał się poprawnie na urządzeniach mobilnych oraz komputerach stacjonarnych.
- **Wydajność:** Szybkie ładowanie i płynne działanie widgetu.

## Projekt interfejsu:

### Szkice/wizualizacje interfejsu:

- _Strona główna:_ Widok miesięczny kalendarza z opcjami dodawania wydarzeń, zmiany motywu i przeglądania przypomnień.
- _Widok wydarzenia:_ Okno modalne umożliwiające dodawanie nowych wydarzeń lub edytowanie już istniejących.

### Mapa strony:

- _Strona główna_
  - Widok kalendarza
  - Przełącznik motywu (czarny/biały)
- _Widok wydarzenia_
  - Formularz dodawania wydarzenia
  - Opcja przypomnienia

## Architektura systemu:

### Opis struktury danych:

Widget przechowuje dane dotyczące wydarzeń, ustawień użytkownika oraz motywu w lokalnej pamięci przeglądarki, z możliwością integracji z kontami użytkowników w przyszłości.

- **Parametry wydarzeń:** Data, godzina, opis wydarzenia, oraz ustawienia przypomnienia.
- **Motyw:** Informacje o aktualnie wybranym motywie (czarny lub biały), które są zapisywane w pamięci przeglądarki.

### Diagramy architektury:

Widget oparty jest na architekturze MVC (Model-View-Controller):

- **Model:** Przechowuje informacje o wydarzeniach i ustawieniach motywu.
- **Widok (View):** Wyświetla kalendarz i okna dodawania wydarzeń oraz ustawień motywu.
- **Kontroler (Controller):** Zarządza interakcjami użytkownika, w tym zmianą motywu i dodawaniem/edycją wydarzeń.

## Implementacja:

### Opis technologii:

- **Frontend:** HTML, CSS, JavaScript (React.js) dla responsywnego i intuicyjnego interfejsu użytkownika.
- **Lokalne przechowywanie danych:** Web Storage API (Local Storage) do zapisu danych o wydarzeniach i motywie.

### Struktura kodu:

- _Katalogi/pliki:_ Oddzielne komponenty dla widoku kalendarza, ustawień motywu oraz formularza wydarzenia.
- _Style pisania kodu:_ Stosowanie dobrych praktyk, takich jak modularność, komentarze i przestrzeganie konwencji stylu kodu.

## Testowanie:

### Plan testów:

- **Testy jednostkowe:** Sprawdzanie funkcji dodawania, edycji i usuwania wydarzeń.
- **Testy interfejsu użytkownika:** Sprawdzanie poprawności wyświetlania kalendarza i funkcji zmiany motywu.
- **Testy kompatybilności:** Upewnienie się, że widget działa poprawnie w różnych przeglądarkach.
- **Testy wydajnościowe:** Ocena szybkości ładowania oraz responsywności widgetu.

### Procedury testowania:

- Przygotowanie zestawu przypadków testowych dla każdej funkcji.
- Dokumentacja błędów i usprawnień.

## Wdrożenie i konserwacja:

### Plan wdrożenia:

- **Etapy wdrażania:** Testowanie i publikacja w formie widgetu dostępnego w przeglądarce.
- **Terminy:** Harmonogram obejmuje testy i publikację widgetu na docelowej platformie.

### Procedury konserwacji:

- **Wsparcie techniczne:** Możliwość zgłaszania problemów technicznych przez użytkowników.
- **Aktualizacje:** Regularne aktualizacje na podstawie opinii użytkowników oraz bieżących trendów UX.

## Harmonogram:

### Plan projektu:

- **Etapy realizacji:** Obejmuje przygotowanie kalendarza, interfejsu i motywów, a także testowanie i wdrożenie.
- **Terminy:** Oceniany czas na realizację każdego z etapów w celu optymalizacji harmonogramu.

## Kosztorys:

### Szacunkowe koszty:

- **Rozwój aplikacji:** Wg godzin pracy lub stawek zespołu.
- **Koszty utrzymania:** Hosting oraz konserwacja widgetu, wsparcie techniczne.

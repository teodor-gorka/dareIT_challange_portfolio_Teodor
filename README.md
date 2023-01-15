# Task 1
## Subtask 1
Uzyskałem 10 punktów z testu. 
## Subtask 3
<p align="justify">Cześć, jestem Teodor. Zdecydowałem się na udział w projekcie, aby oswoić się z praktyczną stroną testowania. Zdecydowanie łatwiej przyswajać mi informacje poprzez praktyczne wykonywanie zadań, a następnie usystematyzowanie wiedzy przez naukę definicji. Mam nadzieję, że po naszej współpracy będę gotowy na rozpoczęcie stażu jako tester manualny, a zdobyte z Wami doświadczenie, prawidłowo ukierunkuje mnie do dalszego rozwoju i nauki.</p>

***Teo***
## Subtask 4
### Przeznaczenie aplikacji [ScoutsPanel](https://scouts-test.futbolkolektyw.pl/)
<p align="justify">Aplikacja służy do katalogowania informacji o zawodnikach piłki nożnej oraz zbierania ich statystyk z rozegranych spotkań. Pozwala również na przeszukiwanie skatalogowanych danych.</p> 

### Funkcjonalności aplikacji


* Wyświetlanie strony w języku polskim lub angielskim
* Logowanie użytkowników 

*<p align="justify">Wszystkie niżej wymienione funkcjonalności, wymagają zalogowania do konta użytkownika poprawnymi danymi, przypisanymi przez administratora aplikacji.*</p> 
* Zarządzanie wpisami w katalogu zawodników
  * dodawanie nowego profilu zawodnika do katalogu
  * edytowanie już istniejącego profilu zawodnika
  * usuwanie już istniejącego profilu zawodnika
  * przeszukiwanie katalogu przy pomocy filtrów:
    * imię
    * nazwisko
    * przedział wiekowy (min-max)
    * pozycja
    * klub 
    * ocena zawodnika
  * pobranie całego katalogu do pliku csv
  * wydrukowanie całego katalogu
  * wyświetlanie jedynie wybranych kolumn katalogu
    * imię
    * nazwisko
    * wiek
    * pozycja
    * klub
    * średnia ocena zawodnika
    * ilość rozegranych meczów
    * ilość utworzonych raportów

* Dodawanie rozegranych meczów do profilu zawodnika
* Tworzenie dla profilu zawodnika raportów meczowych "na żywo" 
    * dodawanie informacji o zdarzeniach boiskowych dotyczących zawodnika, wraz ze wskazaniem miejsca zdarzenia na boisku
    * licznik rozegranych połów meczu
    * licznik czasu meczu / czasu zawodnika na boisku (nie doprecyzowano)
    * możliwość cofnięcia ostatniego dodanego zdarzenia
    * możliwość wykasowania wszystkich wprowadzonych informacji
* Tworzenie dla profilu zawodnika raportów meczowych "po meczu"
    * dodanie oceny opisowej w trzech kategoriach
      * Inteligencja boiskowa
      * Mentalność
      * Podsumowanie
    * Wybranie końcowej oceny występu zawodnika, w skali 1-5 
    * pobranie informacji z raportu tworzonego "na żywo", oraz ich prezentacja na wykresach wraz ze statystykami
      * możliwość dodania komentarzy przy poszczególnych statystykach
      * możliwość dodania własnych notatek na temat zagrań/zdarzeń niekonwencjonalnych, nieujętych w statystykach.
      
##### Ocena intuicyjności oraz wyglądu interfejsu aplikacji
* Strona główna
  * Na stronie głównej zabrakło mi wyszukiwarki zawodników, dostęp do niej powinien być szybszy. 
  * Na ekranach o dużej rozdzielczości, "kafelki" przestają być wyrównane. Część jest zbyt rościągnięta, pomiędzy innymi przerwy są zbyt szerokie, cała strona przestaje być czytelna i użyteczna. Sugerowałbym wrzucenie "Kafelek" do kontenera, który będzie miał określoną maksymalną szerokość, tak aby przy szerszych ekranach, cała zawartość strony pozostawała wyrównana na środku ekranu. <img width="1422" alt="zrzut ekranu, rozrzucone kafelki" src="https://user-images.githubusercontent.com/75786629/212549708-c962cdb2-26b5-4e2e-8ab7-be90b5301abf.png">

  * Część przycisków ma wygląd podkreślonego linku, natomiast przycisk "Dev team contact", jest bez podkreślenia - brak spójności. <img width="1132" alt="zrzut ekranu przyciski" src="https://user-images.githubusercontent.com/75786629/212549739-c7787663-f8ec-4408-ba00-b4cd46dafc90.png">

  * Wygląd przycisków jest archaiczny.

* Katalog zawodników
  *  Przeglądanie katalogu jest niewygodne, ze względu na zbyt mało wyraźne oddzielenie kolejnych profili zawodników pomiędzy sobą. Problem jest jeszcze większy na urządzeniach mobilnych. <img width="499" alt="zrzut ekranu tabela na mobilnych" src="https://user-images.githubusercontent.com/75786629/212549834-c610da8b-57d7-4851-8b58-985b4839bb67.png">

  * Logo ScoutPanel jest niekatywne. Oczekiwałem przycisku, który przeniesie użytkownika na stronę główną, lub do katalogu zawodników. <img width="624" alt="logo przycisk" src="https://user-images.githubusercontent.com/75786629/212549926-592f285e-d1ca-463f-82fe-204247297cee.png">

  * Kliknięcie w profil zawodnika, przenosi nas od razu do edycji jego danych. Uważam, że po kliknięciu powinniśmy otwierać profil zawodnika z informacjami i 3 opcjami w lewym menu: edycja profilu, mecze, raporty. 
  * 

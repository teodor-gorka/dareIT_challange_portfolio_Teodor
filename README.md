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
  *  Przeglądanie katalogu jest niewygodne, ze względu na zbyt mało wyraźne oddzielenie kolejnych profili zawodników pomiędzy sobą. Problem jest jeszcze większy na urządzeniach mobilnych. <img width="499" alt="tabela na mobilnych" src="https://user-images.githubusercontent.com/75786629/212549834-c610da8b-57d7-4851-8b58-985b4839bb67.png">

  * Logo ScoutPanel jest niekatywne. Oczekiwałem przycisku, który przeniesie użytkownika na stronę główną, lub do katalogu zawodników. 
  <img width="624" alt="logo przycisk" src="https://user-images.githubusercontent.com/75786629/212549926-592f285e-d1ca-463f-82fe-204247297cee.png">

  * Kliknięcie w profil zawodnika, przenosi nas od razu do edycji jego danych. Uważam, że po kliknięciu powinniśmy otwierać profil zawodnika z informacjami i 3 opcjami w lewym menu: edycja profilu, mecze, raporty. 

* Raport po meczu
  * gwiazdki na początku formularza nie aktywne, a odruchowo to własnie tam chciałem wstawić ocenę. 
* zakładka "Mecze" oraz zakładka "Raporty
  * Tabela nie mieści sie w całości na urządzeniach mobilnych
  * Brak możliwości sortowania wg poszczególnych kolumn tabeli.

W mojej ocenie, szata graficzna nie jest zbyt atrakcyjna, natomiast nie przeszkadza to w funkcjonalności aplikacji. Sugerowałbym konsultację z klientem, czy oczekuje "surowej" funkcjonalności, czy chciałby wprowadzić bardziej atrakcyjny design aplikacji. 

### Błędy


#### 1. Logowanie
* formularz nie przepuszcza białych znaków. Bardzo łatwo o nieprawidłowe logowanie, jeśli np wkleimy poprawny adres email, ale nieświadomie - ze spacją na końcu. 

#### 2. Strona główna 
* Błąd językowy, zgodnie z zasadami języka polskiego "Ilość meczów" 
<img width="296" alt="błąd językowy - meczów" src="https://user-images.githubusercontent.com/75786629/212661347-e1289a0a-6415-4774-bbbc-397d3fe29494.png">

* Jeśli mamy niezapisany mecz i klikniemy w odnośnik "Wróć do raportu", nic sie nie dzieje + otrzymujemy błąd w konsoli. Działa natomiast clickPPM + "otwórz w nowej karcie"
<img width="930" alt="powrot do niezapisanego meczu oraz blad w konsoli" src="https://user-images.githubusercontent.com/75786629/212663692-7226f752-ab3e-4d80-a5ce-3ad0c0b2cfe0.png">

#### 3. Katalog zawodników (zakładka "Gracze")

* Brak możliwości sortowania tabeli wg kategorii "Mecze" oraz "Raporty"
* Brak zwijania zbyt długiej zawartości komórki tabeli, powoduje brak czytelności całej tabeli
<img width="1327" alt="zbyt dlugie dane" src="https://user-images.githubusercontent.com/75786629/212667503-0e5b0889-627c-4748-9fb0-1f2f96e6aed6.png">

* Brak opcji "Dodaj gracza" - sugeruję umieścić na górze strony. 


#### 4. Dodawanie/Edycja danych zawodnika
* Formularz akceptuje zbyt wiele znaków w poszczególnych polach, powodując późniejsze problemy z wyświetlaniem.
* Formularz akceptuje ujmeny wzrost, oraz zbyt wysokie wartości
* Formularz akceptuje ujemą wagę, oraz zbyt wysokie wartości
* Brak informacji o jednostkach masy pola "waga". należy uzupełnić np: (kg)
<img width="550" alt="brak jednostek masy" src="https://user-images.githubusercontent.com/75786629/212672910-714ad3df-4a12-4777-9530-f2c24a855c87.png">

* Formularz akceptuje przyszłą datę urodzenia, oraz zbyt odległe daty urodzenia z przeszłości
* Pole "telefon" akceptuje stringsy zamiast wyłącznie wartości liczbowe i ewentualne znaki specjalne
* Formularz akceptuje niepoprawne linki (np ze spacjami)
* Pola "Łączy nas piła", "90 minut", "profil facebook" akceptują linki do innych stron internetowych, oraz niepoprawny format adresów. 
<img width="1137" alt="bledne linki" src="https://user-images.githubusercontent.com/75786629/212674321-9ab381ba-2a67-4369-b67a-3871c62919ab.png">

* Przy wprowadzeniu adresu email w niepoprawnej formie, formularz nie pozwoli nam zapisać gracza, bez informacji zwrotnej dlaczego. Należy wstawić prompt "niepoprawny adres email" pod polem "adres email"
<img width="1175" alt="niepoprawny mail gracza" src="https://user-images.githubusercontent.com/75786629/212671382-7e5fad44-8eb3-45f1-8e7f-b83b1ce3fae6.png">

* Formularz akceptuje puste pola "Języki" po kliknięciu "dodaj język"
 <img width="1173" alt="puste pola jezyki" src="https://user-images.githubusercontent.com/75786629/212675083-9849d79d-83b0-4cbd-9a40-95ded54d06d1.png">

* Formularz akceptuje puste pola "link do youtube", oraz niepoprawne linki
<img width="291" alt="Puste linki youtube" src="https://user-images.githubusercontent.com/75786629/212882441-56c440e5-1e39-46bf-8e60-82ec308dc781.png">

* W trybie edycji, przycisk "Clear" kasuje tylko dane wprowadzone w tej "sesji" zamiast wyczyścić wszystkie pola. Sugeruję dodanie/zmianę nazwy przycisku na "cofnij zmiany" 
* Błędy językowe: 
  * nazwy województw w języku polskim, piszemy małą literą.
  * rozwijana lista województwo: "Dolnoślaskie" (brak ą) -> poprawić na "dolnośląskie"
  * w języku angielskim rozwijana lista "district": Łódź -> poprawić na "lodzkie"


* Wątpliwości i sugestie:
  * Brak kategorii płeć - katalog mógłby być bardziej precyzyjny i łatwiejszy w filtrowaniu, jeśli użytkownik mógłby rozróżnić zawodników i zawodniczki. 
  * Wprowadzenie rozwijanych list zamiast pól tekstowych: 
    * "Główna Pozycja", 
    * "Pozycja alternatywna" 
    * "Języki"  
  Przy zmianie języka wyświetlania strony, te kategorie byłyby tłumaczone i odpowiednio filtrowane w wyszukiwarce. Przy aktualnym stanie aplikacji, użytkownik szukając "Bramkarz" nie znajdzie wszystkich zawodników o pozycji "Goalkeeper" itp.  
  * Przy scrollowaniu formularza, możemy przez przypadek zmienić wzrost lub wagę zawodnika, jeśli były wybrane i wskaźnik myszy jest nad tym polem. 


#### 5. Zakładka "Mecze"
* Brak odpowiedniej responsywności, tabela wymaga przewijania w prawo/lewo na urządzeniach mobilnych. Jest zbyt rozciągnięta na ekranach o wysokiej rozdzielczości. 
* Brak możliwości sortowania tabeli wg poszczególnych kolumn
* Wyświetlanie całości zawartości komórki, powoduje nieczytelne wyświetlanie tabeli. Należy wyświetlić jedynie początkowy fragment dłuższego tekstu, tak by zachować funkcjonalność i wygodę użytkowania aplikacji.
<img width="1254" alt="zbyt długi tekst w komórce" src="https://user-images.githubusercontent.com/75786629/212680036-3560b496-09fc-4c6c-986f-9cbee2292a4b.png">
* Nie ma możliwości usunięcia dodanego meczu 
* Możemy wielokrotnie dodawać raport z tego samego meczu, powodując duplikaty w zakładce "Raporty"

#### 6. Formularz dodawania meczu do profilu zawodnika
* Formularz akceptuje datę meczu wcześniejszą niż data urodzenia zawodnika
* Daty z odległej przeszłości, daty przyszłe, są akceptowane. 
* Numer zawodnika powinien mieścić się w zakresie 1 - 99, formularz akceptuje wartości poniżej zera oraz zbyt wysokie wartości. 
* Formularz akceptuje "czas gry" dłuższy, niż możliwa jest długośc meczu wg zasad piłkarskich. Sugeruję 180 minut jako maksymalną wartość dla tego pola
* "Czas gry" akceptuje wartości ujemne
* Ilośc zdobytych oraz straconych goli powinna mieścić się w zakresie 0-99
* W trybie edycji, przycisk "Clear" kasuje tylko dane wprowadzone w tej "sesji" zamiast wyczyścić wszystkie pola. Sugeruję dodanie/zmianę nazwy przycisku na "cofnij zmiany" 
* W polskiej wersji językowej nie przetłumaczono z angielskiego nazw pól "Web match" oraz "general"

#### 7. Tworzenie raportu "na żywo" (opcja "rozegraj mecz" w zakładce "mecze")
* przycisk <img width="35" alt="ikona zegara" src="https://user-images.githubusercontent.com/75786629/212684164-f1dbfc40-b90f-409a-8c7f-b37e14acf063.png"> pozwala na więcej niż 4 połowy meczu. 

* numer połowy może być ujemny
* "czas" - sugeruję doprecyzowanie czy to czas meczu, czy czas gry zawodnika
* "czas" akceptuje wartości ujemne 
<img width="202" alt="ujemny czas i numer połowy" src="https://user-images.githubusercontent.com/75786629/212684858-412f6289-83c2-4682-9a2d-551cc3141667.png">
* Brak informacji o roli przycisków, sugeruję dodać prompty przy najechaniu wskaźnikiem, lub podpisy pod ikonami. 
* Brak logiki: wg zakładki "Mecze", zawodnik rozegrał w tym meczu 0 minut, ale w raporcie może w 5 minucie strzelić bramkę, w 10min podać itp. 
* Brak możliwości edytowania wykasowania dodanego wydarzenia/zagrania.
* Po poprawnym "wysłaniu raportu" - raport nie pojawia się w zakładce raporty, czy to oczekiwany rezultat?

#### 8. Zakładka "Raporty"
* Brak odpowiedniej responsywności, tabela wymaga przewijania w prawo/lewo na urządzeniach mobilnych. Jest zbyt rozciągnięta na ekranach o wysokiej rozdzielczości. 
* Brak możliwości sortowania tabeli wg poszczególnych kolumn
* Wyświetlanie całości zawartości komórki, powoduje nieczytelne wyświetlanie tabeli. Należy wyświetlić jedynie początkowy fragment dłuższego tekstu, tak by zachować funkcjonalność i wygodę użytkowania aplikacji.
* Nie ma możliwości usunięcia dodanego raportu 

#### 9. Formularz dodawanie raportu do profilu zawodnika
* Brak responsywności na urządzenia mobilnych
* W polach tekstowych, niektóre funkcjonalności edytora tekstu, nie działają zgodnie z oczekiwaniem:
  * Lista numerowana po kliknięciu klawisza enter, nie tworzy kolejnego podpunktu listy z cyfrą. 
  * Lista punktowana po kliknięciu klawisza enter, nie tworzy kolejnego podpunktu listy z punktorem.
  * Przedzielenie tekstu w liście numerowanej/punktowanej klawiszem enter, tworzy podwójny odstęp między liniami (podwójny enter)
<img width="174" alt="niepoprawne listy" src="https://user-images.githubusercontent.com/75786629/212690981-eed6793e-c455-4bea-8584-def829aa9083.png">

* Blockquote nie dodaje tła tekstu. (powinien?)
* Pole IV. Recenzja, niepoprawne i niezrozumiałe tłumaczenie tekstu.
  <img width="806" alt="niepoprawne tlumaczenie review" src="https://user-images.githubusercontent.com/75786629/212692137-1467f2ef-1ef6-45c8-8e0e-56f9b06a485c.png">

* Brak limitu liczby znaków w polach tekstowych formularza, może wprowadzać utrudnioną czytelność i funkcjonalność raportów. 

#### 10. Dodatkowe uwagi i wątpliwości
* czy w aplikacji oczekiwane jest rozróżnienie płci? 
* czy słowo "gracz" jest właściwym określeniem? Sugeruję "Zawodnik" lub "Piłkarz". "Gracz" kojarzy się raczej z rekreacyjnym a nie zawodowym zajmowaniem się dyscypliną. 


# Task 2

### Subtask 1
[Test cases for user stories](https://docs.google.com/spreadsheets/d/1pv7msMy5xce1eiu3cJlrYPfXBqqHVeoBAAWHH1DlHi8/edit?usp=share_link)

### Subtask 2

[Test cases based on own experience](https://docs.google.com/spreadsheets/d/13ROkTFxQMq_r0yxWq9p_w_1NaGysFLD_z55bLUTCoqo/edit?usp=share_link)

### Subtask 3
##### Po co piszemy test case'y?
Test case'y tworzą ważną dokumentację pracy testera oraz mogą być pomocne w zrozumieniu działania aplikacji. Test case systematyzuje logikę i kolejność testowania, zwiększając pewność przetestowania kluczowych przypadków użycia aplikacji. Przypadek testowy, daje jasne kryteria, na podstawie których tester może ocenić, czy funkcjonalność działa zgodnie z oczekiwaniami. Ukazuje, które elementy zostały przetestowane oraz dokładnie w jakich krokach. Pozwala na odtwarzanie tych kroków w przyszłości w identyczny sposób.  Testowanie oparte o dobrze napisane przypadki testowe, w oparciu jedynie o dokumentację, mogą wpłynąć na dokładniejsze przetestowanie aplikacji, niż w przypadku testów eksploracyjych. Dobrze przygotowane test case'y stanowią również istotny element przy wdrażaniu nowych osób do projketu.


### Subtask 4
[5 test cases for pick.eat.up app](https://docs.google.com/spreadsheets/d/1A1ClmNCzGkpAbMm4YY02DBopjd0cOJuWXbbWaWR-sok/edit?usp=sharing)

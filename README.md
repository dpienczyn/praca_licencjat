    
                                       AWARIA - SYSTEM REJESTRUJĄCY USTERKI I NAPRAWY
---------------------------------------------------------------------------------------------------------------------

## Keywords
aplikacja internetowa, ruby on rails, system rejestrowania, naprawa, bootstrap, interfejs graficzny użytkownika

## Autor
Dominika Pienczyn, numer albumu 236389

## Streszczenie

   Praca przedstawia aplikacje internetową o nazwie "Awaria" która jest systemem rejestrującym usterki oraz naprawy sprzętu i została stworzona w grupie 3-osobowej. Jako cel postawiłam sobie, wykonanie frontendu aplikacji oraz stworzenie poszczególnych elementów takich jak: automatyzacja powiadomień, filtracja danych, uaktywnienie resetowania hasła oraz e-maili powitalnych podczas rejestracji. Do stworzenia aplikacji wykorzystano system Linux, baze danych Postgresql, framework Ruby on Rails oraz Bootstrap a następnie wdrożono ją na serwer Heroku. Wgląd do szerszej dokumentacji możliwy jest pod adresem <https://github.com/dpienczyn/awaria1>, przechowywany w repozytorium Githuba razem z kodem aplikacji.
  
## 1.Wstęp

   Graficzny interfejs użytkownika to ogólne określenie sposobu prezentacji informacji przez komputer oraz interakcji z użytkownikiem, polegające na rysowaniu i obsługiwaniu widżetów. Głównym aspektem tworzonego interfejsu jest optymalne rozmieszczenie elementów na stronie zgodnie z ergonomią pracy oraz szata graficzna która pełni ważną rolę dopełniającą i pomaga prowadzić użytkowników przez strukturę informacji prezentowaną w serwisie. Kolejnym istotnym elementem jest to aby aplikacja była responsywna. W dzisiejszym świecie korzystamy z różnego typu urządzeń nośnych tzn tabletów, smartfonów itp. dlatego tak ważne jest to aby aplikacja umiała dopasować sie do każdej rozdzielczości i każdego nośnika automatycznie. Od prawidłowo zaprojektowanego interfejsu zależy sukces strony, wygoda, intuicyjność oraz odpowiednia funkcjonalność. 
   W mojej pracy zamierzam przedstawić to w jak prosty i skuteczny sposób można zmienić szatę graficzną aplikacji oraz kilka innych elementów które umożliwiły zwiększenie funkcjonowania danego systemu.
   
## 2.  Wykorzystane technologie

### 2.1  Ruby on Rails
W utworzonym projekcie wykorzystano język Ruby wersje 2.3 oraz Framework Rails wersja 5.0.0. Ruby on rails jest frameworkiem open source i wykorzystuje się go do tworzenia aplikacji webowych. Napisany został z wykorzystaniem architektury MVC *(ang. Model-View-Controller)*.

Modele *(ang. Model)*  reprezentują dane aplikacji  i służą do manipulowania tymi danymi. W Railsach jest tak że jeden model odpowiada jednej tabeli w bazie danych.</br>

Widoki *(ang. View)* tworzą interfejs użytkownika aplikacji i służą do dostarczania danych do przeglądarki internetowej bądź innego urządzenia. Są to pliki zawierające kod w języku Ruby i HTML.</br>

Kontrolery *(ang. Controller)* w nich znajduje się cała logika aplikacji, mają za zadanie połączyć model i widok. Odpowiadają za przetwarzanie żądań przychodzących z przeglądarki internetowej, za pozyskiwanie danych z modeli oraz przekazanie ich do widoków w celu ich reprezentacji. </br>

### 2.2 Bootstrap

Bootstrap – Framework CSS, zawiera wiele narzędzi które przydają się podczas tworzenia interfejsu graficznego stron oraz aplikacji internetowych. Jest bardzo prosty w obsłudze, nie potrzeba wiele umiejętności żeby zacząć z nim pracować. Wystarczy podstawowa wiedza by rozpocząć tworzyć coś własnego. Bootstrap bazuje głównie na gotowych rozwiązaniach HTML i CSS. Może być używany do stylizacji m.in. przycisków, formularzy, wykresów nawigacji oraz innych komponentów wyświetlanych na stronie. Framework korzysta również z języka JavaScripts. By zacząć korzystać z platformy Bootstrap należy w pliku Gemfile dodać gem który odpowiedzialny jest za odpowiednie funkcjonowanie Frameworka.</br>

                                        gem ‘bootstrap-sass’, ‘~> 3.3.7’

Bootstrap jest platformą stylów CSS więc każdy kod powinien, zapisany być w pliku o dowolnej nazwie z rozszerzeniem *css.scss. Pliki musza być umieszczone w przeznaczonym do tego katalogu */app/assets/stylesheets*.</br>

W plikach z rozszerzeniem musza znaleźć się dwa kody:</br>

*@import „Bootstrap-sprockets”*</br>
*@import „Bootstrap”*</br>

Wymagane są również referencje do skryptów JavaScripts które wykorzystywane są przez platformę.</br>

*//= require Bootstrap-sprockets*</br>
*//= require Bootstrap*</br>

### 2.3 Baza danych

W projekcie posłużono się bazą danych Postgresql w wersji 9.5. Jest to jedna z trzech najpopularniejszych wolnodostępnych systemów zarządzania danymi. W Ruby on Rails wszystkie ustawienia bazy danych odbywają się w domyślnym pliku konfiguracyjnym config/database.yml. W pliku znajdują się trzy środowiska:
* deweloperskie
* testowe
* produkcyjne 

Poniżej znajduję się kod który został zamieszczony w projekcie:

## 3. Implementacja

### 3.1 Interfejs graficzny użytkownika

Pierwszy interfejs graficzny został stworzony w latach 70, XX wieku przez firme Xerox. Służy on do komunikowania się człowieka z oprogramowaniem komputera, wykorzystując obiekty wyświetlane na monitorze w trybie graficznym. Interfejs graficzny określa wygląd oraz funkcjonalność obiektów. Składa sie zazwyczaj z:
* menu
* wyświetlanych na ekarnie ikonek które oznaczają obiekty i polecenia
* okien wyświetlanych na ekranie
* funkcje dialogowe np. zapytania potwierdzajace usuniecie lub zmiane wydanego polecenia

W projekcie do stworzenia interfejsu wykorzystano framework Bootstrap który korzysta również z języka JavaScripts. 

## 4. Testy

### Test szybkości ładowania strony

Test szybkości ładowania strony polega na zbadaniu, to w jakim czasie ładuje się aplikacja. Im krótszy czas tym wyższa pozycja w Google. Według przeprowadzonych badań im wolniej ładuje się strona, tym mniej czasu spędza na niej użytkownik. Wywiera także istotny wpływ na przeglądanie podstron przez użytkownika i szybkie dotarcie przez niego do porządanych informacji co przekłada się na oszczędność czasu oraz oszczedność transferu w przypadku urządzeń mobilnych. Dzięki szybko działającej stronie roboty wyszukiwarek mogą szybciej przeskanować strone i wyszukać nowe treści.

Po wykonaniu testów narzędzie wskazało obszary w których miejscach należałoby użyć udoskonaleń, by strona ładowała się o wiele szybciej. Obszary dzielone są według trzech priorytetów: wysokim, średnim, niskim.</br>

Na podstawie badań PageSpeed Insights aplikacja otrzymała następujące wyniki:</br>

Szybkość działania strony na komputerach PC 86/100 - udoskonalenia na poziomie niskim</br>

Sugestie rekomendowane przez Google co należy poprawić:

1. Wyeliminuj blokujący renderowanie kod JavaScript i CSS z części strony widocznej na ekranie:
* Strona zawiera blokujące skrypty (3) i blokujące zasoby CSS (3). Powoduje to opóźnienia w renderowaniu strony.
2. 
Szybkość działania strony na urządzeniach mobilnych 69/100 - udoskonalenia na poziomie średnim</br>

Według PageSpeed Insights, strone można uznać za działającą dobrze kiedy wynik w obu testach osiągnie conajmniej 85 punktów.

### Walidacja kodu

Walidacja to inaczej proces weryfikowania poprawności składniowej pliku XHTML. Wyróznia się dwa rodzaje takiej poprawności składniowej: połączone z kontrolą zgodności z oficjalną specyfikacją XHTML, gdzie zastosowane zostają serwisy siecowe tak zwane parasery oraz sprawdzanie wyłącznie poprawności składniowej w tym przypadku sotosuje się specjalne programy do tego przeznaczone czyli walidatory. 

Dlaczego należy używać walidacji:
1. Ponieważ jeżeli kod strony jest poprawny to prawdopodobieństwo że strona będzie dobrze wyświetlana na większości przeglądarek jest większa. 
## Spis treści
1. Wprowadzenie
2. Wykorzystane technologie
* Ruby on Rails
* Bootstrap
* Baza danych
3. Implementacja
* Interfejs graficzny użytkownika
4. Elementy funkcjonalne systemu</br>

* Automatyzacja powiadomień
* Filtracja danych</br>
* Uaktywnienie przypominania hasła na e-mail</br>
* Uaktywnienie e-maili powitalych podczas rejestracji</br>
5. Testy
* Testowanie aplikacji na urządzeniach mobilnych
* Test szybkości ładowania strony
* Walidacja kodu
6. Podsumowanie
7. Bibliografia


## Literatura

1. http://getbootstrap.com/
2. http://helion.pl/ksiazki/ruby-on-rails-tworzenie-aplikacji-www-john-elder,rrtwww.htm
3. https://www.railstutorial.org/book
4. http://ruby-on-rails-tutorial.x25.pl/site
5. http://www.justinweiss.com/articles/search-and-filter-rails-models-without-bloating-your-controller/
6. http://quirktools.com/smaps/
7. https://rubygems.org/
8. http://api.rubyonrails.org/
9. http://bootsnipp.com/ 

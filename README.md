    
                                       AWARIA - SYSTEM REJESTRUJĄCY USTERKI I NAPRAWY
---------------------------------------------------------------------------------------------------------------------

## Keywords
aplikacja internetowa, ruby on rails, system rejestrowania, naprawa, bootstrap, interfejs graficzny użytkownika

## Autor
Dominika Pienczyn, numer albumu 236389

## Streszczenie

   Praca przedstawia aplikacje internetową o nazwie "Awaria" która jest systemem rejestrującym usterki oraz naprawy sprzętu i została stworzona w grupie 3-osobowej. Jako cel postawiłam sobie, wykonanie frontendu aplikacji oraz stworzenie poszczególnych elementów takich jak: automatyzacja powiadomień, filtracja danych, uaktywnienie resetowania hasła oraz e-maili powitalnych podczas rejestracji. Do stworzenia aplikacji wykorzystano system Linux, framework Ruby on Rails oraz Bootstrap a następnie wdrożono ją na serwer Heroku. Wgląd do szerszej dokumentacji możliwy jest pod adresem <https://github.com/dpienczyn/awaria1>, przechowywany od samego początku w repozytorium Githuba razem z kodem aplikacji.
  
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


   
## Spis treści
1. Wprowadzenie
2. Wykorzystane technologie
* Ruby on Rails
* Bootstrap
3. Implementacja
* Interfejs graficzny użytkownika
* Elementy funkcjonalne systemu</br>

 Automatyzacja powiadomień</br>
 Filtracja danych</br>
 Uaktywnienie przypominania hasła na e-mail</br>
 Uaktywnienie e-maili powitalych podczas rejestracji
4. Testy
* Testowanie aplikacji na urządzeniach mobilnych
* Test szybkości ładowania strony
* Walidacja kodu
5. Podsumowanie
6. Bibliografia


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

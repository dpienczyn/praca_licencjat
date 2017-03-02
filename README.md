
                                       AWARIA - SYSTEM REJESTRUJACY USTERKI I NAPRAWY
******************************************

##Keywords
aplikacja internetowa, ruby on rails, system rejestrowania, naprawa

##Autor
Dominika Pienczyn, numer albumu 236389

##Streszczenie
  Praca przedstawia aplikacje internetowa która jest systemem rejestrującym usterki oraz naprawy sprzętu. We wstępnej części swojej pracy skupiłam się na wymaganiach, jakich oprogramowanie musi sprostać. W kolejnym etapie opisuje technologie wybrane do implementacji oraz projekt tworzonego oprogramowania. Ostatni rozdział poświęcony jest opisowi narzędzi programistycznych wykorzystanych w implementacji.
  
##Wstęp

###1.1 Aplikacja internetowa

  Aplikacja internetowa zwana również aplikacja webową to program komputerowy który pracuje na serwerze i komunikuje się poprzez sieć komputerową z hostem użytkownika będącego w takim przypadku, interaktywnym klientem aplikacji internetowej.
Ich zaletą jest kompatybilność wieloplatformowa ponieważ nie zależą od systemu operacyjnego oraz cechuje je  łatwość w obsłudze. Do korzystania z aplikacji dany użytkownik potrzebuje tylko zainstalowanej przeglądarki internetowej. Dodatkowym atutem jest również to że w przypadku awarii urządzenia nie jesteśmy narażeni na utratę swoich danych gdyż są one gromadzone na serwerach dostawcy oprogramowania. W dzisiejszych czasach mamy szeroki wybór aplikacji, stają się one nieodłącznym elementem naszej codzienności, dzięki nim możemy np. uczyć się języka obcego niezależnie od tego w jakim położeniu się znajdujemy, możemy kontrolować ilość spożytych kalorii w ciągu dnia albo uzyskać rozpiskę z tygodniowym treningiem. Kolejnym plusem i chyba najbardziej cenionym jest to że z aplikacji nie tylko możemy korzystać na laptopie lub komputerze stacjonarnym ale na tablecie i smartfonie również.

###1.2 Cel aplikacji
  Stworzona aplikacja polega na rejestrowaniu usterek oraz napraw sprzętu. Klient – użytkownik po zarejestrowaniu się w systemie ma możliwość złożenia zgłoszenia tzn. zgłasza uszkodzony produkt uprzednio podając jego nazwę oraz opis uszkodzenia. Dodatkowo na bieżąco informowany jest droga elektroniczną o stanie swojego zgłoszenia. Zmiana statusu zgłoszenia przez pracownika powoduje automatyczne wygenerowanie odpowiedniego emaila i poinformowanie o tym użytkownika. Każdy z użytkowników ma możliwość wygenerowania PDF ze swoim zgłoszeniem. 
Posiadając uprawnienia administratora i pracownika mamy możliwość wglądu do zaplecza. Od strony zaplecza mamy miedzy innymi dostęp do statystyk, stanowisk, działów oraz zgłoszeń. Możemy edytować zgłoszenia tzn. zmieniać dany status zgłoszenia. Mamy możliwość przydzielenia pracownikowi stanowiska oraz działu jakim się zajmuje. 
Ogólnodostępne opcje to filtrowanie zgłoszeń, użytkowników, stanowisk oraz działów.

##Literatura

1. https://github.com/plataformatec/devise
2. http://helion.pl/ksiazki/ruby-on-rails-tworzenie-aplikacji-www-john-elder,rrtwww.htm
3. https://www.railstutorial.org/book
4. http://ruby-on-rails-tutorial.x25.pl/site
5. http://www.justinweiss.com/articles/search-and-filter-rails-models-without-bloating-your-controller/
6. https://github.com/mislav/will_paginate
7. https://rubygems.org/
8. http://api.rubyonrails.org/

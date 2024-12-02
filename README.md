Jest to raport Quarto w postaci dokumentu HTML z klasyfikacji binarnej metodą prostego (naiwnego) Bayesa i metodą KNN, czyli k najbliższych sąsiadów. Raport wykonany został w wersji dwujęzycznej. 

 

Potraktowałem to jako ćwiczenie z zastosowania  Pythona w klasyfikacji binarnej oraz z generowania raportu dwujęzycznego  w Quarto (RStudio). 

 

Dokument jest dostępny pod adresem: https://michaljk.github.io/klasyfikacja_binarna 

 

# Temat: Klasyfikacja binarna 

Jako podstawę działania wybrano bazę 'mtcars' ze środowiska R. Zawiera ona dane charakteryzujące silniki zawartych w bazie marek samochodów. Na potrzeby ćwiczenia została ona okrojona do bazy zawierającej dwie zmienne: ‘mpg’ – zmienna ciągła opisująca przebieg samochodu na jednym galonie benzyny oraz ‘vs’ – zmienna kategorialna, wyznaczająca typ silnika i przybierająca dwie wartości (‘0’ i’1’). Celem obliczeń było stworzenie modelu klasyfikującego silnik samochodu do konkretnego typu na podstawie znajomości jego przebiegu ‘mpg’. Zastosowano dwie metody: NB (Naive Bayes) i KNN (K Nearest Neighbors). 

Baza ćwiczeniowa została poprzez losowanie podzielona na bazę szkoleniową, zawierającą 80% rekordów danych oraz na bazę testującą (pozostałe 20%). 

Modele klasyfikacyjne stworzono z wykorzystaniem funkcji: GaussianNB() oraz KNeighborsClassifier() z bazy sklearn. Badanie dokładności modeli przeprowadzono metodą ‘accuracy’ i ‘kappa’. Zarówno NB, jak i KNN wykazały taką samą dokładność: accuracy =  0.857. Wskaźnik kappa był nieco wyższy dla KNN. Przeprowadzono również klasyfikacją na danych zewnętrznych. 

Klasyfikacja wraz z wyznaczonym prawdopodobieństwem została zilustrowana na wykresach z wykorzystaniem animacji w celu wyraźnego zaznaczenia wyników. 

Baza ‘mtcars’ liczy sobie zaledwie 32 rekordy danych. W związku z tym wynik klasyfikacji silnie zależy od sposobu losowania bazy treningowej i testowej. 

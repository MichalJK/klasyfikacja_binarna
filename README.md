Jest to raport Quarto w postaci dokumentu HTML z klasyfikacji binarnej metodą prostego (naiwnego) Bayesa i metodą KNN, czyli k najbliższych sąsiadów. Raport wykonany został w wersji dwujęzycznej.

Potraktowałem to jako ćwiczenie z zastosowania  Pythona w klasyfikacji binarnej oraz z generowania raportu dwujęzycznego  w Quarto (RStudio).

Dokument jest dostępny pod adresem: https://michaljk.github.io/klasyfikacja_binarna


# Temat: Klasyfikacja binarna
Jako podstawę działania wybrano bazę 'mtcars' ze środowiska R. Zawiera ona dane charakteryzujące silniki zawartych w bazie marek samochodów. Na potrzeby ćwiczenia została ona okrojona do bazy zawierającej dwie zmienne: ‘mpg’ – zmienna ciągła opisująca przebieg samochodu na jednym galonie benzyny oraz ‘vs’ – zmienna kategorialna, wyznaczająca typ silnika i przybierająca dwie wartości (‘0’ i’1’). Celem obliczeń było stworzenie modelu klasyfikującego silnik samochodu do konkretnego typu na podstawie znajomości jego przebiegu ‘mpg’. Zastosowano dwie metody: NB (Naive Bayes) i KNN (K Nearest Neighbors).
Baza ćwiczeniowa została poprzez losowanie podzielona na bazę szkoleniową, zawierającą 80% rekordów danych oraz na bazę testującą (pozostałe 20%).
Modele klasyfikacyjne stworzono z wykorzystaniem funkcji: GaussianNB() oraz KNeighborsClassifier() z bazy sklearn. Badanie dokładności modeli przeprowadzono metodą ‘accuracy’ i ‘kappa’. Zarówno NB, jak i KNN wykazały taką samą dokładność: accuracy =  0.857. Wskaźnik kappa był nieco wyższy dla KNN. Przeprowadzono również klasyfikacją na danych zewnętrznych.
Klasyfikacja wraz z wyznaczonym prawdopodobieństwem została zilustrowana na wykresach z wykorzystaniem animacji w celu wyraźnego zaznaczenia wyników.
Baza ‘mtcars’ liczy sobie zaledwie 32 rekordy danych. W związku z tym wynik klasyfikacji silnie zależy od sposobu losowania bazy treningowej i testowej.



&nbsp;




-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


&nbsp;



This is a Quarto report in the form of an HTML document on binary classification using the simple (naive) Bayes method and the k-nearest neighbor (KNN) method. The report was done in a bilingual version.

I treated it as an exercise in using Python for binary classification and in generating a bilingual report in Quarto (RStudio).

The document can be found at: https://michaljk.github.io/klasyfikacja_binarna


# Topic: Binary Classification

The database 'mtcars' from the R environment was chosen as the basis for the activity. It contains data characterizing the engines of the car brands included in the database. For the purposes of the exercise, it was truncated to a database containing two variables: 'mpg', a continuous variable describing the mileage of the car per gallon of gasoline, and 'vs', a categorical variable describing the engine type that takes two values ('0' and '1'). The goal of the calculations was to create a model that would classify a car's engine into a particular type based on knowledge of its 'mpg' mileage. Two methods were used: NB (Naive Bayes) and KNN (K Nearest Neighbors).

The training base was randomized into a training base containing 80% of the datasets and a test base (the remaining 20%).

Classification models were built using the functions: GaussianNB() and KNeighborsClassifier() from the sklearn database. The accuracy of the models was tested using the 'accuracy' and 'kappa' methods. Both NB and KNN showed the same accuracy: accuracy = 0.857. The kappa index was slightly higher for KNN. Classification was also performed on external data.

The classification along with the obtained probability was presented in graphs using animation to highlight the results.

The 'mtcars' database has only 32 records. Therefore, the classification result depends strongly on how the training and test bases are drawn.





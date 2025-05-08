# Opis
Projekt ma na celu przeprowadzenie analizy porównawczej gotowych modeli predykcyjnych z własnym modelem tworzonym krok po kroku. Dane dotyczą obrotu restauracji. Zawierają datę, obrót i liczbę konkurencji.
# Implementacja
Zbiór danych został uprzednio, w pliku xlsx, podzielony na treningowy i testowy. Spośród gotowych modeli zastsowano Regresion Tree, Random Forest, ich modyfikację oraz Linear Regression.
Własny model jest oparty na zauważeniu powtarzających się wzorców w danych. Można dostrzec, że w obrocie występują wahania dobowe regularne dla danych dni. Występują też wahania wynikające z sezonu, obserwowane dla konkretnych miesięcy. Ilość konkurencyjnych resturacji również ma wpływ na obrót tej restauracji.
# Podsumowanie
Jako metrykę zastosowano błąd względny. Najlpeszymi i bardzo zbliżonymi do siebie wynikami okazały się modele Linear Regression oraz własny model.
# Jak używać?
1. Zainstalowanie platfomy KNIME https://www.knime.com/downloads
2. Otworzyć w aplikacji KNIME plik Prognozowanie.knwf
3. W ustawieniach nodów Excel Reader upewnić się, że ścieżka do pliku Grupowanie.xlsx jest ustawiona poprawnie oraz że w pierwszym ustawiono arkusz treningowy, a w drugim testowy.
4. Wyniki metryki predykcji można znaleźć w node Column Filter przy każdym modelu, w zakładce Statistics.

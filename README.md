# Optymalizacja_TSP_Metaheurystyki
**OPTYMALIZACJA PROBLEMU KOMIWOJAŻERA (TSP) – ANALIZA METAHEURYSTYK | 12/2025**

**Narzędzia**
  * Python
  * NumPy
  * Pandas
  * Matplotlib
  * Excel Solver

**Problem** 

Konieczność znalezienia optymalnej trasy w NP-trudnym Problemie Komiwojażera (TSP) dla instancji o rosnącej skali (48, 76, 127 miast), poprzez porównanie skuteczności szerokiego spektrum algorytmów inteligencji obliczeniowej i metaheurystyk w kontekście jakości rozwiązań oraz czasu obliczeń.

**Rozwiązanie**
  * Zaimplementowano 7 algorytmów: NN, IHC, SA, GA, FA, TS oraz hybrydę GA+SA
  * Przeprowadzono pełną analizę parametryczną (projekt czynnikowy) dla kluczowych metaheurystyk
  * Zweryfikowano wyniki względem rozwiązania referencyjnego z Solvera
  * Zbadano wpływ operatorów sąsiedztwa (swap, insert, 2-opt) na zbieżność
  * Opracowano autorskie usprawnienia: intensyfikacja wyszukiwania lokalnego i hybrydyzacja GA z SA
  * Przeanalizowano stabilność i wariancję wyników dla 5 niezależnych przebiegów każdego scenariusza

**Wynik**
  * Algorytmy GA i TS konsekwentnie dostarczały trasy o najniższym koszcie
  * Operator 2-opt zdominował wszystkie metody jako najskuteczniejszy ruch lokalny
  * Hybryda GA+SA poprawiła eksploatację, osiągając wyniki na poziomie czystego GA
  * Zidentyfikowano optymalne zakresy parametrów: populacja 400, 800 generacji, chłodzenie wykładnicze 0.9995
  * Proste heurystyki (NN, IHC) okazały się najmniej skuteczne (błąd względem optimum >10%)
  * Algorytm świetlikowy (FA) wykazał dużą wariancję i wrażliwość na parametry startowe
  * Projekt zrealizowano w zespole 5-osobowym z pełną dokumentacją w PDF




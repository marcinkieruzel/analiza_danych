# Analiza cen kakao - Przykład dla studentów

Przykładowy projekt analizy danych dla pierwszych zajęć z analizy danych.

## Opis projektu

Projekt zawiera analizę historycznych cen kakao (ICCO Daily Prices) z lat 1994-2025 z wykorzystaniem:
- **Regresji liniowej** - do przewidywania trendów długoterminowych
- **Wygładzania wykładniczego (Exponential Smoothing)** - do modelowania sezonowości i krótkoterminowych prognoz

## Wymagania

- Python 3.12+
- Jupyter Notebook

## Instalacja

1. Sklonuj repozytorium lub pobierz pliki
2. Utwórz środowisko wirtualne:
```bash
python3 -m venv env
```

3. Aktywuj środowisko:
```bash
source env/bin/activate  # Linux/Mac
# lub
env\Scripts\activate  # Windows
```

4. Zainstaluj wymagane pakiety:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels jupyter
```

## Uruchomienie

1. Aktywuj środowisko wirtualne (jeśli nie jest aktywne)
2. Uruchom Jupyter Notebook:
```bash
jupyter notebook
```

3. Otwórz plik `analiza_kakao.ipynb`
4. Uruchom kolejno komórki noteBooka

## Zawartość

### Dane
- `icco_daily_prices_1994-2025.csv` - dane historyczne cen kakao ICCO

### Notebook
- `analiza_kakao.ipynb` - główny notebook z analizą

### Struktura analizy

1. **Wczytanie i przygotowanie danych**
   - Import danych CSV
   - Konwersja dat
   - Statystyki opisowe

2. **Wizualizacja danych historycznych**
   - Wykres cen w czasie
   - Histogramy i wykresy pudełkowe

3. **Regresja liniowa**
   - Podział na zbiór treningowy i testowy (80/20)
   - Budowa modelu regresji
   - Ocena modelu (MSE, RMSE, R², MAE)
   - Predykcja na 90 dni do przodu

4. **Wygładzanie wykładnicze (Holt-Winters)**
   - Model z trendem i sezonowością
   - Ocena modelu
   - Predykcja na 90 dni do przodu

5. **Porównanie modeli**
   - Analiza błędów predykcji
   - Wizualizacja porównawcza
   - Podsumowanie wyników

## Metryki oceny

- **MSE** (Mean Squared Error) - średni błąd kwadratowy
- **RMSE** (Root Mean Squared Error) - pierwiastek ze średniego błędu kwadratowego
- **MAE** (Mean Absolute Error) - średni błąd bezwzględny
- **R²** (R-squared) - współczynnik determinacji

## Nauczone umiejętności

Ten projekt pozwala nauczyć się:
- Wczytywania i przetwarzania danych w pandas
- Wizualizacji danych za pomocą matplotlib i seaborn
- Budowy modeli regresji liniowej (scikit-learn)
- Stosowania modeli szeregów czasowych (statsmodels)
- Oceny i porównywania modeli
- Tworzenia prognoz
- Pracy z Jupyter Notebook

## Zadania dla studentów

1. Spróbuj zmienić proporcję podziału train/test
2. Dodaj inne modele regresji (regresja wielomianowa, Ridge, Lasso)
3. Zmodyfikuj parametry sezonowości w modelu Holt-Winters
4. Stwórz predykcje na inne okresy czasu (30, 60, 180 dni)
5. Dodaj analizę reszt (residuals) dla obu modeli
6. Wypróbuj inne modele szeregów czasowych (ARIMA, Prophet)

## Autor

Materiał dydaktyczny dla pierwszych zajęć z analizy danych.

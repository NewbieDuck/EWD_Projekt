# Analiza wpływu gamingu na wyniki akademickie i zawodowe 🎮📚

## Opis projektu
Celem projektu realizowanego w ramach przedmiotu **Ewaluacja i Wizualizacja Danych (EWD)** jest przeprowadzenie pełnego cyklu eksperymentu Data Science na wybranym zbiorze danych.

Głównym założeniem eksperymentu jest:
* **Stworzenie modelu predykcyjnego** przewidującego wyniki (Score).
* **Analiza wpływu nawyków grania** oraz stylu życia (sen, stres) na wydajność akademicką i zawodową.

---

## 📊 Dane (Dataset)
Dane zostały pozyskane z platformy **Kaggle**: 
[Gaming Hours vs Academic & Work Performance](https://www.kaggle.com/datasets/prince7489/gaming-hours-vs-academic-and-work-performance)

### Charakterystyka danych:
* **Zmienna docelowa:** `Academic_or_Work_Score` (zakres 55–95).
* **Główne cechy (Features):**
    * Nawyki gamingowe (godziny dzienne/tygodniowe, typy gier).
    * Styl życia (godziny snu, poziom stresu).
    * Dane demograficzne (wiek, zawód, płeć).

---

## 🎯 Cele eksperymentu
1. **Faza 1: Cel i Ewaluacja** - Zdefiniowanie problemu i przyjęcie metryki sukcesu (zakładany błąd MAE < 10% zakresu zmiennej).
2. **Faza 2: Eksploracyjna Analiza Danych (EDA)** - Wizualizacja rozkładów, szukanie korelacji oraz identyfikacja wartości odstających (outliers) za pomocą wykresów pudełkowych.
3. **Faza 3: Przygotowanie danych** - Czyszczenie zbioru (usunięcie `User_ID`, `Productivity_Level`), kodowanie zmiennych kategorycznych oraz podział na zbiór treningowy i testowy.
4. **Faza 4: Modelowanie** - Budowa i trenowanie modeli regresyjnych.
5. **Faza 5: Ewaluacja** - Porównanie wyników i wyciągnięcie wniosków.

---

## 🛠️ Wykorzystane technologie
* **Język:** Python 🐍
* **Biblioteki:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

---
**Autor:** Newbie Duck
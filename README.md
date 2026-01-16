# Przewidywanie jakości czerwonego wina 🍷📊

## Opis projektu
Celem projektu realizowanego w ramach przedmiotu **Ewaluacja i Wizualizacja Danych (EWD)** jest przeprowadzenie pełnego cyklu eksperymentu Data Science na zbiorze danych dotyczącym parametrów fizykochemicznych czerwonego wina.

Głównym założeniem eksperymentu jest:
* **Stworzenie modelu predykcyjnego**, który na podstawie składu chemicznego wina przewidzi jego ocenę jakości (`quality`).
* **Zbadanie wpływu poszczególnych składników** (np. alkoholu, kwasowości, siarczanów) na końcową ocenę wystawioną przez ekspertów.

---

## 📊 Dane (Dataset)
Dane pochodzą z platformy **Kaggle**: 
[Red Wine Quality Dataset](https://www.kaggle.com/datasets/uciml/red-wine-quality-cortez-et-al-2009)

### Charakterystyka danych:
* **Zmienna docelowa:** `quality` (skala dyskretna od 4 do 8).
* **Główne cechy (Features):**
    * `alcohol`: Zawartość alkoholu (najsilniejszy pozytywny predyktor).
    * `volatile acidity`: Kwasowość lotna (wysoka zawartość obniża jakość).
    * `sulphates`: Zawartość siarczanów.
    * `citric acid`: Zawartość kwasu cytrynowego.
    * `pH`, `density`, `chlorides`, `residual sugar` i inne parametry chemiczne.

---

## 🎯 Cele eksperymentu
1. **Faza 1: Cel i Ewaluacja** - Zdefiniowanie problemu regresji i przyjęcie metryk sukcesu (MAE, RMSE, R²).
2. **Faza 2: Eksploracyjna Analiza Danych (EDA)** - Analiza macierzy korelacji, wizualizacja rozkładów oraz identyfikacja najsilniejszych czynników wpływających na jakość.
3. **Faza 3: Przygotowanie danych (Preprocessing)** - Czyszczenie zbioru z wartości odstających przy użyciu metody **Z-score** (usunięcie rekordów wykraczających poza zakres +/- 3 odchylenia standardowe).
4. **Faza 4: Modelowanie** - Trening modeli takich jak Random Forest Regressor, k-NN oraz Regresja Liniowa.
5. **Faza 5: Ewaluacja** - Porównanie wyników i analiza istotności cech (Feature Importance).

---

## 📈 Kluczowe spostrzeżenia
* Wstępna analiza korelacji wykazała, że **zawartość alkoholu** jest najsilniej powiązana z wysoką jakością wina.
* Wysoka **kwasowość lotna (volatile acidity)** koreluje ujemnie z oceną, co sugeruje jej negatywny wpływ na profil smakowy.
* Usunięcie wartości odstających pozwoliło na ustabilizowanie rozkładów cech przed procesem modelowania.

---

## 🛠️ Wykorzystane narzędzia
* **Python** (Pandas, NumPy)
* **Seaborn / Matplotlib** (Wizualizacja danych)
* **Scikit-learn** (Modelowanie i ewaluacja)
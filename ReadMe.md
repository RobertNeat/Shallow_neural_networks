# Projekt Analizy Danych z Użyciem Sieci Neuronowych

## Opis

Projekt obejmuje analizę danych z użyciem sieci neuronowych. Poniżej znajdują się instrukcje dotyczące przygotowania danych, budowy modeli sieci neuronowych oraz wyniki testów wydajnościowych.

## Wczytywanie Danych

Do wczytania danych używamy biblioteki Pandas oraz narzędzia Google Colab. Dane zostają wczytane z pliku Excela (`practice_lab_3.xlsx`) znajdującego się na dysku Google Drive.

## Przygotowanie Danych

Kolejnym krokiem jest przekształcenie cech jakościowych na ilościowe za pomocą kodowania typu 'One-Hot Encoding'. Następnie zbiór danych jest dzielony na zbiór uczący i testowy, a wartości są skalowane.

## Zadanie 6.2

Tworzymy model sieci neuronowej z warstwami Dense i Dropout. Przeprowadzamy przeszukiwanie gridowe w celu optymalizacji parametrów. Ostateczne wykresy prezentują przebieg wartości metryk w zależności od liczby epok dla różnych wartości współczynnika Dropout.

## Zadanie 6.3

Analogicznie do zadania 6.2, z wykorzystaniem warstw GaussianNoise, przeprowadzamy testy wydajnościowe dla różnych poziomów szumu.

## Zadanie 6.4

Ostatni etap to budowa modeli z różnymi kombinacjami warstw: Dense, BatchNormalization, LayerNormalization, Dropout, GaussianNoise. Przeprowadzamy przeszukiwanie gridowe dla różnych konfiguracji modeli.

## Podsumowanie

Każda sekcja zawiera opis wykonanych działań oraz prezentuje wyniki testów i analizy danych.

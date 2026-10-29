# Analýza výmenných kurzov EUR/USD a GBP/USD

Projekt sa zameriava na analýzu vývoja a volatility výmenných kurzov EUR/USD a GBP/USD.

Analýza využíva denné údaje za obdobie 2021-2024, ARMA modely a modely volatility v jazyku R.

## Obsah projektu

- grafické porovnanie kurzov a ich logaritmických výnosov,
- analýza stacionarity pomocou ACF a PACF,
- výber ARMA modelov podľa AIC,
- diagnostika rezíduí pomocou štatistických testov,
- porovnanie modelov GARCH, EGARCH a GJR-GARCH,
- jednodňová prognóza a analýza vzťahu medzi výmennými kurzami.

Pre EUR/USD bol vybraný model ARMA(0,1) a pre GBP/USD ARMA(2,3). Pri oboch kurzoch dosiahol najnižšie AIC model EGARCH(1,1), ktorý umožňuje zachytiť asymetrickú reakciu volatility na trhové šoky. Korelácia denných výnosov bola 0,758.

## Použité nástroje

R, R Markdown, `readxl`, `xts`, `astsa`, `forecast`, `tseries`, `FinTS`, `rugarch`.

## Súbory projektu

- `eurusd_gbpusd.Rmd` - zdrojový dokument s kódom a interpretáciou.
- `eurusd_gbpusd.html` - vykreslený výstup analýzy.
- `eurusd.xlsx`, `gbpusd.xlsx` - vstupné dátové súbory.


# Analiza rynku muzycznego Spotify
[Available only in polish]

## Spis treści
- [Opis projektu](#opis-projektu)
- [Struktura projektu](#struktura-projektu)
- [Notebook](#notebook)
- [PDF](#pdf)
- [Dane](#dane)
- [Wymagania](#wymagania)
- [Użyte narzędzia](#użyte_narzędzia)
- [Wyniki](#wyniki)
- [Użycie](#użycie)
- [Wkład](#wkład)
- [Licencja](#licencja)

## Opis projektu
Niniejszy projekt to moja praca licencjacka, zrealizowana na kierunku Informatyka i Ekonometria, Wydziału Nauk Ekonomicznych Uniwersytetu Warszawskiego, pod kierunkiem dr. hab. Katarzyny Kopczewskiej, prof. ucz. Praca zawiera analizę rynku muzycznego Spotify z wykorzystaniem różnych metod statystycznych i technik uczenia maszynowego.

## Struktura projektu
Projekt składa się z trzech głównych części:
1. **Jupyter Notebook**: `Spotify_market_analysis.ipynb`
2. **Dokument PDF**: `Spotify_rynek.pdf`
3. **Zbiór baz danych niezbędnych do przeprowadzenia analizy**: 'bazy_danych' (UWAGA: dodatkowo wymagane jest własnoręczne umieszczenie w folderze zbioru dotyczącego playlist użytkowaników, patrz rozdział Użycie)

### Notebook
Notebook zawiera kod użyty do analizy danych pobranych z platformy Spotify. 

### PDF
Dokument PDF zawiera pełny opis badania, w tym przegląd literatury, metodologię badania, analizę danych oraz wnioski.

## Dane
W projekcie wykorzystano dane z API Spotify zlokalizowane na platformie Kaggle. Zawierają one informacje o utworach, artystach, albumach oraz ich popularności. Dane te zostały przetworzone i zanalizowane za pomocą narzędzi takich jak Pandas, NumPy oraz Matplotlib.

## Wymagania
- Python 3.7+
- Jupyter Notebook lub JupyterLab Notebook
- Baza danych "spotify_users_playlist" (patrz punkt 2. w poniższym rozdziale)

## Użyte narzędzia
Techniki statystyczne oraz techniki uczenia maszynowego użyte w badaniu:
- Normalizacja zmiennych
- Test Jarque-Bera: test normalności rozkładu
- Test Barlett'a: test homogeniczności wariancji
- Test Kruskala-Wallisa: nieparametryczny test równości median
- Test ANOVA: test równości średnich
- Testy porównań parami (Manna-Whitney'a, Wilcoxon'a, Tukey'a)
- Klastrowanie K-średnich: technika grupowania danych na podstawie ich cech, z wykorzystaniem metryki euklidesowej
- Współczynnik Silhouette
- Wykres łokcia
- Współczynnik Gini'ego
- korekta Bonferonniego

# Wyniki
Najważniejsze wnioski i wyniki z przeprowadzonego badania:
- Istnieje **heterogeniczność preferencji muzycznych co do najpopularniejszych utworów** wśród użytkowników Spotify
- **45,69%** ogółu badanych utworów stanowią utwory o **skrajnie długim czasie trwania**
- **40,31%** ogółu badanych utworów stanowią utwory o **bardzo wyrazistym charakterze energicznym**
- **39,66%** ogółu badanych utworów stanowią utwory o **relatywnie wysokim poziomie melancholii**
- Potwierdzono możliwość występowania zjawiska **„TikTok-to-Spotify pipeline”**. Jednakże, z powodu braku odpowiednio wysokiej jakości danych, nie przeprowadzono w pełni empirycznej analizy tego zagadnienia.

## Użycie
Aby uruchomić analizę, wykonaj poniższe kroki:

1. Sklonuj lub pobierz repozytorium

2. Pobierz bazę danych z playlistami użytkowników, zmień jej nazwę na "spotify_users_playlists" oraz umieść w folderze "bazy_danych". Dane te nie mogły zostać udostępnione za pomocą GitHuba ze względu na swój duży rozmiar. Wspomniane dane dostępne są pod tym linkiem: https://www.kaggle.com/datasets/andrewmvd/spotify-playlists?select=spotify_dataset.csv
   
3. Otwórz Jupyter Notebook lub JupyerLab Notebook

4. Uruchom wszystkie komórki, aby zobaczyć wyniki analizy. Zachęcam również do zapoznania się z dokładną treścią analizy w pliku PDF :) 

## Wkład
Jeśli chcesz przyczynić się do rozwoju tego projektu, proszę o zgłoszenie problemów oraz tworzenie pull requestów. Zapraszam do współpracy!

## Licencja
Ten projekt jest licencjonowany na podstawie licencji MIT. Szczegóły znajdują się w pliku `LICENSE`.

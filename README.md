# Analiza i wizualizacja widma częstotliwości fal dźwiękowych

## 1. Cel projektu
 - Stworzenie oprogramowania umożliwiającego odczyt sygnałów
dźwiękowych oraz wizualizację widma częstotliwości w czasie
rzeczywistym.

## 2. Wykorzystany sprzęt
- Laptop z systemem operacyjnym Ubuntu 20.04

## 3. Zastosowane metody
- Odczyt próbek dźwiękowych z karty dźwiękowej za pomocą ALSA -
modułu jądra Linux.
- Transformacja próbek z domeny amplitudowej do domeny
częstotliwościowej z użyciem algorytmu FFT - szybkiej transformaty
Fouriera.
- Wizualizacja zmieniającego się widma częstotliwości w trzech
wymiarach w dynamicznej stronie HTML ze skryptem JavaScript
wykorzystującym bibliotekę vis-graph3d.

## 4. Niskopoziomowe komponenty
- moduł w języku C odpowiedzialny za odczyt próbek dźwiękowych z
ALSA i grupowanie próbek w partie wykorzystywane później przez FFT
- własnoręczna implementacja algorytmu FFT w języku Python

## 5. Przygotowanie środowiska
```shell
sudo apt-get install libasound2-dev libasound2
```

## 6. Bibliografia
- *Making Sense of the Audio Stack on Unix* - wpis na blogu “Venam’s
Blog” autorstwa Patricka Louisa - https://venam.nixers.net/blog/unix/2021/02/07/audio-stack.html
- *Sound Programming: Alsa Tutorial* - https://soundprogramming.net/programming/alsa-tutorial-1-initialization/
- *A Tutorial on Using the ALSA Audio API* - http://equalarea.com/paul/alsa-audio.html

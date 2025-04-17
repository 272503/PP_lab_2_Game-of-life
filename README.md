# PP_lab_2_Game-of-life

# Game of Life (Conway’s Game of Life) – Terminal Simulation

## Opis projektu

Ten projekt to prosta symulacja **Gry w Życie Conwaya** uruchamiana w terminalu. Gra w Życie to automat komórkowy, który demonstruje, jak złożone wzorce mogą powstać z prostych reguł.

Każda komórka na dwuwymiarowej planszy ma dwa możliwe stany: **żywa (alive)** lub **martwa (dead)**. Przy każdej iteracji plansza aktualizuje się na podstawie liczby żywych sąsiadów każdej komórki.

---

## Jak uruchomić

### Wymagania

- Python 3.6+

### Uruchomienie w terminalu

```bash
python game_of_life.py
```
Domyślna siatka to 20×20, z losowo ustawionym stanem komórek

### Zasady gry (reguły Conwaya)
Każda komórka na planszy zachowuje się według następujących reguł:

1. Przetrwanie: Komórka żywa z 2 lub 3 żywymi sąsiadami przeżywa do następnej generacji.

2. Śmierć z powodu samotności: Komórka żywa z mniej niż 2 żywymi sąsiadami umiera.

3. Śmierć z przeludnienia: Komórka żywa z więcej niż 3 żywymi sąsiadami umiera.

4. Narodziny: Komórka martwa z dokładnie 3 żywymi sąsiadami staje się żywa.

### Struktura projektu

.
├── game_of_life.py      # Główna aplikacja z definicją klasy Cell i Grid
└── README.md            # Dokumentacja projektu

### Przykładowy wygląd w terminalu
```bash
 O  O     O  O
 O           O
    O  O  O
 O           O
 O  O     O  O
```
Każde `O`to żywa komórka, a puste miejsce reprezentuje komórkę martwą.

### Autor
Projekt stworzony przez Piotra Kosiora jako prosty przykład działania automatu komórkowego w terminalu.

# Zaawansowane Języki Programowania - WesołyWąż

### Informacje podstawowe:

| Wykonawcy | Prowadzący | Język<br>programowania | Narzędzie<br>analizy kodu | Źródło kodu | Data oddania |
:-:|:-:|:-:|:-:|:-:|:-:
| Mateusz Labuda<br> Wojciech Januszk <br>Michał Gorzkowski | dr Bzyl Włodzimierz | [Python](https://www.python.org/) | [Radon](https://radon.readthedocs.io/en/latest/) | [Martin Fowler's book Refactoring](https://martinfowler.com/books/refactoring.html) | 26.01.2019

---

Halstead Effort (złożoność Halsteada) - takie metryki jak: liczba unikatowych operatorów, liczba unikatowych operandów, całkowita liczba wystąpień operatorów oraz całkowita liczba wystąpień operandów, które dotyczą rozmiaru programu, pozwalają na zdefiniowanie bardziej skomplikowanych metryk złożoności. Wyróżnia się wśród nich m. in. trudność, poziom programu, wysiłek, czas, szacunkową liczbę błędów. Im mniejsza wartość, tym lepiej.

## Before

```
$ radon hal *

customer.py:
    effort: 2364.2626656801754

movie.py:

    effort: 0

rental.py:
    effort: 0

```
effort: 2364.2626656801754

## After 3 steps
```
$ radon hal *

customer.py:
    effort: 117.1120418468254

movie.py:

    effort: 0

rental.py:

    effort: 1214.0175180589347
```
effort: 117.1120418468254  
effort: 1214.0175180589347



## Refactored

```
$ radon hal *
customer.py:
    effort: 117.1120418468254

movie.py:
    effort: 426.2062467936566

rental.py:
    effort: 0
```
effort: 117.1120418468254  
effort: 426.2062467936566
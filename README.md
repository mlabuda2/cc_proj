Refactoring example in Python. Based on an example in Martin Fowler's book Refactoring.

## Before

```
$ radon hal *
customer.py:
    h1: 6
    h2: 44
    N1: 32
    N2: 64
    vocabulary: 50
    length: 96
    calculated_length: 255.724766224368
    volume: 541.8101942183736
    difficulty: 4.363636363636363
    effort: 2364.2626656801754
    time: 131.34792587112085
    bugs: 0.1806033980727912
movie.py:
    h1: 0
    h2: 0
    N1: 0
    N2: 0
    vocabulary: 0
    length: 0
    calculated_length: 0
    volume: 0
    difficulty: 0
    effort: 0
    time: 0.0
    bugs: 0.0
rental.py:
    h1: 0
    h2: 0
    N1: 0
    N2: 0
    vocabulary: 0
    length: 0
    calculated_length: 0
    volume: 0
    difficulty: 0
    effort: 0
    time: 0.0
    bugs: 0.0

```
effort: 2364.2626656801754


## After

```
$ radon hal *
customer.py:
    h1: 1
    h2: 28
    N1: 15
    N2: 30
    vocabulary: 29
    length: 45
    calculated_length: 134.6059378176129
    volume: 218.60914478074076
    difficulty: 0.5357142857142857
    effort: 117.1120418468254
    time: 6.506224547045856
    bugs: 0.07286971492691359
movie.py:
    h1: 4
    h2: 11
    N1: 10
    N2: 20
    vocabulary: 15
    length: 30
    calculated_length: 46.053747805010275
    volume: 117.20671786825557
    difficulty: 3.6363636363636362
    effort: 426.2062467936566
    time: 23.67812482186981
    bugs: 0.03906890595608519
rental.py:
    h1: 0
    h2: 0
    N1: 0
    N2: 0
    vocabulary: 0
    length: 0
    calculated_length: 0
    volume: 0
    difficulty: 0
    effort: 0
    time: 0.0
    bugs: 0.0
test_customer.py:
    h1: 1
    h2: 2
    N1: 1
    N2: 2
    vocabulary: 3
    length: 3
    calculated_length: 2.0
    volume: 4.754887502163469
    difficulty: 0.5
    effort: 2.3774437510817346
    time: 0.1320802083934297
    bugs: 0.0015849625007211565

```
 effort: 117.1120418468254
effort: 426.2062467936566
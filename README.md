# Методы оптимизации
## Лабораторная работа №1
**Вариант 2**

f(x) = cos(x), x in [0, pi]
### Метод дихотомии

**Epsilon** | **Delta** | **x** | **f(x)** | **iterations**
--- | --- | --- | --- | ---
0.1 | 0.025 | 3.0924395824 | -0.9987922310 | 6
0.01 | 0.0025 | 3.1375611106 | -0.9999918733 | 10
0.001 | 0.00025 | 3.1411509329 | -0.9999999024 | 13
0.00001 | 0.0000025 | 3.1415886520 | -1.0000000000 | 20
0.0000001 | 0.000000025 | 3.1415926016 | -1.0000000000 | 26

### Метод золотого сечения

**Epsilon** | **x** | **f(x)** | **iterations**
--- | --- | --- | ---
0.1 | 3.1081563083 | -0.9994410575 | 8
0.01 | 3.1367143535 | -0.9999881011 | 12
0.001 | 3.1411527743 | -0.9999999033 | 17
0.00001 | 3.1415890735 | -1.0000000000 | 27
0.0000001 | 3.1415926029 | -1.0000000000 | 36

### Метод Фиббоначи

n: 91

F_{n-2}: 2880067194370816120

F_{n-1}: 4660046610375530309

F_{n}: 7540113804746346429

**Epsilon** | **x** | **f(x)** | **iterations**
--- | --- | --- | ---
0.1 | 3.1081563083 | -0.9994410575 | 9
0.01 | 3.1367143535 | -0.9999881011 | 13
0.001 | 3.1411527743 | -0.9999999033 | 18
0.00001 | 3.1415890735 | -1.0000000000 | 28
0.0000001 | 3.1415926041 | -1.0000000000 | 37

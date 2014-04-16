# Методы оптимизации
### Выполнил: Баев Дмитрий, гр. 4539

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

F<sub>n-2</sub>: 2880067194370816120

F<sub>n-1</sub>: 4660046610375530309

F<sub>n</sub>: 7540113804746346429

**Epsilon** | **x** | **f(x)** | **iterations**
--- | --- | --- | ---
0.1 | 3.1081563083 | -0.9994410575 | 9
0.01 | 3.1367143535 | -0.9999881011 | 13
0.001 | 3.1411527743 | -0.9999999033 | 18
0.00001 | 3.1415890735 | -1.0000000000 | 28
0.0000001 | 3.1415926041 | -1.0000000000 | 37

## Лабораторная работа №2
*Решение линейной задачи симплекс-методом*

**Вариант 2**

**A =** 
<table>
<tr><td>−1</td> <td>3</td> <td>0</td> <td>2</td> <td>1</td></tr>
<tr><td>2</td> <td>−1</td> <td>1</td> <td>2</td> <td>3</td></tr>
<tr><td>1</td> <td>−1</td> <td>2</td> <td>1</td> <td>0</td></tr>
</table>

<table>
<tr><td>1</td><td>1</td><td>1</td><td>0</td><td>0</td><td>-1</td><td>3</td><td>0</td><td>2</td><td>1</td></tr>
<tr><td>2</td><td>4</td><td>0</td><td>1</td><td>0</td><td>2</td><td>-1</td><td>1</td><td>2</td><td>3</td></tr>
<tr><td>3</td><td>5</td><td>0</td><td>0</td><td>1</td><td>1</td><td>-1</td><td>2</td><td>1</td><td>0</td></tr>
<tr><td></td><td>10</td><td>0</td><td>0</td><td>0</td><td>2</td><td>1</td><td>3</td><td>5</td><td>4</td></tr>
</table>

**k = 4, s = 2**

<table>
<tr><td>5</td><td>6/5</td><td>2/5</td><td>1/5</td><td>0</td><td>0</td><td>1</td><td>1/5</td><td>6/5</td><td>1</td></tr>
<tr><td>4</td><td>13/5</td><td>1/5</td><td>3/5</td><td>0</td><td>1</td><td>0</td><td>3/5</td><td>8/5</td><td>2</td></tr>
<tr><td>3</td><td>18/5</td><td>1/5</td><td>-2/5</td><td>1</td><td>0</td><td>0</td><td>8/5</td><td>3/5</td><td>-1</td></tr>
<td>  </td><td>18/5</td><td>-4/5</td><td>-7/5</td><td>0</td><td>0</td><td>0</td><td>8/5</td><td>3/5</td><td>-1</td>
</table>

**k = 5, s = 1**

<table>
<tr><td>5</td><td>6/5</td><td>2/5</td><td>1/5</td><td>0</td><td>0</td><td>1</td><td>1/5</td><td>6/5</td><td>1</td></tr>
<tr><td>4</td><td>13/5</td><td>1/5</td><td>3/5</td><td>0</td><td>1</td><td>0</td><td>3/5</td><td>8/5</td><td>2</td></tr>
<tr><td>3</td><td>18/5</td><td>1/5</td><td>-2/5</td><td>1</td><td>0</td><td>0</td><td>8/5</td><td>3/5</td><td>-1</td></tr>
<td>  </td><td>18/5</td><td>-4/5</td><td>-7/5</td><td>0</td><td>0</td><td>0</td><td>8/5</td><td>3/5</td><td>-1</td>
</table>

**k = 6, s = 3**

<table>
<tr><td>5</td><td>3/4</td><td>3/8</td><td>1/4</td><td>-1/8</td><td>0</td><td>1</td><td>0</td><td>9/8</td><td>9/8</td></tr>
<tr><td>4</td><td>5/4</td><td>1/8</td><td>3/4</td><td>-3/8</td><td>1</td><td>0</td><td>0</td><td>11/8</td><td>19/8</td></tr>
<tr><td>6</td><td>9/4</td><td>1/8</td><td>-1/4</td><td>5/8</td><td>0</td><td>0</td><td>1</td><td>3/8</td><td>-5/8</td></tr>
<td>  </td><td>0</td><td>-1</td><td>-1</td><td>-1</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td>
</table>

**5/4 3/4 9/4 0 0**

<table>
<tr><td>1</td><td>5/4</td><td>1</td><td>0</td><td>0</td><td>11/8</td><td>19/8</td></tr>
<tr><td>2</td><td>3/4</td><td>0</td><td>1</td><td>0</td><td>9/8</td><td>9/8</td></tr>
<tr><td>3</td><td>9/4</td><td>0</td><td>0</td><td>1</td><td>3/8</td><td>-5/8</td></tr>
<tr><td>  </td><td>-23/4</td><td>0</td><td>0</td><td>0</td><td>-57/8</td><td>-41/8</td></tr>
</table>

## Лабораторная работа №3
*Решениe транспортной задачи*

### Первое решение. Метод северо-западного угла 

<table border="0" cellpadding="2" cellspacing="2" class="body_txt">
    <tbody>
        <tr>
            <td height="15" align="middle" valign="middle" rowspan="2">Поставщик</td>
            <td height="15" align="middle" valign="middle" colspan="4">Потребитель</td>
            <td width="60" height="15" align="middle" valign="middle" rowspan="2">Запас</td>
        </tr>
        <tr>
            <td width="60" height="15" align="middle" valign="middle">B<sub>1</sub> 
            </td>
            <td width="60" height="15" align="middle" valign="middle">B<sub>2</sub> 
            </td>
            <td width="60" height="15" align="middle" valign="middle">B<sub>3</sub> 
            </td>
            <td width="60" height="15" align="middle" valign="middle">B<sub>4</sub> 
            </td>
        </tr>
        <tr>
            <td width="70" height="15" align="middle" valign="middle">A<sub>1</sub> 
            </td>
            <td height="15" bgcolor="e4e4e4" align="middle" valign="middle">1</td>
            <td height="15" bgcolor="e4e4e4" align="middle" valign="middle">7</td>
            <td height="15" bgcolor="e4e4e4" align="middle" valign="middle">9</td>
            <td height="15" bgcolor="e4e4e4" align="middle" valign="middle">5</td>
            <td width="60" height="15" bgcolor="d4d0c8" align="middle" vaslign="middle">120</td>
        </tr>
        <tr>
            <td width="70" height="15" align="middle" valign="middle">A<sub>2</sub></td>
            <td height="15" bgcolor="e4e4e4" align="middle" valign="middle">4</td>
            <td height="15" bgcolor="e4e4e4" align="middle" valign="middle">2</td>
            <td height="15" bgcolor="e4e4e4" align="middle" valign="middle">6</td>
            <td height="15" bgcolor="e4e4e4" align="middle" valign="middle">7</td>
            <td width="60" height="15" bgcolor="d4d0c8" align="middle" valign="middle">280</td>
        </tr>
        <tr>
            <td width="70" height="15" align="middle" valign="middle">A<sub>3</sub> 
            </td>
            <td height="15" bgcolor="e4e4e4" align="middle" valign="middle">2</td>
            <td height="15" bgcolor="e44e4" align="middle" valign="middle">8</td>
            <td height="15" bgcolor="e4e4e4" align="middle" valign="middle">1</td>
            <td height="15" bgcolor="e4e4e4" align="middle" valign="middle">2</td>
            <td width="60" height="15" bgcolor="d4d0c8" align="middle" valign="middle">160</td>
        </tr>
        <tr>
            <td height="15" align="middle" valign="middle">Потребность</td>
            <td height="15" align="middle" bgcolor="d4d0c8" valign="middle">130</td>
            <td height="15" align="middle" bgcolor="d4d0c8" valign="middle">220</td>
            <td height="15" align="middle" bgcolor="d4d0c8" valign="middle">60</td>
            <td height="15" align="middle" bgcolor="d4d0c8" valign="middle">70</td>
        </tr>
    </tbody>
</table>


Суммарные запасы продукции у поставщиков должны равняться суммарной потребности потребителей.

Разница в 80 единиц продукции.
Введем в рассмотрение фиктивного потребителя B<sub>5</sub>, с потребностью 80 единиц продукции.

Стоимость доставки единицы продукции от всех поставщиков к потребителю B<sub>5</sub> примем равной нулю.

Откуда | Кому | Сколько
--- | --- | --- | ---
A<sub>1</sub> | B<sub>1</sub> | min = { 120 , 130 } = 120
A<sub>2</sub> | B<sub>1</sub> | min = { 280 , 10 } = 10
A<sub>2</sub> | B<sub>2</sub> | min = { 270 , 220 } = 220
A<sub>2</sub> | B<sub>3</sub> | min = { 50 , 60 } = 50
A<sub>3</sub> | B<sub>3</sub> | min = { 160 , 10 } = 10
A<sub>3</sub> | B<sub>4</sub> | min = { 150 , 70 } = 70
A<sub>3</sub> | B<sub>5</sub> | 80

<table>
    <tbody>
        <tr>
            <td width="80" align="center" valign="middle" rowspan="2">Поставщик</td>
            <td align="center" valign="middle" colspan="5">Потребитель</td>
            <td width="60" align="center" valign="middle" rowspan="2">Запас</td>
        </tr>
        <tr>
            <td align="center" valign="middle">B <sub>1</sub> 
            </td>
            <td align="center" valign="middle">B <sub>2</sub> 
            </td>
            <td align="center" valign="middle">B <sub>3</sub> 
            </td>
            <td align="center" valign="middle">B <sub>4</sub> 
            </td>
            <td align="center" valign="middle">B <sub>5</sub> 
            </td>
        </tr>
        <tr>
            <td align="center" valign="middle">A <sub>1</sub> 
            </td>
            <td align="center" valign="middle">
               <strong> 120</strong>         
            </td>
            <td align="center" valign="middle">  
            </td>
            <td align="center" valign="middle">
            </td>
            <td align="center" valign="middle">
            </td>
            <td align="center" valign="middle">
            </td>
            <td width="60" align="center" valign="middle">&nbsp; 0</td>
        </tr>
        <tr>
            <td align="center" valign="middle">A <sub>2</sub> 
            </td>
            <td align="center" valign="middle">
                <strong> 10</strong> 
            </td>
            <td align="center" valign="middle">
                <strong> 220</strong> 
            </td>
            <td align="center" valign="middle">
                <strong> 50</strong> 
            </td>
            <td align="center" valign="middle">
            </td>
            <td align="center" valign="middle">
            </td>
            <td width="60" align="center" valign="middle">&nbsp; 0</td>
        </tr>
        <tr>
            <td align="center" valign="middle">A <sub>3</sub> 
            </td>
            <td align="center" valign="middle">
            </td>
            <td align="center" valign="middle">
            </td>
            <td align="center" valign="middle">
                <strong> 10</strong>
            </td>
            <td align="center" valign="middle">
                <strong> 70</strong>
            </td>
            <td align="center" valign="middle">
                <strong> 80</strong> 
            </td>
            <td width="60" align="center" valign="middle">&nbsp; 0</td>
        </tr>
        <tr>
            <td height="25" align="center" valign="middle">Потребность</td>
            <td>0</td>
            <td>0</td>
            <td>0</td>
            <td>0</td>
            <td>0</td>
        </tr>
    </tbody>
</table>

Стоимость доставки продукции, для начального решения, не сложно посчитать.
S = 120 * 1 + 10 * 4 + 220 * 2 + 50 * 6 + 10 * 1 + 70 * 2 + 80 * 0 = 1050 ден. ед.

Чтобы проверить, является ли решение оптимальным, количество задействованных маршрутов должно быть не больше (rows + col - 1) = 5 + 3 - 1 = 7 :+1: 

### Метод потенциалов

Найдем потенциалы поставщиков и покупателей:

* Для задействованного маршрута, сумма потенциала поставщика и потребителя равна тарифу задействованного маршрута.
* Оценка незадействованного маршрута = тариф маршрута - ( потенциал поставщика + потенциал потребителя ).


#### Шаг 1

<table border="0" cellpadding="3" cellspacing="0" class="body_txt">
    <tbody>
        <tr>
            <td colspan="3">Потенциалы задействованных маршрутов</td>
        </tr>
        <tr>
            <td>A<sub>3</sub>B<sub>3</sub> : &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>3</sub> + u<sub>3</sub> = 1 &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>3</sub> = 1 - 0 = 1</td>
        </tr>
        <tr>
            <td>A<sub>3</sub>B<sub>4</sub> : &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>4</sub> + u<sub>3</sub> = 2 &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>4</sub> = 2 - 0 = 2</td>
        </tr>
        <tr>
            <td>A<sub>3</sub>B<sub>5</sub> : &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>5</sub> + u<sub>3</sub> = 0 &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>5</sub> = 0 - 0 = 0</td>
        </tr>
        <tr>
            <td>A<sub>2</sub>B<sub>3</sub> : &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>3</sub> + u<sub>2</sub> = 6 &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; u<sub>2</sub> = 6 - 1 = 5</td>
        </tr>
        <tr>
            <td>A<sub>2</sub>B<sub>1</sub> : &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>1</sub> + u<sub>2</sub> = 4 &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>1</sub> = 4 - 5 = -1</td>
        </tr>
        <tr>
            <td>A<sub>2</sub>B<sub>2</sub> : &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>2</sub> + u<sub>2</sub> = 2 &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>2</sub> = 2 - 5 = -3</td>
        </tr>
        <tr>
            <td>A<sub>1</sub>B<sub>1</sub> : &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>1</sub> + u<sub>1</sub> = 1 &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; u<sub>1</sub> = 1 - ( -1 ) = 2</td>
        </tr>
    </tbody>
</table>


<table border="0" cellpadding="3" cellspacing="0" class="body_txt">
    <tbody>
        <tr>
            <td colspan="3">Потенциалы незадействованных маршрутов</td>
        </tr>
        <tr>
            <td>A<sub>1</sub>B<sub>2</sub>
            </td>
            <td>&Delta;<sub>1</sub><sub>2</sub> = 7 - ( 2 + ( -3 ) ) = 8</td>
        </tr>
        <tr>
            <td>A<sub>1</sub>B<sub>3</sub>
            </td>
            <td>&Delta;<sub>1</sub><sub>3</sub> = 9 - ( 2 + 1 ) = 6</td>
        </tr>
        <tr>
            <td>A<sub>1</sub>B<sub>5</sub>
            </td>
            <td>&Delta;<sub>1</sub><sub>5</sub> = 0 - ( 2 + 0 ) = -2</td>
        </tr>
        <tr>
            <td>A<sub>2</sub>B<sub>4</sub>
            </td>
            <td>&Delta;<sub>2</sub><sub>4</sub> = 7 - ( 5 + 2 ) = 0</td>
        </tr>
        <tr>
            <td>A<sub>2</sub>B<sub>5</sub>
            </td>
            <td>&Delta;<sub>2</sub><sub>5</sub> = 0 - ( 5 + 0 ) = -5</td>
        </tr>
        <tr>
            <td>A<sub>3</sub>B<sub>1</sub>
            </td>
            <td>&Delta;<sub>3</sub><sub>1</sub> = 2 - ( 0 + ( -1 ) ) = 3</td>
        </tr>
        <tr>
            <td>A<sub>3</sub>B<sub>2</sub>
            </td>
            <td>&Delta;<sub>3</sub><sub>2</sub> = 8 - ( 0 + ( -3 ) ) = 11</td>
        </tr>
    </tbody>
</table>

Здесь два незадействованных маршрута с отрицательными потенциалами. A<sub>1</sub>B<sub>5</sub> и A<sub>2</sub>B<sub>5</sub>

Задействуем A<sub>2</sub>B<sub>5</sub>

Пусть ячейка A<sub>2</sub>B<sub>5</sub>, для которой мы строили цикл, имеет порядковый номер один.
Среди ячеек цикла, номера которых четные, найдем ячейку обладающую наименьшим значением.
min = { 50, 80 } = 50.

От ячеек цикла с четными номерами отнимает 50. К ячейкам с нечетными номерами прибавляем 50.

<table>
    <tbody>
        <tr>
            <td width="80" align="center" valign="middle" rowspan="2">Поставщик</td>
            <td align="center" valign="middle" colspan="5">Потребитель</td>
            <td width="60" align="center" valign="middle" rowspan="2">Запас</td>
        </tr>
        <tr>
            <td align="center" valign="middle">B <sub>1</sub> 
            </td>
            <td align="center" valign="middle">B <sub>2</sub> 
            </td>
            <td align="center" valign="middle">B <sub>3</sub> 
            </td>
            <td align="center" valign="middle">B <sub>4</sub> 
            </td>
            <td align="center" valign="middle">B <sub>5</sub> 
            </td>
        </tr>
        <tr>
            <td align="center" valign="middle">A <sub>1</sub> 
            </td>
            <td align="center" valign="middle">
              120       
            </td>
            <td align="center" valign="middle">  
            </td>
            <td align="center" valign="middle">
            </td>
            <td align="center" valign="middle">
            </td>
            <td align="center" valign="middle">
            </td>
            <td width="60" align="center" valign="middle">&nbsp; 0</td>
        </tr>
        <tr>
            <td align="center" valign="middle">A <sub>2</sub> 
            </td>
            <td align="center" valign="middle">
                10
            </td>
            <td align="center" valign="middle">
                220
            </td>
            <td align="center" valign="middle">
                <strong>0</strong> 
            </td>
            <td align="center" valign="middle">
            </td>
            <td align="center" valign="middle">
                <strong>50</strong> 
            </td>
            <td width="60" align="center" valign="middle">&nbsp; 0</td>
        </tr>
        <tr>
            <td align="center" valign="middle">A <sub>3</sub> 
            </td>
            <td align="center" valign="middle">
            </td>
            <td align="center" valign="middle">
            </td>
            <td align="center" valign="middle">
                <strong> 60</strong>
            </td>
            <td align="center" valign="middle">
                70
            </td>
            <td align="center" valign="middle">
                <strong> 30</strong> 
            </td>
            <td width="60" align="center" valign="middle">&nbsp; 0</td>
        </tr>
        <tr>
            <td height="25" align="center" valign="middle">Потребность</td>
            <td>0</td>
            <td>0</td>
            <td>0</td>
            <td>0</td>
            <td>0</td>
        </tr>
    </tbody>
</table>

S = 1050 + &Delta;<sub>25</sub> * 50 = 1050 - 5 * 50 = 800 ден. ед.

#### Шаг 2

<table border="0" cellpadding="3" cellspacing="0" class="body_txt">
    <tbody>
        <tr>
            <td colspan="3">Потенциалы задействованных маршрутов</td>
        </tr>
        <tr>
            <td>A<sub>3</sub>B<sub>3</sub> : &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>3</sub> + u<sub>3</sub> = 1 &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>3</sub> = 1 - 0 = 1</td>
        </tr>
        <tr>
            <td>A<sub>3</sub>B<sub>4</sub> : &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>4</sub> + u<sub>3</sub> = 2 &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>4</sub> = 2 - 0 = 2</td>
        </tr>
        <tr>
            <td>A<sub>3</sub>B<sub>5</sub> : &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>5</sub> + u<sub>3</sub> = 0 &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>5</sub> = 0 - 0 = 0</td>
        </tr>
        <tr>
            <td>A<sub>2</sub>B<sub>5</sub> : &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>5</sub> + u<sub>2</sub> = 0 &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; u<sub>2</sub> = 0 - 0 = 0</td>
        </tr>
        <tr>
            <td>A<sub>2</sub>B<sub>1</sub> : &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>1</sub> + u<sub>2</sub> = 4 &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>1</sub> = 4 - 0 = 4</td>
        </tr>
        <tr>
            <td>A<sub>2</sub>B<sub>2</sub> : &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>2</sub> + u<sub>2</sub> = 2 &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>2</sub> = 2 - 0 = 2</td>
        </tr>
        <tr>
            <td>A<sub>1</sub>B<sub>1</sub> : &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; v<sub>1</sub> + u<sub>1</sub> = 1 &nbsp; &nbsp;</td>
            <td align="left">&nbsp; &nbsp; u<sub>1</sub> = 1 - 4 = -3</td>
        </tr>
    </tbody>
</table>

<table border="0" cellpadding="3" cellspacing="0" class="body_txt">
    <tbody>
        <tr>
            <td colspan="3">Потенциалы незадействованных маршрутов</td>
        </tr>
        <tr><td>A<sub>1</sub>B<sub>2</sub></td><td>&Delta;<sub>1</sub><sub>2</sub>  = 7 - ( -3 + 2 )  = 8</td></tr>
        <tr><td>A<sub>1</sub>B<sub>3</sub></td><td>&Delta;<sub>1</sub><sub>3</sub>  = 9 - ( -3 + 1 )  = 11</td></tr>
        <tr><td>A<sub>1</sub>B<sub>4</sub></td><td>&Delta;<sub>1</sub><sub>4</sub>  = 5 - ( -3 + 2 )  = 6</td></tr>
        <tr><td>A<sub>1</sub>B<sub>5</sub></td><td>&Delta;<sub>1</sub><sub>5</sub>  = 0 - ( -3 + 0 )  = 3</td></tr>
        <tr><td>A<sub>1</sub>B<sub>5</sub></td><td>&Delta;<sub>1</sub><sub>5</sub>  = 0 - ( -3 + 0 )  = 3</td></tr>
        <tr><td>A<sub>2</sub>B<sub>4</sub></td><td>&Delta;<sub>2</sub><sub>4</sub>  = 7 - ( 0 + 2 )  = 5</td></tr>
        <tr><td>A<sub>3</sub>B<sub>1</sub></td><td>&Delta;<sub>3</sub><sub>1</sub>  = 2 - ( 0 + 4 )  = -2</td></tr>
        <tr><td>A<sub>3</sub>B<sub>2</sub></td><td>&Delta;<sub>3</sub><sub>2</sub>  = 8 - ( 0 + 2 )  = 6</td></tr>
    </tbody>
</table>

Здесь только один незадействованный маршрут с отрицательным потенциалом - A<sub>3</sub>B<sub>1</sub>

<table>
    <tbody>
        <tr>
            <td width="80" align="center" valign="middle" rowspan="2">Поставщик</td>
            <td align="center" valign="middle" colspan="5">Потребитель</td>
            <td width="60" align="center" valign="middle" rowspan="2">Запас</td>
        </tr>
        <tr>
            <td align="center" valign="middle">B <sub>1</sub> 
            </td>
            <td align="center" valign="middle">B <sub>2</sub> 
            </td>
            <td align="center" valign="middle">B <sub>3</sub> 
            </td>
            <td align="center" valign="middle">B <sub>4</sub> 
            </td>
            <td align="center" valign="middle">B <sub>5</sub> 
            </td>
        </tr>
        <tr>
            <td align="center" valign="middle">A <sub>1</sub> 
            </td>
            <td align="center" valign="middle">
              120       
            </td>
            <td align="center" valign="middle">  
            </td>
            <td align="center" valign="middle">
            </td>
            <td align="center" valign="middle">
            </td>
            <td align="center" valign="middle">
            </td>
            <td width="60" align="center" valign="middle">&nbsp; 0</td>
        </tr>
        <tr>
            <td align="center" valign="middle">A <sub>2</sub> 
            </td>
            <td align="center" valign="middle">
                <strong>0</strong> 
            </td>
            <td align="center" valign="middle">
                220
            </td>
            <td align="center" valign="middle">
                
            </td>
            <td align="center" valign="middle">
            </td>
            <td align="center" valign="middle">
                <strong>60</strong> 
            </td>
            <td width="60" align="center" valign="middle">&nbsp; 0</td>
        </tr>
        <tr>
            <td align="center" valign="middle">A <sub>3</sub> 
            </td>
            <td align="center" valign="middle">
            <strong>10</strong> 
            </td>
            <td align="center" valign="middle">
            </td>
            <td align="center" valign="middle">
                60
            </td>
            <td align="center" valign="middle">
                70
            </td>
            <td align="center" valign="middle">
                <strong> 20</strong> 
            </td>
            <td width="60" align="center" valign="middle">&nbsp; 0</td>
        </tr>
        <tr>
            <td height="25" align="center" valign="middle">Потребность</td>
            <td>0</td>
            <td>0</td>
            <td>0</td>
            <td>0</td>
            <td>0</td>
        </tr>
    </tbody>
</table>

S = 800 + &Delta;<sub>31</sub> * 10 = 800 - 2 * 10 = 780 ден. ед.

#### Шаг 3

Тут потенциалы всех незадействованных маршрутов неотрицательны.

### Ответ

<table>
    <tbody>
        <tr>
            <td width="80" align="center" valign="middle" rowspan="2">Поставщик</td>
            <td align="center" valign="middle" colspan="5">Потребитель</td>
            
        </tr>
        <tr>
            <td align="center" valign="middle">B <sub>1</sub> 
            </td>
            <td align="center" valign="middle">B <sub>2</sub> 
            </td>
            <td align="center" valign="middle">B <sub>3</sub> 
            </td>
            <td align="center" valign="middle">B <sub>4</sub> 
            </td>
            <td align="center" valign="middle">B <sub>5</sub> 
            </td>
        </tr>
        <tr>
            <td align="center" valign="middle">A <sub>1</sub> 
            </td>
            <td align="center" valign="middle">
              120       
            </td>
            <td align="center" valign="middle">  
            </td>
            <td align="center" valign="middle">
            </td>
            <td align="center" valign="middle">
            </td>
            <td align="center" valign="middle">
            </td>
            
        </tr>
        <tr>
            <td align="center" valign="middle">A <sub>2</sub> 
            </td>
            <td align="center" valign="middle">
                
            </td>
            <td align="center" valign="middle">
                220
            </td>
            <td align="center" valign="middle">
                
            </td>
            <td align="center" valign="middle">
            </td>
            <td align="center" valign="middle">
               60
            </td>
           
        </tr>
        <tr>
            <td align="center" valign="middle">A <sub>3</sub> 
            </td>
            <td align="center" valign="middle">
            10
            </td>
            <td align="center" valign="middle">
            </td>
            <td align="center" valign="middle">
                60
            </td>
            <td align="center" valign="middle">
                70
            </td>
            <td align="center" valign="middle">
                20
            </td>
            
        </tr>
        
    </tbody>
</table>

#### S = 780 ден. ед.

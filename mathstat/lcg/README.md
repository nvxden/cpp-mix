# Линейный конгруэнтный метод

Линейный конгруэнтный метод (linear congruential generator) — один
из простейших, но в то же время эффективный и поэтому
частоупотребимый метод при генерации последовательности случайных
чисел. Каждое следующее число расчитывается по формуле:

`R' = mod(k∙R + b, M)`

где

- `M` — модуль 
- `k` — множитель: 
- `b` — приращение: 

Последовательность чисел, полученная с помощью данной формулы,
называется линейной конгруэнтной последовательностью.

Чтобы генератор был качественным, необходимо правильно подобрать
параметры. За  часто берут наибольшее простое число меньшее (для
таких чисел доказывается, что младшие разряды числа  ведут себя так
же случайно, как и старшие), например, число Мерсенна, равное .
Одним из требований к линейной конгруэнтной последовательности
является как можно большая длина периода, т.е. количество чисел,
через которое последовательность начинает повторяться. С этим
требованием связана одна теорема.

***Теорема.*** Линейная конгруэнтная последовательность имеет период
длинной  тогда и только тогда, когда:

1. Числа `b` и `M` взаимно простые
2. `k-1` кратно `p` для каждого `p`, являющегося простым делителем `M`
3. Если `M` кратно 4, то и `k-1` кратно 4

Примечание. Если `M` простое, то `k-1` должно быть кратно в том числе
и самому `M`.
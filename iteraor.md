유폭 보고서
-----------------

1. iterater란?
-next()라는 함수가 사용될 수 있으면 iterater이다.
-next()를 사용하여 출력할 때, 다음 출력 데이터가 없으면 StopIteration exception을 발생시킨다.
-파이썬의 내장함수 iter()를 이용해 iterator 객체를 만든다.
2. iterator 예제
--1-

>>> list = [1,2,3]

>>> it = iter(list)

>>> next(it)
1

>>> next(it)
  2

>>> next(it)
  3

--2-

>>> list = range(1,10)

>>> it = iter(list)

>>> next(it)
  1

>>> next(it)
  2

>>> next(it)
  3

>>> next(it)
  4

>>> next(it)
  5


--3-

>>> list = range(1,10)

>>> it = iter(list)

>>> for i in range(1,10):
  ...     next(it)
  ...
  1
  2
  3
  4
  5
  6
  7
  8
  9

--4-

>>> list  = {'a':1,'b':2,'c':3}

>>> it  = iter(list)

>>> next(it)
  'a'

>>> next(it)
  'b'

>>> next(it)
  'c'

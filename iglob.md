유폭 보고서
-----------------

1. iglob란?
    -재귀적으로 현재 폴더의 모든 하위폴더까지 탐색하여 선택한 확장자 파일을 출력한다.
2. iglob 예제

-1-

    C:\Users\hrths>cd C:\유폭 땜에 만든거
    C:\유폭 땜에 만든거>py
    Python 3.7.0 (v3.7.0:1bf9cc5093, Jun 27 2018, 04:06:47) [MSC v.1914 32 bit (Intel)] on win32
    Type "help", "copyright", "credits" or "license" for more information.
    >>> import glob
    >>> for file in glob.glob('*.*'):
    ...     print(file)
    ...
    유폭1.txt
  
-2-

    C:\Users\hrths>cd C:\유폭 땜에 만든거
    C:\유폭 땜에 만든거>py
    Python 3.7.0 (v3.7.0:1bf9cc5093, Jun 27 2018, 04:06:47) [MSC v.1914 32 bit (Intel)] on win32
    Type "help", "copyright", "credits" or "license" for more information.
    >>> import glob
    >>> for file in glob.iglob('**/*.txt'):
    ...     print(file)
    ...
    유폭땜에 만든거 2\유폭 2.txt

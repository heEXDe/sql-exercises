# Some SQL exercises solved by me
## From CodeWars
***
exercise: https://www.codewars.com/kata/53da3dbb4a5168369a0000fe/train/sql
```
SELECT number, CASE WHEN (number % 2) = 0 THEN 'Even' ELSE 'Odd' END AS is_even
FROM numbers;
```
***
exercise: https://www.codewars.com/kata/56dec885c54a926dcd001095
```
select (number * -1) as "res"
from opposite;
```
***
exercise: https://www.codewars.com/kata/53369039d7ab3ac506000467/sql
```
select bool, CASE WHEN bool = true THEN 'Yes' ELSE 'No' END AS res
from booltoword;
```
***
exercise: https://www.codewars.com/kata/57a0e5c372292dd76d000d7e/sql
```
select s, n, repeat(s, n) as "res"
from repeatstr;
```
***
exercise: https://www.codewars.com/kata/56bc28ad5bdaeb48760009b0
```
SELECT s, (SUBSTRING(s, 2, LENGTH(s) - 2)) AS res
FROM removechar;
```
***
exercise: https://www.codewars.com/kata/55d24f55d7dd296eb9000030
```
select n, (n * (1+n)/2) as res
from kata;
```
***
exercise: https://www.codewars.com/kata/57eae20f5500ad98e50002c5
```
select x, replace(x, ' ', '') as res from nospace;
```
***
exercise: https://www.codewars.com/kata/55a70521798b14d4750000a4
```
select format('Hello, %s how are you doing today?', name) as greeting 
from person;
```
***
exercise: https://www.codewars.com/kata/582cb0224e56e068d800003c
```
SELECT *, FLOOR(hours * 0.5) as liters FROM cycling;
```
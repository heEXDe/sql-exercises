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
exercise: https://www.codewars.com/kata/53369039d7ab3ac506000467/sql
```
select bool, CASE WHEN bool = true THEN 'Yes' ELSE 'No' END AS res
from booltoword;
```
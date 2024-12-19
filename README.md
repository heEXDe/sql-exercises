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
***
exercise: https://www.codewars.com/kata/5a3fe3dde1ce0e8ed6000097
```
SELECT (
CASE 
WHEN yr % 100 > 0 THEN yr / 100 + 1 
WHEN yr % 100 = 0 THEN yr / 100 
END  
) AS century 
FROM years;
```
***
exercise: https://www.codewars.com/kata/555086d53eac039a2a000083
```
select flower1, flower2, (
case
  when (flower1 % 2 = 0 and flower2 % 2 = 1) then true
  when (flower2 % 2 = 0 and flower1 % 2 = 1) then true
  else false
  end
) as res
from love;
```
***
exercise: https://www.codewars.com/kata/55f9b48403f6b87a7c0000bd
```
SELECT n, m, (
CASE
 WHEN n<0 OR m<0 THEN 0
 ELSE n * m
END
) as res
FROM paperwork;
```
exercise: https://www.codewars.com/kata/55f9bca8ecaa9eac7100004a
```
SELECT (h * 60 * 60 * 1000 + m * 60 * 1000 + s * 1000) AS res FROM past;
```
***
exercise: https://www.codewars.com/kata/57a0556c7cb1f31ab3000ad7
```
SELECT s, UPPER(s) AS res
FROM makeuppercase; 
```
***
exercise: https://www.codewars.com/kata/583710ccaa6717322c000105
```
select number, (
case
  when number % 2 = 0 then number * 8
  else number * 9
  end
) as res 
from multiplication;
```
exercise: https://www.codewars.com/kata/57eae65a4321032ce000002d
```
SELECT x, (REGEXP_REPLACE(REGEXP_REPLACE(x, '[0-4]', '0', 'g'), '[5-9]', '1', 'g')) AS res
FROM fakebin;
```
***
exercise: https://www.codewars.com/kata/5861d28f124b35723e00005e
```
SELECT 
        distance_to_pump,
        mpg,
        fuel_left,
        CASE WHEN(distance_to_pump - (mpg * fuel_left)) <= 0 THEN true
        ELSE false END AS res
FROM zerofuel;
```
***
exercise: https://www.codewars.com/kata/5513795bd3fafb56c200049e
```
select x, n, (
select array_agg(i * x) from generate_series(1, n) i
) as res
from counter
order by x asc, n asc;
```
***
exercise: https://www.codewars.com/kata/5545f109004975ea66000086
```
SELECT id, (
  CASE 
  WHEN n % x = 0 AND n % y = 0 THEN true ELSE false END
) AS res FROM kata;
```
***
exercise: https://www.codewars.com/kata/5ce9c1000bab0b001134f5af/sql
```
SELECT month, (
CASE
WHEN month <= 3 THEN 1 
WHEN month <= 6 THEN 2
WHEN month <= 9 THEN 3
ELSE 4 END
) AS res FROM quarterof;
```
***
exercise: https://www.codewars.com/kata/57a0885cbb9944e24c00008e/sql
```
SELECT s, (REGEXP_REPLACE(s, '!', '', 'g')) AS res FROM removeexclamationmarks;
```
***
exercise: https://www.codewars.com/kata/5a023c426975981341000014
```
select a, b, (180 - a - b) as res from otherangle;
```
***
exercise: https://www.codewars.com/kata/55f73be6e12baaa5900000d4
```
SELECT (la_liga_goals + copa_del_rey_goals + champions_league_goals) AS res FROM goals;
```
***
exercise: https://www.codewars.com/kata/55cbc3586671f6aa070000fb
```
SELECT id, (
CASE 
  WHEN base % factor = 0 THEN true ELSE false 
  END
) AS res FROM kata;
```
***
exercise: https://www.codewars.com/kata/523b623152af8a30c6000027
```
SELECT n, CAST(POWER(n, 2) AS INTEGER) AS res FROM square;
```
***
exercise: https://www.codewars.com/kata/54ff3102c1bad923760001f3
```
SELECT 
    str,
    CHAR_LENGTH(REGEXP_REPLACE(str, '[^aeiou]', '', 'g')) AS res
FROM 
    getcount;
```
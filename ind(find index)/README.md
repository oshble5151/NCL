# ind

ind함수를 사용해서, index를 찾을 수 있다.

```ncl

arr =(/0,2,4,6,8/)
ind_4 = ind(arr .eq. 4)
print(ind_4)

Variable: ind_4
Type: integer
Total Size: 4 bytes
            1 values
Number of Dimensions: 1
Dimensions and sizes:   [1]
Coordinates:
(0)     2
```

배열에 있는 요소의 index를 출력해준다.

## .ep
eq는 배열 사용 가능하다.
뒤의 숫자가 맞는지 판별한뒤 bool 배열을 돌려준다.
```ncl
arr = (/1,2,3,4,5/)

test = arr.eq.3
print(test)
Type: logical
Total Size: 20 bytes
            5 values
Number of Dimensions: 1
Dimensions and sizes:   [5]
Coordinates:
(0)     False
(1)     False
(2)     True
(3)     False
(4)     False
```

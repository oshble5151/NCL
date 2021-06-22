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

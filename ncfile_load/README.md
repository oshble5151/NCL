![image](https://user-images.githubusercontent.com/73323188/122921614-a49cd580-d39d-11eb-822d-1a05976fdbad.png)


# &로file에서 dimention 추출하기
```ncl

file -> addfile('atmos_month_1981.nc', "r")
print(file&time)

Variable: time (coordinate)
Type: double
Total Size: 96 bytes
            12 values
Number of Dimensions: 1
Dimensions and sizes:   [time | 12]
Coordinates:
Number Of Attributes: 6
  long_name :   time
  units :       days since 1850-01-01 00:00:00
  cartesian_axis :      T
  calendar_type :       JULIAN
  calendar :    JULIAN
  bounds :      time_bounds
(0)     47863.5
(1)     47893
(2)     47922.5
(3)     47953
(4)     47983.5
(5)     48014
(6)     48044.5
(7)     48075.5
(8)     48106
(9)     48136.5
(10)    48167
(11)    48197.5
```

# 배열 indexing

ncl은 python과 indexing 방법에 약간의 차이가 있다.

바로 index1:index2로 적으면 index(순서)로 indexing 되지만, 중괄호{:}로 indexing하면 값을 기준으로 indexing한다.

```ncl
file = addfile("atmos_month_1981.nc", "r")

tas(0:5,{-10:10},:) ; time 5개 축, 위도 -10~10 범위, 전 경도 범위가 indexing됨 
```




ncl과 python은 문법이 비슷하다.

다음은 ncl과 python의 차이를 나타낸다.

출처(https://www.ncl.ucar.edu/Document/Manuals/NCL_to_Python/)

![image](https://user-images.githubusercontent.com/73323188/122519015-ed2a5b00-d04c-11eb-933f-01b7528ede42.png)

![image](https://user-images.githubusercontent.com/73323188/122519136-14812800-d04d-11eb-868e-a7f6f638cbc6.png)

![image](https://user-images.githubusercontent.com/73323188/122519242-337fba00-d04d-11eb-8dde-64c1729b4e79.png)

![image](https://user-images.githubusercontent.com/73323188/122519792-d0daee00-d04d-11eb-9f71-76087ce5a03c.png)

#### *ncl에서 이미 지정한 변수를 사용할때 $변수명$과 같이 사용해야함 
```ncl
f = addfile("atmos_month_1981.nc","r")

var_lcc = "low_cld_amt"
lcc = f->$var_lcc$
print(lcc)
Variable: lcc
Type: float
Total Size: 622080 bytes
            155520 values
Number of Dimensions: 3
Dimensions and sizes:   [time | 12] x [grid_yt | 90] x [grid_xt | 144]
Coordinates:
            time: [47863.5..48197.5]
            grid_yt: [-89.49438202247191..89.49438202247191]
            grid_xt: [1.25..358.75]
Number Of Attributes: 7
  long_name :   low cloud amount
  units :       percent
  missing_value :       1e+20
  _FillValue :  1e+20
  cell_methods :        time: mean
  time_avg_info :       average_T1,average_T2,average_DT
  interp_method :       conserve_order1

```

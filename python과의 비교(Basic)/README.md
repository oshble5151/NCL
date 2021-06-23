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
```

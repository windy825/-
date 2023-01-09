# 2차원 x, y 축 좌표계의 회전행렬 구하기

<br>

####  2차원 XY 평면에서 점 P 를 θ 만큼 회전하여 P′ 를 얻을 때 사용하는 행렬 구하기

![image](https://user-images.githubusercontent.com/89068148/196026599-467d2347-73ff-4b74-81e1-6d9fe27c4256.png)

<br>

#### [1] **α 각 정리**

```
sin(α) = y / r
cos(α) = x / r
```

`r을 기준`으로 등식 정리

```
x sin(α) = y cos(α)
```

<br>

#### [2] **α + θ 각 정리**

##### 1) X' 정의

```
x′ = r * cos(θ+α)
```

`cos(θ+α) = cos(θ)cos(α) − sin(θ)sin(α)` 를 이용해서 위의 식 전개

```
rcos(θ+α) = r * ( cos(θ)cos(α) − sin(θ)sin(α) )
          = r * ( cos(θ) * x/r − sin(θ) * y/r )
          = xcos(θ) − ysin(θ)
```

```
∴ x′ = xcos(θ) − ysin(θ)
```

<br>

##### 2) y' 정의

```
y′ = r * sin(θ+α)
```

`sin(θ+α) = sin(θ)cos(α) + cos(θ)sin(α)` 를 이용해서 식 전개

```
∴ y′ = xsin(θ) + ycos(θ)
```

<br>

##### 3) 행렬로 나타내기

![image](https://user-images.githubusercontent.com/89068148/200154937-6f15b4a5-f7f4-4455-b1e1-24ab84f2d3e2.png)





## 3차원 좌표계 축과 회전변환

![제목 없음](https://user-images.githubusercontent.com/89068148/189534461-f5e26cb7-11de-4088-bb53-0eb6086a9257.png)

<br>

<br>

## **Change of 3D coordinates by rotation**

선형변환에서 회전변환행렬은 임의의 행렬을 **원점을 중심으로 회전**시킨다.

특히 좌표계 축은 유지한채로, 좌표점만을 원점에 대해 외전한 행렬을 의미함...

<br>

**3차원 회전행렬은 기존 2차원 회전행렬을 활용한다.  (θ가 양수면 반시계 방향, 음수면 시계 방향)**

![image](https://user-images.githubusercontent.com/89068148/196034209-e6be7d1f-5ffd-4fdf-b3a8-a06ea0c4e811.png)

![image](https://user-images.githubusercontent.com/89068148/200154952-b6c5b71b-e09b-4f26-9e08-7a3dcbc656f8.png)

![image](https://user-images.githubusercontent.com/89068148/200154958-bd72bf62-187f-4de7-98f8-05aa14ed8b21.png)

## **Change of basis by rotation**

이번엔 좌표계의 축 `basis` 가 회전할때 좌표점의 변화를 확인한다.

![image](https://user-images.githubusercontent.com/89068148/196034242-6e600b06-6a0b-423c-b119-0724b5b03fea.png)

위 그림의 행렬 식과 같이 회전 변환 행렬의 역행렬을 곱하면 된다.





---

*참고 : https://gaussian37.github.io/vision-concept-calibration/*

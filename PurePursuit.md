# Pure Pursuit 

#### way_point 에 대한 차량 조향각도는 타겟 원호의 곡률에 비례하도록 해야 함 

![KakaoTalk_20220825_0159sdsdsd56816](https://user-images.githubusercontent.com/89068148/186479180-860f07ae-e57f-4d9f-9020-378981c0201d.jpg)

여기서 그럼 r을 구하려면,

![KakaoTalk_20220825_015956816](https://user-images.githubusercontent.com/89068148/186479341-4c582ea2-52e0-4c5a-8262-ba66b1b1060a.jpg)

Steering angles should be propotional to the curvature of the arc (**원호의 곡률에 비례**하도록 만들자)

```
알파 = 1 / r = 2*|gy| / L**2
```



## 적용은 어떤 방식으로 도출하나??

![CamScanner 08-25-2022 02 21_1](https://user-images.githubusercontent.com/89068148/186485214-648d5f12-ef96-4051-9c7c-0c69f5e5aaf1.jpg)



## 차량의 조향각 계산 하는 방법 ??

![CamScanner 08-25-2022 02 28_1](https://user-images.githubusercontent.com/89068148/186485362-79357085-76a4-4126-a406-b373bde2db18.jpg)

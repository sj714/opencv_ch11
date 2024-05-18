실습과제1

구조요소행렬의 3가지 종류(MORPH_RECT, MORPH_CROSS, MORPH_ELLIPSE)를 getStructuringElement() 함수를 
이용하여 구하고 다음과 같이 출력

![KakaoTalk_20240518_224930164](https://github.com/sj714/opencv_ch11/assets/169256660/b1950ced-314d-4a75-8e35-323b52352cbd)

실습과제2

원본영상(letterj.png)을 이진화

이진화된 영상을 모폴로지연산 이용하여 노이즈 제거

평균값 필터는 단순한 평균으로 잡음을 제거하지만, 에지를 흐리게 만들고 세부 사항을 잃을 수 있습니다. 반면 가우시안 필터는 가중치를 적용하여 잡음을 더 자연스럽게 제거하며, 에지를 덜 흐리게 만드는 장점이 있습니다.

![KakaoTalk_20240518_224959459](https://github.com/sj714/opencv_ch11/assets/169256660/43e53703-9468-441c-9057-e0efe40c4e03)

실습과제3

원본영상(letterj2.png)을 이진화

이진화된 영상을 침식 또는 팽창 연산을 이용하여 에지를 구함

![KakaoTalk_20240518_225030781](https://github.com/sj714/opencv_ch11/assets/169256660/9b0ec465-36bc-4f72-9e82-39687edcd241)

실습과제4

원본영상(car.jpg)을 그레이로 변환

그레이 영상에서 블러링 적용하고, sobel 함수 이용하여 수직방향의 에지만 검출

에지 검출된 영상을 이진화하고, 닫기연산 수행

닫기연산시 구조요소행렬의 사이즈는 5행 32열로 가로방향으로 긴 사각형 형태의 마스크를 이용하여 숫자들을 하나의 객체로 합쳐준다.

![KakaoTalk_20240518_225112682](https://github.com/sj714/opencv_ch11/assets/169256660/a9eb7a75-da5e-43c4-bff9-6b4edc1d3ad4)


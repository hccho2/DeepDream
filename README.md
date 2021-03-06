# DeepDream, Inception V1, Tensorflow 2.x
<a href="https://drive.google.com/uc?export=view&id=11_Oe9DQE3sHSxaT2Ac7QYjEnHlcfgJsE"><img src="https://drive.google.com/uc?export=view&id=11_Oe9DQE3sHSxaT2Ac7QYjEnHlcfgJsE" style="width: 650px; max-width: 100%; height: auto" title="Deep Dream Zoom" />


## 왜 Inception V1인가?

- Inception V1 model를 이용하여 이미지 생성
    * [Tensorflow Tutorial](https://www.tensorflow.org/tutorials/generative/deepdream?hl=ko)의 Deep Dream에서는 Inception V3 모델을 사용하고 있고, 제가 본 몇몇 책에서도 Inception V3를 사용.
    * Inception V3로 이미지를 생성하면, 멋진(?) 이미지가 잘 안 나옴. 아래 그림을 보면, 뭔가 좀 부족해 보인다.
    ![img7](./img7_v3.png)
    
    * Inception V1이 Inception V3보다 더 다양한 이미지를 잘 만듬.
   ![img8](./img8_v1.png)
    * 그런데, Inception V1의 pre-trained weight는 proto buffer(pb)파일이라, tensorflow 2.x에서 사용하기 위해서는 추가 작업이 필요.

# jupyte Notebook에 구현된 내용들
- tensorflow 1.x로 train된 proto buffer(pb) 파일을 다운받은 후, tensorflow 2.x에서 로드.
- ipywidget을 이용하여, 편리하게 parameter 변경
   ![img9](./ipywidget.png)
- zooming 효과로 이미지 생성
- animated git 생성
- 구현코드는 jupyte notebook [파일](https://github.com/hccho2/DeepDream/blob/main/deemdream_InceptionV1_TF2.ipynb).  --> google colab에서 작성했습니다.

## Deep Dream 생성 이미지

![img5](./img5.png)

![img1](./img1.png)
![img6](./img6.jpg)
![img2](./img2.png)

![img3](./img3.jpg)

![img4](./img4.jpg)

# findname
은행 적요에 들어있는 인명찾기
> 은행사람들이 사람이름도 개인정보라고 해서 적요데이터를 함부로 주지 않는다. <br>그래서 우리가 직접 사람이름을 마스킹 처리해야 하는데 일일히 하면 시간이 너무 오래걸린다. <br>이를 lstm 기반의 딥러닝 기법을 이용해서 사람이름을 학습하고 분류하여 자동으로 찾아내도록 한다. 

![](./path/to/image.png)

<br>
<br>

## requirments
``` cmd
jupyter
tensorflow-gpu == 2.10.0
pandas == 1.2.4
keras == 2.10.0
tqdm == 4.61.0
```
<br>
<br>

## 사용방법
1. 쥬피터 노트북 접속 
``` cmd
$ jupyter notebook
```
2. data.ipynb 로 데이터셋 생성<br>
데이터셋은 ```data/``` 폴더에 생성된다.

3. train.ipynb로 학습<br>
마지막에 있는 성가지표로 학습성능을 확인한다.

4. inference.ipynb로 추론(테스트)<br>
여기서 추론용 데이터는 본인의 은행거래 데이터를 사용해서 확인해보자.

<br>
<br>

## 정보
최승언 – [@velog](https://velog.io/@csu5216) – su.choi@niccompany.co.kr

라이센스: 원본 코드의 라이센스 또는 본인이 작성


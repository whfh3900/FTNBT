# FTNBT
은행 적요에 들어있는 인명찾기
> 은행사람들이 사람이름도 개인정보라고 해서 적요데이터를 함부로 주지 않는다. <br>그래서 우리가 직접 사람이름을 마스킹 처리해야 하는데 일일히 하면 시간이 너무 오래걸린다. <br>이를 lstm 기반의 딥러닝 기법을 이용해서 사람이름을 학습하고 분류하여 자동으로 찾아내도록 한다. 

![](./path/to/image.png)

<br>
<br>

## Requirments
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
0. 설치<br>
Requirments 에 적힌 라이브러리를 설치한다.
1. 쥬피터 노트북 접속 
``` cmd
$ jupyter notebook
```
2. 데이터 준비<br>
```data/name``` 경로에 사람이름이 적힌 txt 파일과 ```data/etc```에 3글자로 이루어진 이름외 명사 및 고유명사 등의 단어들이 적힌 txt 파일을 준비한다.
3. data.ipynb 로 학습을 위한 데이터셋 생성<br>
데이터셋은 ```data/use_data``` 폴더에 생성된다.
4. train.ipynb로 학습<br>
학습된 모델경로는 ```model/```에 생성되고 마지막에 있는 성가지표로 학습성능을 확인한다.
5. inference.ipynb로 추론(테스트)<br>
여기서 추론용 데이터는 본인의 은행거래 데이터를 사용해서 확인해보자.
6. 튜닝<br>
성능을 더 올리기 위해서 2번에서 데이터를 수정하고 5번까지 진행하면서 결과를 성능평가표에 기록한다.

<br>
<br>

## 정보
최승언 – [@velog](https://velog.io/@csu5216) – su.choi@niccompany.co.kr

라이센스: 원본 코드의 라이센스 또는 본인이 작성


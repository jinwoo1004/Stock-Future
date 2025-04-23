# 📈 Stock Future

본 프로젝트는 머신러닝과 딥러닝을 활용하여 주가를 예측하는 것을 목표로 진행되었습니다.  
현재까지 총 2개의 미니 프로젝트로 구성되어 있으며, 주요 내용은 다음과 같습니다.

## 프로젝트 구성

### 1. 뉴스 데이터를 활용한 KOSPI 지수 예측

- `pandas_datareader`를 사용하여 KOSPI 지수 데이터를 수집합니다.
- `BeautifulSoup`을 활용해 Naver, Paxnet 등의 사이트에서 뉴스 데이터를 크롤링합니다.
- `konlpy`로 뉴스 텍스트를 형태소 분석한 뒤, 감성 분석 모델을 적용하여 KOSPI 지수를 예측합니다.

### 2. 딥러닝을 활용한 종목별 주가 예측

- `pandas_datareader`의 `get_data_yahoo`를 이용해 종목별 주가 데이터를 수집합니다.
- `TensorFlow` 기반의 LSTM(Long Short-Term Memory) 모델을 생성하여 주가를 예측합니다.

## 참고 사항

### 💡 TensorFlow 설치 방법

1. 명령 프롬프트(cmd)를 실행하여 다음 명령어로 conda를 최신 버전으로 업데이트합니다:
   ```bash
   conda update -n base conda
   
2. (최초 실행 시) 필요한 패키지를 설치합니다:
   ```bash
   pip install jupyter notebook
   pip install ipykernel

3. 가상환경을 Jupyter Kernel에 등록합니다:
   ```bash
  python -m ipykernel install --user --name tensor_37_env --display-name "[Tensorflow_37_env]"

4. 가상환경을 Jupyter Kernel에 등록합니다:
   ```bash
  jupyter notebook

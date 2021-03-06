# Machine Learning for Healthcare Analytics Projects(한국어 번역판)

**Machine Learning for Healthcare Analytics Projects** 한국어 번역판 예제 코드를 공유를 위한 사이트이다.

## 예제 파일 사용법

- 이 사이트를 다운로드하거나 클론닝하여 사용한다. 

	1. 다운로드한 압축을 해제한다.
	2. 아나콘다 프롬프트(윈도우) 또는 터미널(맥)을 실행한다.
	3. 아나콘다 프롬프트/터미널에서 압축 해제한 폴더로 이동한다. 
	4. 가상 환경을 활성화시킨다. 
	5. 커맨드라인에서 주피터 노트북(Jupyter Notebook) 또는 주피터랩(JupyterLab) 실행시키고 노트북 파일을 열어서 활용한다.
	
	        (ml4hap)...$ jupyter notebook (또는 jupyter lab)



## 원본 예제 파일 공유 사이트 

- 원본 예제 코드 파일은 <https://github.com/PacktPublishing/Machine-Learning-for-Healthcare-Analytics-Projects>에 있다. 번역을 하면서 필요한 부분은 적절히 수정했지만, 오히려 그 과정에서 실수를 범했을 수도 있다. 필요한 경우 원본 코드와 대조해 보길 권한다. 

## 번역본에서 고려한 주요 내용

- 파이썬 > 3.8.6 버전에 맞추고, 업그레이드된 패키지에 맞춰 코드를 수정했다(파이썬 2.X 버전을 모두 수정).

- 파이썬 데이터 과학을 위한 컴퓨터 환경 구성에 대해 자세히 설명했다.
  - 아나콘다 파이썬의 설치 
  - 콘다(conda)를 이용한 가상 환경 생성 및 관리
  - 콘다(conda)를 이용한 패키지 관리
  - 데이터 과학에 필수적인 주피터 노트북을 비롯한 주피터 에코시스템 소개


## 번역본에 사용된 파이썬과 주요 패키지 설명

본역본의 코드는 아래 환경에서 실행되는 것을 검토했다.

- 파이썬 바이너리: python=3.9.7
- 넘파이: numpy=1.19.5
- 판다스: pandas=1.3.5
- 맷플롯립: matplotlib=3.5.1
- 사이파이: scipy=1.7.3
- 사이킷런: scikit-learn=1.0.2
- 케라스: keras=2.7.0
- 텐서플로: tensorflow=2.4.1
- 주피터:  jupyter=1.0.0
- 주피터랩: jupyterlab=3.0.14


## 코드 실행을 위한 콘다 가상 환경 구성 

번역하 때 사용하 콘다 가상 환경이다. 아나콘다 파이썬이 설치되어 있다고 가정한다. 

1. 윈도우의 경우 아나콘다 프롬프트, 맥은 터미널을 실행한다.
1. 다음 명령을 실행한다. 파이썬 버전을 3.9으로 하고 가상 환경의 이름은 `ml4hap`으로 지정했다.

		(base)...$ conda create --name ml4hap python=3.9

1. 가상 환경을 활성화시킨다. 
   
		(base)...$ conda activate ml4hap 

1. 주피터를 가상 환경에 설치한다. 

		(ml4hap)...$ conda install -c anaconda jupyter

1. 주피터랩을 가상 환경에 설치한다.

		(ml4hap)...$ conda install -c conda-forge jupyterlab

1. 넘파이, 판다스, 맷플롯립을 가상 환경에 설치한다.
   
		(ml4hap)...$ conda install numpy pandas matplotlib

1. 텐서플로를 가상 환경에 설치한다.
   
		(ml4hap)...$ conda install -c conda-forge tensorflow
	
1. 케라스를 가상 환경에 설치한다.

		(ml4hap)...$ conda install -c conda-forge keras

## UCI 머신러닝 데이터 저장소

- 5장을 제외하고는 모든 데이터는 UCI 머신러닝 데이터 저장소에서 코드로 내려받아 실행된다.

- 가끔은 이 사이트가 반응하지 않는 경우가 있어서, CSV 파일로 `uci_data` 폴더에 저장해 두었다. 

- 각 장의 데이터 로딩 코드에서 `pd.read_csv()`에서 `url` 부분을 `uci_data/파일이름`으로 바꿔 사용할 수 있다.





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

- 파이썬 3.8.6 버전에 맞추고, 업그레이드된 패키지에 맞춰 코드를 수정했다(파이썬 2.X 버전을 모두 수정).

- 파이썬 데이터 과학을 위한 컴퓨터 환경 구성에 대해 자세히 설명했다.
  - 아나콘다 파이썬의 설치 
  - 콘다(conda)를 이용한 가상 환경 생성 및 관리
  - 콘다(conda)를 이용한 패키지 관리
  - 데이터 과학에 필수적인 주피터 노트북을 비롯한 주피터 에코시스템 소개


## 번역본에 사용된 파이썬과 주요 패키지 설명

본역본의 코드는 아래 환경에서 실행되는 것을 검토했다.

- 파이썬 바이너리: python=3.8.6
- 넘파이: numpy=1.20
- 판다스: pandas=1.2.4
- 맷플롯립: matplotlib=3.4.1
- 사이파이: scipy=1.6.3
- 사이킷런: scikit-learn=0.24.2
- 케라스: keras=2.4.3
- 텐서플로: tensorflow=2.4.1
- 주피터:  jupyter=1.0.0
- 주피터랩: jupyterlab=3.0.14

**주의**: 파이썬 바이너리를 3.8.6으로 고정하여 가상 환경을 구성하면 패키지를 설치하고 사용함에 문제가 없을 것이다. 더 최신의 파이썬 바이너리를 사용하는 경우 텐서플로와의 호환성이 문제가 될 수 있다. 

다음 절차에 따라서 콘다 가상 환경을 구성하고 필요한 패키지들을 설치한다. 아나콘다 파이썬이 설치되어 있다고 가정한다. 

1. 윈도우의 경우 아나콘다 프롬프트, 맥은 터미널을 실행한다.
1. 다음 명령을 실행한다. 파이썬 버전을 3.8.6으로 하고 가상 환경의 이름은 `ml4hap`으로 지정했다.

		(base)...$ conda create --name ml4hap python=3.8.6

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




## 머신러닝 연구회(2019년)
- 2019년 머신러닝 연구회(이하 "머연")는 "밑바닥부터 시작하는 딥러닝"으로 개념학습을 합니다.(30분 이내) : [코드](https://github.com/WegraLee/deep-learning-from-scratch)  
- 캐글의 커널과 데이터를 통해 데이터 [EDA](https://eda-ai-lab.tistory.com/13)와 데이터 모델링을 학습합니다.(1시간+@)  
- 주요 관련 학회 논문을 리뷰합니다.(30분 이내)  
- 참석하시는 모든 분들은 노트북을 지참하셔야 합니다. 교재는 드립니다.  
  단, 커피 등 음료 및 다과는 개인별로 준비하여 주시고 도네이션은 언제나 환영입니다. (__)  
### 첫번째 시간
- 머연 소개(5분) + 교재 배포(5분) + 인터넷 연결(5분)
- 교재 학습(20분) : 2장 퍼셉트론(게이트), [코드](https://github.com/WegraLee/deep-learning-from-scratch/tree/master/ch02)  
- [캐글](https://www.kaggle.com/) 가입(10분) + 설명(10분) + 실습(1시간+@) : [House Price Prediction EDA](https://www.kaggle.com/chocozzz/house-price-prediction-eda-updated-2019-03-12)  
- 논문 리뷰(30분) : [Learning to Make Analogies by Contrasting Abstract Relational Structure](https://openreview.net/forum?id=SylLYsCcFm&fbclid=IwAR2ZuOupcgQvFOZHmhYFFLH17FFb2bYPZdumYBTmvLkWtWjv4NbnkwgNqLE), [ICLR 2019 리뷰](https://hoya012.github.io/blog/ICLR-image-recognition-paper-guide/)    
### 참고자료
- [모두를 위한 머신러닝/딥러닝 강의](https://hunkim.github.io/ml/?fbclid=IwAR1xF_LJVUW1JW2HEfpXLm3tC2NPkKZba3mCGi8DtAygO6tREw-TJqwN_98)  
- [모두를 위한 딥러닝 시즌2](https://www.youtube.com/playlist?list=PLQ28Nx3M4Jrguyuwg4xe9d9t2XE639e5C&fbclid=IwAR2gEytKg0CHIoS8yL_wXX0OmLXcDHc3VFVzkRuuqzoqJDY1WsVk5nUqNWw)   

### 이전 작성분
- 2019년은 빅데이터 연구방법론 중 
- (데이터 수집-저장)은 ELKv4를 통해 진행합니다.  
1) (웹 포털, 비정형 텍스트) 네이버 뉴스(https://news.naver.com/) : 환경<사회, 이 시각 주요뉴스(텍스트;포토)(2회차)  
2) (웹 포털, 반정형 텍스트) 한국학술정보 KISS : 간행물(전체, 특정)(1회차)  
3) (웹 포털, 비정형 텍스트, 파일) 에어코리아 최종확정자료 연도별 다운로드(1회차)   
4) (오픈API) 공공데이터포털 대기오염정보 조회 서비스(1회차  
5) +@  
- (데이터 분석-처리)는 머신러닝 연구회와 블록체인 연구회를 구분해서 운영합니다.
- 머신러닝 연구회는 연구자 활용을 목적으로 
1) 애저 ML 스튜디오 가이드(2회차) : https://docs.microsoft.com/ko-kr/azure/machine-learning/studio/
2) 캐글스터디(3회차) : https://www.kaggle.com/
- 블록체인 연구회는 하이퍼레저 구현을 목적으로
1) 교재 : 하이퍼레저 패브릭으로 배우는 블록체인(https://kyobobook.co.kr/product/detailViewKor.laf?ejkGb=KOR&linkClass=33&barcode=9791188621453)  
2) 교재를 중심으로 하이퍼레저를 구축하는 것이 올해 목표입니다.  
3) 하이퍼레저(Hyperledger)는 업계 표준기술이라고 생각하시면 됩니다.  
4) 투표, 문서유통, 농축산물 및 부동산 이력관리, 통관 등 공공선도 사업도 하이퍼레저 기반으로 구축될 것입니다.   
- 과기정통부 블록체인 예산 87억 -> 319억, 
- 공공선도 사업 중 환경부 온실가스종합정보센터, 블록체인 기반 탄소배출권(외부감축사업) 이력관리 시스템 구축  
  
### 환경구축(별도 워크숍)
- 아나콘다(Anaconda) 설치  
- [Anaconda Tensorflow GPU 버전 설치](https://junn.in/archives/2466)  
[CUDA Toolkit 9.0](https://developer.nvidia.com/cuda-90-download-archive?target_os=Windows&target_arch=x86_64&target_version=7&target_type=exelocal) / [cuDNN for CUDA 9.0](https://developer.nvidia.com/rdp/cudnn-download)  
- https://www.tensorflow.org/guide/using_gpu  
- http://hellogohn.com/post_one38  
  
### TensorFlow 기초  
선행학습 요구 : 파이썬을 모르시면, 참여가 어렵습니다.  
- [골빈해커의 3분 딥러닝, 텐서플로맛](https://github.com/golbin/TensorFlow-Tutorials)
- [pythonkim.tistory.com](http://pythonkim.tistory.com/8?category=573319)  
  
### Pandas 기초(별도 워크숍)
선행학습 요구 : 파이썬을 처음하셔도 괜찮지만, 문법을 모르시면 참여가 어렵습니다.
- [팬더스 데이터분석 기초 실습](http://edu.goorm.io/lecture/3999/pandas-%ED%8C%AC%EB%8D%94%EC%8A%A4-%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B6%84%EC%84%9D-%EA%B8%B0%EC%B4%88-%EC%8B%A4%EC%8A%B5)  
  
### 데이터 처리(별도 워크숍)
- [파이썬으로 데이터 주무르기](https://github.com/PinkWink/DataScience)
- [Ultimate guide to handle Big Datasets for Machine Learning using Dask(in Python0](https://www.analyticsvidhya.com/blog/2018/08/dask-big-datasets-machine_learning-python/?utm_medium=social&utm_source=facebook.com&utm_campaign=buffer)
- [국민대학교 빅데이터 강의](http://doc.mindscale.kr/km/)
  
### 데이터 분석(별도 워크숍)
- [파이썬으로 머신러닝 배우기 (3/3)](https://www.youtube.com/watch?v=BUmAlJUOmKo&feature=youtu.be)  
  
### 캐글 스터디(별도 워크숍)
- [Home Credit Default Risk](https://www.kaggle.com/c/home-credit-default-risk)
  
### [KEI 환경 블록체인 연구회](https://github.com/ur1ove/KEIBC)

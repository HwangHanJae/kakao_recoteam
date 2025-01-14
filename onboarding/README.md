# 추천팀 온보딩

카카오 추천팀에 입사하기 전에 미리 보시면 좋을 내용들을 정리해놓은 문서입니다.

## 추천 기술 관련 자료

해당 내용에 링크된 자료는 방대하므로(특히 수학/ML 기초) 필요한 부분들 위주로 보시기 바랍니다.

### 수학/ML 기초

추천 시스템은 머신러닝의 응용 분야로서 머신러닝에 대한 기초지식을 탄탄히 다지는 것은 큰 도움이 됩니다. 기본적인 Linear Algebra, Statistical Inference, Convex Optimization에 대해 익숙하지 않다면 이에 대한 학습이 필요할 수 있습니다.

대표적인 ML 교재 최소 1개 이상을 정독해본 경험을 가지는 것을 추천해 드립니다.

- [Introduction to Statistical Learning (ISLR)](https://www.statlearning.com/)
- [Elements of Statistical Learning (ESL)](https://hastie.su.domains/Papers/ESLII.pdf)
- [Machine Learning: A Probabilistic Perspective (Murphey 책)](https://probml.github.io/pml-book/)
- [Pattern Recognition an Machine Learning (Bishop 책)](https://www.microsoft.com/en-us/research/uploads/prod/2006/01/Bishop-Pattern-Recognition-and-Machine-Learning-2006.pdf)
- ... etc.

딥러닝 교재, 최신 추천시스템은 뉴럴넷을 활용하는 경우도 많고 자연어, 이미지 등의 데이터를 활용하는 경우도 있습니다.

- [Deep Learning Book](https://www.deeplearningbook.org/)
- ... etc.

### 추천 알고리즘

대표적인 올드 스쿨 알고리즘입니다. 해당 알고리즘들은 논문이 발표된지 오래되었지만, 아직도 대중적으로 많이 활용되고 있습니다.

- iALS ([Collaborative Filtering for Implicit Feedback Datasets](http://yifanhu.net/PUB/cf.pdf))
- BPR ([BPR: Bayesian Personalized Ranking from Implicit Feedback](https://arxiv.org/pdf/1205.2618.pdf))
- LinUCB ([A Contextual-Bandit Approach to Personalized News Article Recommendation](https://arxiv.org/pdf/1003.0146.pdf))

그 외, 벤치마크로 자주 등장하는 전통 알고리즘은 다음과 같습니다.

- WARP ([Improving Pairwise Learning for Item Recommendation from Implicit Feedback](http://webia.lip6.fr/~gallinar/gallinari/uploads/Teaching/WSDM2014-rendle.pdf))
- SLIM ([SLIM: Sparse Linear Methods for Top-N Recommender Systems](https://ieeexplore.ieee.org/abstract/document/6137254))

카카오 테크 블로그에 카카오 추천시스템에 대하여 주제별로 설명한 글들입니다.

- [테크 블로그: 추천 시스템](/README.md/#%EC%B6%94%EC%B2%9C-%EC%8B%9C%EC%8A%A4%ED%85%9C)

추천 관련 최신 논문들을 서칭해보고 abstract와 related works를 읽어보면 최신 연구 방향과 그 기반이 되는 주요 논문들을 알 수 있습니다

- 추천 관련 대표 학회들: RecSys, WWW, SIGIR, KDD, WSDM, CIKM, AAAI, IJCAI, ICML, NeurIPS, ... etc.

(좋은 논문인지와 별개로) 대표적으로 유명한 추천 알고리즘 논문들은 아래와 같습니다.

- [BERT4Rec: Sequential Recommendation with Bidirectional Encoder Representations from Transformer, CIKM'19](https://arxiv.org/abs/1904.06690)
- [Variational Autoencoders for Collaborative Filtering, WWW'18](https://dl.acm.org/doi/10.1145/3178876.3186150)
- [Neural Collaborative Filtering, WWW'17](https://dl.acm.org/doi/10.1145/3038912.3052569)
- [Recommending What Video to Watch Next: A Multitask Ranking System, RecSys'19](https://daiwk.github.io/assets/youtube-multitask.pdf)
- [Collaborative Metric Learning, WWW'17](https://vision.cornell.edu/se3/wp-content/uploads/2017/03/WWW-fp0554-hsiehA.pdf)
- [Convolutional Matrix Factorization for Document Context-Aware Recommendation, RecSys'16](http://uclab.khu.ac.kr/resources/publication/C_351.pdf)
- ... etc.

### 그 외

#### 강화학습

실시간 추천시스템은 사용자와 상호작용하며 사용자들의 취향을 파악하고 추천해주는 시스템으로서 강화학습 framework이 잘 어울린다는 평가가 많습니다, 특히 Multi-Armed Bandit, Contextual-Bandit 등은 팀 내에서도 매우 많이 사용되고 있습니다

- [강화학습 대표 교재 (Reinforcement Learning: An Introduction)](http://incompleteideas.net/book/the-book.html)
- [David Silver 강의](https://www.davidsilver.uk/teaching/)

## 머신러닝플랫폼 관련 자료

아래의 키워드는 모두 머신러닝플랫폼에서 중요한 것들이지만 업무에 필수는 아닙니다.
학습 비용이 만만치 않기 때문에 천천히 기반 다지는 것을 추천합니다.

### 방법론, 가이드

- [Domain Driven Design (DDD)](https://martinfowler.com/bliki/DomainDrivenDesign.html)
- [Microservices (MSA)](https://learn.microsoft.com/en-us/azure/architecture/guide/architecture-styles/microservices)
- [Event Driven Architecture (EDA)](https://learn.microsoft.com/en-us/azure/architecture/guide/architecture-styles/event-driven)
- [Cloud Native](https://learn.microsoft.com/en-us/dotnet/architecture/cloud-native/definition)
- [CI/CD](https://en.wikipedia.org/wiki/CI/CD)
- [Test Driven Development (TDD)](https://martinfowler.com/bliki/TestDrivenDevelopment.html)

### 개발 자원

머신러닝플랫폼은 대부분 파이썬 3.10을 사용하고 있습니다.
아래는 개발할 때 많이 사용하는 라이브러리를 간추렸습니다.

- [poetry](https://python-poetry.org/)
- [pydantic](https://pydantic-docs.helpmanual.io/)
- [pytest](https://pytest.org)
- [mypy](https://mypy.readthedocs.io/)

## 팀 개발환경 및 플랫폼

### 기본 개발환경

팀의 메인 개발언어는 Python, C++입니다.

코드 Editor로는 주로 Vim을 사용하고 있으나, 제약은 없으며 VSCode, PyCharm등 개발자 본인에게 가장 편한 editor를 사용할 수 있습니다. (단, 서버 내에서 작업하는 경우도 많기에, Vim에 대한 기본적인 사용법을 익혀두시면 유용합니다.)

- [Vim](https://www.vim.org/)
  - [Vim adventures](https://vim-adventures.com/): Vim을 간단한 게임형태로 배워볼 수 있는 페이지입니다.

코드의 버전관리는 Git / GitHub를 사용하고 있습니다.

- [git](https://git-scm.com/)
  - [Git/GitHub 안내서](https://subicura.com/git/guide/)

팀 내 대부분의 서비스는 docker 및 kubernetes를 기반으로 동작합니다.

- [docker](https://www.docker.com/)
  - [초보를 위한 도커 안내서](https://subicura.com/2017/01/19/docker-guide-for-beginners-1.html)
- [kubernetes](https://kubernetes.io/)
  - [쿠버네티스 안내서](https://subicura.com/k8s/guide/#%E1%84%80%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%83%E1%85%B3)

### 플랫폼

#### Kafka

추천 시스템에서는 각 유저가 어떤 아이템을 소비했는지, 또 소비한 아이템에 대해 어떠한 반응을 보였는지에 대한 정보가 중요하게 사용됩니다. 이러한 정보는 서비스단에서 실시간으로 수집되어 [Kafka](https://kafka.apache.org/)를 통해 추천팀에서 받아볼 수 있는 형태로 전달되고 있습니다. 따라서 Kafka의 기본구조 및 동작 방식에 대해 미리 알아두시면 팀에서 실제 업무를 하실 때 많은 도움이 됩니다.

- [Youtube강의-아파치 카프카](https://www.youtube.com/playlist?list=PL3Re5Ri5rZmkY46j6WcJXQYRlDRZSUQ1j)

#### MongoDB

[MongoDB](https://www.mongodb.com/)는 팀에서 가장 많이 사용하는 key-value storage 중 하나이며, 주 사용처는 다음과 같습니다.

- 개별 유저에 대한 추천 결과 저장(캐시 용도)
- Feature storage
- 유저들의 아이템 소비 로그, 피드백 로그 저장

MongoDB 참고 자료 (팀 내에서 직접 관리를 하는 것은 아니기에 깊이 보실 필요는 없습니다. 아래에서는 3, 4, 5를 위주로 보셔도 괜찮습니다.)

- [1편: 소개, 설치 및 데이터 모델링](https://velopert.com/436)
- [2편: Database/Collection/Document 생성, 제거](https://velopert.com/457)
- [3편: Document Query(조회) - find() 메소드](https://velopert.com/479)
- [4편: find() 메소드 활용 - sort(), limit(), skip()](https://velopert.com/516)
- [5편: Document 수정 - update() 메소드](https://velopert.com/545)
- [pymongo docs](https://pymongo.readthedocs.io/en/stable/)
  - pymongo는 MongoDB의 python client로써, 팀에서 MongoDB를 다룰 때 주로 사용하고 있습니다.

#### Hadoop

[Hadoop](https://hadoop.apache.org/)을 구성하는 여러 가지 요소가 있지만, 팀에서는 주로 HDFS, Hive(Presto, Spark)를 많이 사용합니다. Hadoop의 개별 요소를 세세히 설명하기엔 양이 너무 방대하기에, 간단한 개념 위주로 링크를 정리했습니다.

- HDFS: 유저 x 아이템 interaction 데이터 저장, 학습된 추천 모델 저장 등
  - [hdfs 기본개념](https://kadensungbincho.tistory.com/30)
  - [hdfs 명령어 모음](https://blog.voidmainvoid.net/175)
- Hive(Presto, Spark): 데이터 분석, 전처리 등에 사용
  - [Hive, Presto, Spark 기본 설명](https://seoyoungh.github.io/data-science/distribute-system-1/)

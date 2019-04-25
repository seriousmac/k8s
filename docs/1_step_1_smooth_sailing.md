ref: https://cloud.google.com/kubernetes-engine/kubernetes-comic/?authuser=2 <br/>
만화로 보는 쿠버네티스 :) <br/>
이것부터 마스터한다아!!! <br/>

# Smooth Sailing with kubernetes
- what kubernetes is
- how you can use it
- for continuous integration and delivery


- 장면 1
  - **k8s**가 무엇이며, **지속적인 통합 및 배포**에 어떻게 활용할 수 있는지 알아 볼 수 있는 온라인 만화

- 장면 9~10
  - 컨테이너에 앱을 배포했지만, 모든 문제가 해결되지는 않음
  - 관리하기에 여전히 시간이 많이 걸리고 효율성도 떨어지고 헛점도 많음
  - '지혜와 기교, ~~전쟁~~**컨테이너식 애플리케이션**'의 여신 아테나가 말하기를,
  - 앱을 언테이너에 배포하는 것이 중요한 첫걸음이지만, 그 후에는 앱을 **조정**해야해요. 그래서 **k8s이 필요**하죠.
  
- 장면 12~16
  - 모놀리스
    - 모놀리스식 애플리케이션이 대세였던 시절(통굽 신발 유행, 왕좌의 게임 시즌 2가 방송되던 실절)
    - 모놀리스식 서비스는 인상적인 기능들이 많이 있었지만, 상호 의존적인 부분이 너무 많아서 통합하고 배포하기가 상당히 어려움
  - 마이크로
    - 마이크로 서비스는 전체 프로젝트를 중단할 필요 없이 '마이크로 서비스'를 각각 디버깅, 업데이트, 배포할 수 있음
    - 지속적 통합 및 배포로 전환하기 위한 중요한 단계
    - 통신은 가벼운 프로토콜을 사용하여 느슨하게 연결되어 있음
    - 상호 의존적인 하향식 계층구조를 가짐
    
- 장면 18~21
  - 단일 운영체제 아키텍처: CPU/Memory > Kernel > OS > applications
    - 문제점: 라이브러리 버전 및 애플리케이션 구성요소가 충돌할 수 있음
  - 하나의 가상 머신 아키텍처: CPU/Memory > Kernel > OS > 1 VM - n APP
    - 하나의 가상 머신에서도 애플리케이션이 서로 충돌할 수 있음
  - 애플리케이션 별 가상 머신 아키텍처: CPU/Memory > Kernel > OS > n VM = n App
    - 너무 무겁고 낭비, 비용도 많이 듬
  - **독립 실행형 프로세스(SELF-CONTAINED PROCESS)**
    - 하나의 라이브러리와 설정이 내장된 상태에서 각 프로세스가 자체적으로 실행되도록 구축
    - 즉, 각 프로세스가 가상 머신이든 베어 메탈 머신이든 어느 머신에서나 실행될 수 있도록 모든 조건을 제공

- 장면 25~26
  - 마이크로 서비스가 컨테이너식 앱으로 실현된적 = 없었음
  - 모듈화(Modularity) + 상호 운용성(Interoperability)

- 장면 30~32
  - **이동성(Portability)**, **재현성(Reproducibility)**, **확장성(Scalability)**
  
- 장면 34
  - 이 모든 것을 **전 세계 어디서나 언제든지** 실현 가능
  - 확장하면 어떻게 다 추적해? -> k8s를 사용하면, 모든 컨테이너가 **자동화**

- 장면 43
  - Kubernetes의 주요 목표
    - 컨테이너를 논리적(Logical)이고 효율적인(Efficient) 방식으로 분산하는 것
    - 이미 진행 중인 작업에 맞춰 신속하게(Face) 확장(Scale up) 또는 축소하는 것
    - 프로세스를 안정적인(Healthy) 상태로 지속적으로 실행하는(Running) 것
    - **작업에 대한 통제력을 갖는 것** (To give you power over **WHAT** gets done)
    - 행복한 주말 (Withour forcing you to micro-manage **HOW**)
    

    
    

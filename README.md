# Socar Fraud Detection Project

Teams: 이진서, 임상우, 김재욱 (Fastcampus Datascience school 14th)


![image](https://user-images.githubusercontent.com/68367214/97532893-a115a200-19fa-11eb-9049-2dcadfc44eac.png)

* 교보생명의 보험사기 사전예측

교보생명이 인공지능(AI)과 머신러닝 기술로 보험사기 가능성을 사전에 경고해주는 
보험사기예측시스템(K-FDS)을 자체 개발해 본격 운영에 들어갔다고 올해 5월 26일 발표.

실제적으로 교보생명에서는 1년간의 시범적 운영을 통해 200여건의 부당 보험금 지급 방지에 성공.


## Storyline

위 사례처럼 본 쏘카 프로젝트에서는 앞으로 발생할 Fraud 를 예측하고 줄이는데 도움을 줌으로써, 
잠재적으로 발생하는 손실을 방어해줄 수 있어야 할 것이다.

효과적으로 선별할 수 있는 기준을 세우고, Fraud 고위험군 사용자들을 사전 분류하여 
사고접수/처리시 이용한다면 자사에 이익을 줄 수 있을것으로 본다.


사고처리 프로세스에서 Fraud 고위험군 사용자들을 식별해 냈다면, 
이 정보를 활용함에 있어서 어떤 점이 중요할까?

사고를 처음으로 접수하는 순간에, 사전 분류된 사용자들을 집중조사하여 사기를 식별해 내야 하는 점이다. 
시간이 지나 고장을 발견하는 경우, Fraud를 발생시킨 유저 이후에 사용한 유저들이 생겨나 증명에 문제가 생기기 때문이다.

따라서 실질적인 자사 서비스에 적용에 있어서 '시점'이 매우 중요하다고 할 수 있다.


최종적으로 우리는 최초의 사고가 식별되었을 때, 사용자 분류를 통하여
최초 사고가 발생하는 시점에 집중 검증할 수 있게 될 것을 목적으로 한다.


## Goals

* 최초 사고 식별시, 머신러닝의 여러기법을 통해 Fraud 일 가능성이 높은 경우, 담당자에게 고위험군임을 알리는 서비스 구축.

Method 

1. 상담원 콜 발생시, 연동 웹페이지 상에서 메시지 노출.
2. 챗봇 운영시 최초 상담 시작시, 상담원에게 메시지 노출.

(현재 쏘카에서는 콜을 통해서만 사건/사고를 접수하지만, 챗봇을 통한 문의에도 적용가능하도록 구현.)


## Execution

1. 데이터 전처리
2. EDA
3. 분석 모델 적용 및 인사이트 도출
4. Monge DB를 통한 데이터베이스 구축
5. 1) Flask를 통한 웹페이지 서비스
   2) Chatbot 서비스


## Machine Learning Model

* Machine Leaning - Supervised Leaning - Classification

1. Decision Tree
2. Logistic Regression
3. KNN
4. SVM
        
        
## Architectures

![Socar_project-Page-2](https://user-images.githubusercontent.com/68367214/97545022-bf38cd80-1a0d-11eb-84a7-30a7d3d5a116.png)


## Details

* 분류기법 적용예정.

ex) EDA

Not Fraud
![notfraud_repair_cost](https://user-images.githubusercontent.com/68367214/97549401-b0551980-1a13-11eb-8017-7da1a5772841.PNG)

Fraud
![fraud_repair_cost](https://user-images.githubusercontent.com/68367214/97549509-d24e9c00-1a13-11eb-9d37-d9a3e56f2c30.PNG)



## Project Improvements

![Socar_project](https://user-images.githubusercontent.com/68367214/97540316-d1fbd400-1a06-11eb-987f-cfc3fe6df66b.png)


* 이후 분석에 필요한 추가 Feature 제안내용 :
    
- 제12조 자동차 미반납에 대한 조치
① 회사는 회원이 대여 기간 종료 시로부터 3시간을 경과하여도 반납 장소에 자동차를 반납하지 아니하거나 
  회사의 반납 요청에 응하지 않을 때에는 자동차 회수 및 손해보전에 필요한 모든 법적 조치를 취할 수 있습니다. 

⑤ 1. 회원이 회사의 자동차 반납요구에도 불구하고 정당한 사유 없이 자동차를 반납하지 않거나 
  연락이 되지 않는 상태에서 자동차 반납일로부터 6시간 내에 반납하지 아니한 경우
  2. 회원이 서비스 요금을 연체하여 회사가 상당기간 동안 2회 이상 납부를 최고하였음에도 계속 연체하고 있는 경우

 
=> 반납시간 또는 연체 횟수에 따른 칼럼도 추후 추가 Feature로 수집이 된다면 예측에 도움이 될 것.

## Presentation Resourses

1. Sweetviz
2. Draw.io (다이어그램 제작 링크-웹에서 권한 공유하여 수정가능) : https://app.diagrams.net/#G1QTiFJettkl6p3ymERp04PKKDLXpOJqgE
3. Tableau


## learning materials

1. Socar 약관링크 : https://www.socar.kr/terms
2. 머신러닝 기법책(?)

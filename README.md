# 머신러닝 기반 회계부정 기업 예측 모델 개발

- [🎥 [2020데이터청년캠퍼스X연세대학교]머신러닝 기반 회계부정 기업 예측 모델 개발 발표 영상](https://youtu.be/4MUFZ79xNns)
- 🏆 2020 빅데이터 청년인재 양성 사업(데이터 청년 캠퍼스) 프로젝트 평가 장려상 수상

## 💡 기획의도
회계부정이란 기업의 재무상태와 성과를 의도적으로 조작하는 비도덕적인 불법 행위로 자산이나 이익을 부풀리거나 비용을 축소하여 이익을 증가시키는 형태가 대부분이다.
2000년대 초 발생한 대표적인 회계부정 사례인 "엔론 사태" 이후에도 계획된 회계부정으로인한 막대한 사회적, 경제적 손실이 발생하고 있다. 최근 신(新)외감법의 도입으로 회계법인의 책임은 커졌지만, 부실감사에 대한 감리 지적은 여전히 증가 추세를 보이고 있다.

**본 프로젝트 구성원은 해당 문제의 원인이 "감사 시즌 집중된 업무 부담과 효율적이지 못한 실증적 분석 절차 이용"이라고 보고, 머신러닝을 통해 회계부정을 빠르고 정확하게 예측할 수 있는 모델을 구현하고자 하였다.**

## 🧭 분석과정 Overview
![오버뷰](https://user-images.githubusercontent.com/68639271/126611305-c43c1d54-a807-495d-93af-9d93ec3ec28c.png)

📍 **최종 모델은 DNN(Deep Neural Network)로 구현하였으며, 해당 모델을 택한 이유는 다음과 같다.**
- 클래스별 가중치 처리가 가능해 Over sampling을 하지 않아도 데이터 불균형 처리 가능
- 총 변수 개수가 많아 과적합이 우려되는 상황에서 DNN의 Drop-out Layer를 통해 효과적으로 과적합 규제 가능
- Logistic Regression, Random Forest, XGBoost 등 타 머신러닝 모델 대비 고성능(recall=0.87)

## 🧠 사용 언어 및 개발 환경
- Python : 본 프로젝트는 파이썬으로 기업 재무제표 데이터를 전처리하고, 머신러닝을 통해 재무제표의 비정상적 패턴을 예측한다.
- Jupyter Notebook
- KISVALUE : 10개년 기업 재무제표 데이터 추출 출처

## 👪 구성원
2020데이터청년캠퍼스 한배오리조

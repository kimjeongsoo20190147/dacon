# 한국어 기사 제목 분류 모델 (Korean News Title Classification)

이 프로젝트는 한국어 기사 제목과 키워드를 기반으로 기사의 카테고리를 자동으로 분류하는 머신러닝 모델입니다. 뉴스 분류 빅데이터 대회를 위해 개발된 모델로, 다양한 자연어 처리(NLP) 기법과 머신러닝 모델 앙상블(Stacking)을 사용하여 높은 정확도를 달성하였습니다.

프로젝트 개요
---
목적: 한글 기사 제목과 키워드를 활용한 뉴스 카테고리 자동 분류

데이터: 대회 제공 데이터셋(train.csv, test.csv)

모델: Word2Vec을 활용한 임베딩 및 Random Forest, XGBoost를 이용한 Stacking 앙상블 모델

사용된 주요 라이브러리 및 기술

자연어 처리(NLP)
---
형태소 분석기(Mecab)

Word2Vec (gensim)

불용어(stop words) 제거

데이터 전처리
---
Label Encoding (sklearn)

토큰화 및 키워드 결합

ADASYN을 이용한 클래스 불균형 해소

머신러닝 모델
---
Random Forest Classifier

XGBoost Classifier

Stacking Ensemble 모델



주요 작업 과정
---
데이터 로드 및 분석

형태소 분석(Mecab)을 통한 토큰화

불용어(stop words) 제거

Word2Vec을 이용한 단어 임베딩 벡터 생성

ADASYN을 통한 클래스 불균형 문제 해결

Random Forest와 XGBoost를 활용한 Stacking 앙상블 모델 구축 및 학습

모델 평가 (F1-Score)

예측 결과 CSV로 저장

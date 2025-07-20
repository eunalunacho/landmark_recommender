# 🌍 Landmark Image Recommendation (LeNet 기반 CNN 프로젝트)

**입력 이미지 한 장으로 유사한 여행지(랜드마크)를 추천합니다.**  
LeNet 기반 CNN 모델을 통해 Google Landmark Dataset 분류 문제를 다루며, 테스트 이미지로부터 Top-5 추천지를 시각화합니다.

---

## ✅ 프로젝트 개요

- Google Landmark Dataset을 기반으로 여행지 분류 및 추천 모델 설계
- 사용자가 업로드한 이미지를 입력으로 받아 유사 Landmark Top-5 추천
- CNN 모델 구조로 LeNet을 활용하여 학습 및 예측
- 이미지 증강 (좌우 반전, 회전 등)을 통해 적은 데이터에서도 학습 성능 확보
- 이미지 전처리 및 수집 자동화 (PIL + Requests 활용)
- Matplotlib 기반 추천 결과 시각화

---

## ⚠️ 데이터셋 참고 사항

> 현재 Google Landmark Dataset은 직접 다운로드 및 전체 접근이 제한되어 있어,  
> 본 저장소에서는 **10개의 대표 Landmark에 대한 샘플 이미지 데이터**로 대체하여 구현한 프로토타입을 포함하고 있습니다.  
> 전체 모델 성능 측정보다는 학습 파이프라인 및 추천 구조 설계를 중점적으로 보여주는 데 목적이 있습니다.

---

## 🧠 사용 기술

- Python, Colab 환경
- TensorFlow / Keras
- NumPy, Pandas, Matplotlib
- PIL, Requests (이미지 수집 및 전처리)

---

## 📊 예시 결과

- 입력 이미지: 🗼 Eiffel Tower  
- 추천 Top-5:  
  1. Great Pyramid of Giza (conf: 0.38)  
  2. Statue of Liberty  
  3. Taj Mahal  
  4. Golden Gate Bridge  
  5. Eiffel Tower (conf: 0.00)

---

## 📌 참고

- 실제 서비스 수준 모델 성능 확보를 위해서는 Google Landmark Dataset 전체 활용이 필요합니다.
- 대용량 학습/평가가 필요한 경우 GCP BigQuery 또는 Kaggle을 통해 Dataset 접근 권한을 신청할 수 있습니다.

---

## 🧪 개발자 참고

본 프로젝트는 학습용 목적의 소규모 Landmark 추천 모델을 구현한 예제로,  
모델 구조 설계, 이미지 전처리, 증강, 추천 시각화까지의 전체 MLOps 흐름을 이해하는 데 적합합니다.

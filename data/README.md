# Data

대회에서 제공한 데이터는 레포에 포함하지 않습니다.

## 원본 데이터
- **DataCo Smart Supply Chain for Big Data Analysis** (Constante, Silva & Pereira, 2019)
  - Mendeley Data: https://data.mendeley.com/datasets/8gx2fvg2k6/3 (DOI: 10.17632/8gx2fvg2k6.3)
  - Kaggle에도 같은 데이터셋이 공개되어 있습니다.

대회 데이터는 원본에서 누수 가능 컬럼을 제거하고 25개 피처로 정제한 뒤 train / test로 나눈 형태입니다.

## 배치 방법
```
data/
├── train.csv   # id + 피처 25개 + Late_delivery_risk (144,415행)
└── test.csv    # id + 피처 25개 (36,104행)
```

`02_hypothesis_eda.ipynb`는 팀 공통 전처리 결과인 `processed_train_MS.csv`를 함께 사용합니다.

# 사용한 코드

| 파일 | 원본 | 내용 |
|---|---|---|
| [01_center_a_time_series.ipynb](01_center_a_time_series.ipynb) | modeling2.ipynb | A센터 생수·음료·건강 및 신선식품의 SARIMA, SARIMAX, Seasonal Naive 실험 |
| [02_center_b_time_series.ipynb](02_center_b_time_series.ipynb) | modeling3.ipynb | B센터 봉지라면과 탄산음료의 ARIMA/SARIMA 실험 |
| [03_fresh_food_exploration.ipynb](03_fresh_food_exploration.ipynb) | A_물류센터_신선식품_매출.ipynb | 신선식품 EDA, 기온·강수량·물가 결합과 예측 탐색; Colab 형식 |

## 실행 전 준비

Python 3.10을 사용한 분석입니다. 별도 가상환경에서 `pip install -r requirements.txt`로 기본 패키지를 설치하고, `jupyter lab`에서 노트북을 여세요. 패키지 목록은 코드의 import를 정리한 것으로 당시 버전을 고정한 환경 파일은 아닙니다.

1. [데이터 안내](../docs/DATA.md)에 있는 입력 자료를 준비합니다.
2. 각 노트북의 `pd.read_csv` 경로를 실제 보관 위치에 맞춥니다. `전치리`처럼 원 코드에 들어 있는 파일명도 실제 파일명과 일치해야 합니다.
3. 첫 두 노트북은 `code/`를 기준으로 상대 경로를 사용합니다. 세 번째는 Google Drive 연결과 폰트 설치를 포함한 Colab용입니다. 로컬에서는 해당 셀을 건너뛰고 읽기 경로와 폰트를 설정해야 합니다.
4. 셀을 위에서부터 검토하며 실행합니다. 원본 실험 셀은 상태를 공유하므로 완성된 일괄 실행 파이프라인으로 보지 않습니다.

원자료가 없어 전체 실행은 확인하지 않았습니다. 이번 정리에서는 셀 내용 보존, 중복 파일, 노트북 형식과 비밀정보 포함 여부를 확인했습니다. 보고서의 Prophet 최종 실험과 매입량 산정 코드는 이 폴더에 없습니다.

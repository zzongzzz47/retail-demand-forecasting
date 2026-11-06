# 수요예측과 시계열 분석 공부 기록

예측 방법을 공부하면서 티스토리에 남긴 글 14편을 모았습니다. 기초 개념부터 간헐수요, 예측과 재고관리의 연결까지 주제별로 읽을 수 있습니다. 제목을 누르면 원문으로 이동합니다.

**[티스토리](https://zzongzz.tistory.com/) · [수요예측 프로젝트](../README.md) · [분석 보고서](../reports/nexus_demand_forecasting_report.pdf)**

## 처음 읽는다면

[자료의 형태](https://zzongzz.tistory.com/4) → [단순 모형](https://zzongzz.tistory.com/5) → [분해와 지수평활](https://zzongzz.tistory.com/6) → [ARIMA·SARIMA](https://zzongzz.tistory.com/7) 순서로 기초를 살펴볼 수 있습니다.

그다음에는 관심 있는 문제에 따라 나누어 읽으면 좋습니다.

- 판매가 드문 품목을 다룬다면 **간헐수요와 수요 유형**
- 딥러닝이나 모형 결합이 궁금하다면 **딥러닝과 결합 모형**
- 예측 결과를 발주에 연결하려면 **예측과 재고관리**

## 시계열 기초와 통계 모형

| 작성일 | 글 | 다룬 내용 |
|---|---|---|
| 2025-04-01 | [시계열 자료의 형태](https://zzongzz.tistory.com/4) | 단변량·다변량 시계열, 여러 시계열과 패널 자료, 과거·미래 설명변수의 차이. |
| 2025-04-01 | [단순 시계열 모형](https://zzongzz.tistory.com/5) | 평균, Naive와 계절 Naive 모형을 기준선으로 이해하고 예측오차와 예측구간 정리. |
| 2025-04-02 | [시계열 분해와 Exponential Smoothing](https://zzongzz.tistory.com/6) | 수준, 추세와 계절성으로 시계열을 나누는 방법과 지수평활 정리. |
| 2025-04-02 | [ARIMA모형과 SARIMA모형](https://zzongzz.tistory.com/7) | 자기회귀, 이동평균과 차분의 역할, 계절성을 반영한 SARIMA 정리. |
| 2025-06-20 | [Exponential Smoothing for Predicting Demand (1956)](https://zzongzz.tistory.com/9) | 초기 문헌을 읽으며 최근 수요에 가중치를 주는 방식과 평균·추세·분산 갱신 과정 정리. |

## 딥러닝과 결합 모형

| 작성일 | 글 | 다룬 내용 |
|---|---|---|
| 2025-01-12 | [시계열분석에 사용되는 딥러닝 모델](https://zzongzz.tistory.com/1) | RNN의 과거 정보 전달 방식과 장기 의존성 문제, LSTM과 GRU의 구조. |
| 2025-03-30 | [The hybrid PROPHET-SVR approach for forecasting product time series demand with seasonality](https://zzongzz.tistory.com/3) | Prophet과 SVR을 결합해 계절성과 비선형 패턴을 함께 다루는 논문 메모. |

## 간헐수요와 수요 유형

| 작성일 | 글 | 다룬 내용 |
|---|---|---|
| 2025-06-20 | [Forecasting and Stock Control for Intermittent Demands (1972)](https://zzongzz.tistory.com/10) | 수요가 없는 기간이 많은 품목에서 수요 크기와 발생 간격을 나누어 추정하는 Croston 방법. |
| 2025-11-19 | [On the bias of intermittent demand estimates](https://zzongzz.tistory.com/12) | Croston 추정의 편향과 이를 보정하는 접근을 다룬 논문 메모. |
| 2025-04-17 | [Reframing Demand Forecasting: A Two-Fold Approach for Lumpy and Intermittent Demand](https://zzongzz.tistory.com/8) | 간헐적이고 불규칙한 수요를 다루는 논문과 Croston, SBA 등 관련 방법 정리. |
| 2025-03-26 | [Bombardier Aftermarket Demand Forecast with Machine Learning](https://zzongzz.tistory.com/2) | 항공기 부품 수요를 ADI와 CV²로 분류하고 유형별 예측 방법을 살펴본 사례. |

## 예측과 재고관리

| 작성일 | 글 | 다룬 내용 |
|---|---|---|
| 2025-12-03 | [Forecast accuracy and inventory performance: Insights on their relationship from the M5 competition data](https://zzongzz.tistory.com/13) | 예측오차와 재고비용·서비스 수준의 관계, 목표 재고수준까지 보충하는 정책과 안전재고 설정. |
| 2025-12-09 | [Optimizing inventory control through a data-driven and model-independent framework](https://zzongzz.tistory.com/15) | 수요 특성과 보충 정책 변수를 바탕으로 재고 성과를 근사하고 정책을 탐색하는 접근. |

## 연구 구상

| 작성일 | 글 | 구상한 내용 |
|---|---|---|
| 2025-12-04 | [하고 싶은 거... 정리(12/7 수정)](https://zzongzz.tistory.com/14) | ADI·CV² 외의 특성으로 수요를 세분화하고, 그룹별 예측 모형과 안전재고를 재고 성과로 비교하는 방향. |

이 글은 **검증 전 연구 아이디어**입니다. 완료한 실험이나 성과와 구분해 수록했습니다.

## 프로젝트와 함께 읽기

| 프로젝트에서 살펴볼 내용 | 관련 공부 기록 |
|---|---|
| 품목군별 예측 모형과 기준선 비교 | 단순 시계열 모형, 시계열 분해와 지수평활, ARIMA·SARIMA |
| 예측 판매량을 안전재고와 매입량에 연결하는 과정 | 예측 정확도와 재고 성과의 관계, 데이터 기반 재고관리 |
| 이후 확장해 볼 문제 | 수요 유형 분류, 간헐수요 예측, 그룹별 재고 정책 |

위 글은 개념 학습과 논문을 읽으며 남긴 기록입니다. 소개한 방법을 모두 이 프로젝트에 적용한 것은 아니며, 실제 분석 범위와 결과는 [코드 안내](../code/README.md)와 [제출 보고서](../reports/nexus_demand_forecasting_report.pdf)에서 확인할 수 있습니다. 논문 관련 설명은 블로그의 읽기 메모이며, 정확한 수식과 실험 조건은 각 글에서 다룬 원문을 기준으로 확인합니다.

## 새 글을 추가할 때

주제에 맞는 표에 **작성일, 원문 제목과 링크, 한 줄 요약**을 추가하면 됩니다. 연구 아이디어는 실험을 마친 뒤 결과가 담긴 코드나 보고서 링크를 함께 연결합니다.

정리 기준: 2026-11-06 · 티스토리 공개 글 14편

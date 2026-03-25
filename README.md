# 🚇 미세먼지 및 강수량에 따른 지하철 유동인구 분석
![Python](https://img.shields.io/badge/Python-3.x-blue.svg) ![Jupyter Notebook](https://img.shields.io/badge/Jupyter-F37626.svg?&logo=Jupyter&logoColor=white) ![Pandas](https://img.shields.io/badge/Pandas-150458.svg?&logo=Pandas&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-3F4F75.svg?&logo=Python&logoColor=white)

## 🌈 팀명: TMI
**T**oday **M**l세먼지 **I**nformation

## 📌 프로젝트 요약
* **분석 목적:** 대기질과 강수량이 서울 핵심 상권의 지하철 유동인구에 미치는 영향 파악
* **핵심 결과:** 미세먼지 수준 단일 변수만으로는 유동인구 변화를 설명하기 어려움
* **결론:** 현대인의 주말 유동인구는 대기질보다 뚜렷한 목적성과 복합적인 환경 요인에 더 큰 영향을 받음

## 📊 활용 데이터
| 데이터셋 | 데이터 출처 | 활용 목적 |
| :--- | :--- | :--- |
| **서울시 역별 승하차 인원** | [서울 열린데이터 광장](https://data.seoul.go.kr/dataList/OA-12914/S/1/datasetView.do) | 6대 핵심 상권(강남, 홍대 등) 유동인구 지표 |
| **서울시 일평균 대기환경** | [서울 열린데이터 광장](https://data.seoul.go.kr/dataList/OA-2220/S/1/datasetView.do) | 미세먼지(PM10) 농도 독립 변수 수집 |
| **서울시 강수량 정보** | [기상청 기상자료개방포털](https://data.kma.go.kr/stcs/grnd/grndRnList.do?pgmNo=69) | '비' 변수 통제 (강수량 1.0mm 이하만 추출) |

## ⚙️ 분석 파이프라인
1. **데이터 통합:** 인코딩이 혼재된 여러 승하차, 대기환경, 강수량 CSV 파일을 하나의 마스터 데이터로 병합
2. **전처리:** 타겟 상권과 자치구 측정소를 1:1 매핑하고, 외부 노이즈 차단을 위해 '맑은 주말' 데이터만 필터링
3. **범주화:** 연속형 변수인 미세먼지 농도를 환경부 기준 '좋음/보통/나쁨'으로 등급화
4. **시각화:** 롤리팝 차트를 활용해 PM 등급별 유동인구 규모 직관적 비교

## 🌱 회고 및 향후 다짐
**데이터 정리 능력** <br>
서로 다른 공공데이터를 하나로 합치는 과정을 통해,<br> 
어떤 데이터가 주어져도 분석하기 좋게 정리하는 기초 체력을 길렀음.

**협업을 위한 코드 작성** <br>
환경에 상관없이 어디서든 잘 돌아가는 코드를 짜며,<br>
동료들이 바로 가져다 쓸 수 있는 편리한 분석 환경을 만드는 데 기여함.

**실전 분석가로의 성장** <br>
분석의 한계를 스스로 찾아보고 보완하는 태도를 바탕으로,<br>
실제 의사결정에 도움을 주는 분석가로 성장하겠음.

# 여행지 추천 AI
이 리포지터리는 AI hub의 [국내 여행로그 데이터(수도권)](https://www.aihub.or.kr/aihubdata/data/view.do?dataSetSn=71581)를 이용한 추천 서비스 구현용 AI 모델을 학습시키는 코드를 저장하고 있습니다.  
## 목적
본 프로젝트의 목적은 지난 2023년 11월부터 12월에 걸쳐 진행된 엔코아 데이터 엔지니어 양성 코스의 파이널 프로젝트(https://github.com/DJMLteam2/DP_Service)에서의 부족한 점을 보완하기 위함입니다. 당시 최종적으로는 추가 데이터의 크롤링 및 학습 과정을 Airflow로 자동화하기 위해 [대한민국 구석구석](https://korean.visitkorea.or.kr/main/main.do)의 데이터를 사용했으나, 데이터 선정 과정 중 후보로 올랐던 AI-Hub의 데이터를 이용해 당시 프로젝트에 *사용할 수도 있었던* 모델들을 추가로 학습하고 검증하고자 합니다.

## 데이터 구성
![국내여행로그데이터수집_ERD.png](https://www.aihub.or.kr/web-nas/aihub21/files/editor/2023/07/36ef970d172040699271937b73aeecef.png)  
> 출처: 국내 여행로그 데이터(수도권)(https://www.aihub.or.kr/aihubdata/data/view.do?dataSetSn=71581) - 어노테이션 포맷 및 데이터 구조  

이 프로젝트에서는 링크에서 제공하는 전체 데이터 중 Training - 원천데이터 - TS_csv.zip의 파일들을 사용합니다. 필요에 따라 해당 폴더의 csv 파일 중 일부 또는 전체를 불러와서 분석 및 모델 학습에 사용합니다.  
자세한 내용은 출처의 링크에서 '어노테이션 포맷 및 데이터 구조' 칸을 참고하세요.
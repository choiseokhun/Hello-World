빅데이터 이해와 분석 프로젝트

이 저장소는 정신건강 서비스 이용 현황과 지역별 취약지역 분석을 위한 빅데이터 이해 및 분석 과정을 담고 있습니다. 데이터 수집부터 전처리, 탐색적 분석, 모델링, 시각화, 그리고 발표 자료까지 포함되어 있습니다.

주요 기능 및 구성

source:
- 찐막.xlsx: 전국 정신병원 분포와 위/경도가 포함된 엑셀 데이터셋
- sig.dbf, sig.shp: 전국 시군구단위 선 지도 및 지오데이터 파일
- 시군구_인구밀도.xlsx: 전국 시군구단위 인구밀도 및 지오데이터 파일
- 전국 법정동.csv: 시군구 코드 <-> 지오데이터 변환을 위한 메타데이터
- 한국 시군구 지역코드.xlsx: 반복 누락되는 지역들의 데이터들을 따로 모아놓은 엑셀 파일
- GDRP.xlsx: 시군구 단위 GDP 계산을 위한 지역별 총생산 데이터

notebooks/Main.ipynb: 데이터 준비, 탐색, 시각화 코드 및 분석 모델 구축 과정이 포함된 Jupyter Notebook
설치 및 실행

저장소 복제

git clone https://github.com/<choiseokhun>/bigdata-mental-health.git
cd bigdata-mental-health

가상환경 생성 및 활성화

python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

의존성 설치

pip install -r requirements.txt

노트북 실행

jupyter notebook notebooks/Main.ipynb

스크립트 실행 예시

python scripts/visualization.py --input data/population_economy.csv --output maps/overview.html
python scripts/modeling.py --method regression

Git 커밋 상태

* 3f5a2c1 (HEAD -> main) Add regression analysis in modeling.py
* 1b9d7e4 Update visualization.py with Folium map tooltips
* 7cd8a9f Add initial notebook and data preprocessing steps
* e5a3f00 Project structure 및 README 초안 작성

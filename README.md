빅데이터 이해와 분석 프로젝트

이 저장소는 정신건강 서비스 이용 현황과 지역별 취약지역 분석을 위한 빅데이터 이해 및 분석 과정을 담고 있습니다. 데이터 수집부터 전처리, 탐색적 분석, 모델링, 시각화, 그리고 발표 자료까지 포함되어 있습니다.

주요 기능 및 구성

data/: 공공데이터포털에서 수집한 CSV 원본 데이터

service_usage.csv (정신병원 진료인원 및 이용자 수)

facility_status.csv (정신건강 관련 기관 설치 현황)

population_economy.csv (시도별 인당 소득 및 지역내총생산)

notebooks/Main.ipynb: 데이터 준비, 탐색, 시각화 코드 및 분석 모델 구축 과정이 포함된 Jupyter Notebook fileciteturn1file0

scripts/visualization.py: Folium 지도 및 인구 밀도, 정신병원 위치 시각화 코드

scripts/modeling.py: 군집 분석 및 회귀분석 모델링 코드

docs/: 프로젝트 문서

presentation/빅데이터 이해와 분석 발표 초안.pptx (발표 자료) fileciteturn1file1

design.md (분석 설계 및 개념 설명)

requirements.txt (필요 라이브러리 목록)

.github/: GitHub 워크플로우 및 이슈 템플릿

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

문서

분석 설계(docs/design.md): 핵심 기술 및 분석 흐름 설명

발표 자료(docs/presentation/빅데이터 이해와 분석 발표 초안.pptx)

요구사항 목록(docs/requirements.txt)

기여

이슈 생성

브랜치 생성 (git checkout -b feature/your-feature)

변경 사항 커밋 (git commit -m 'Add your feature')

브랜치 푸시 (git push origin feature/your-feature)

풀 리퀘스트 생성

라이선스

MIT 라이선스

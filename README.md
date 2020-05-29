# A_TCL
20년 advanced TCL

EDA 시 고려할 수 있는 방법들
Train , Test 6시 탑승 인원 컬럼 값.
- ID, 날짜, 버스 노선 ID, 이에 따라 탑승 인원의 패턴.
- 값이 없을 때 평균 값을 넣었는데, 다른 방법의 통계 값을 넣어보자
- 1등 코드는 RF, 우리는 다양한 방법 (Boosting Bagging, 자동 Feature 추출 등)
- user category(bus_bts) 활용할 수 있는 컬럼, 정류장 이름 시 학교,아파트를 카테고리화 시켜 label
- 정류장 별로 user category를 매핑하여 변수 추가 가능
- 탄곳 내린곳, get on - get off의 관계
- 날씨 데이터 온도, 강수량 - 추가적으로 끌고올 수 있음.
- 날씨 별로 category화시켜 데이터 활용 가능
- 다른 방법의 통계 값 : 여봉룡선임, 정민경 선임
- get on - get off의 관계, 정류장 카테고리화 : 한승민 선임.
- 정류장 별로 user category를 매핑하여 변수 추가, 외부데이터 맛보기 : 이정미선임
- DB랑 aws 서버 구축 : 방현진 선임


<Data 분석>

- 주요변수 추출(수치형 데이터) 그룹핑 후 새로운 데이터 발생 - 여봉룡 선임
 --> 범주형 변수 추가 후 새로운 데이터를 조합하는 식의 방향
 
- 기초 통계량 데이터 발생 - 정민경 선임
 --> bus_bts, train 데이터 통합 방법
 
- 날짜 별 날씨 데이터 생성 - 이정미 선임
 --> 날씨데이터와 DataSet간의 연관관계 분석 및 그룹핑 작업
 
- 정류장 카테고리화 데이터 생성 - 한승민 선임
 --> ??
- 전체 : N/A값을 처리하는 좋은 방법 고민 필요

<AWS 설정> (방현진선임)

- EC2, RDS(DB) 설정 완료. --> DB에 table 생성 완료
- aws sagemaker를 통해 git 연동 완료.
- sagemaker를 통해 S3(하드디스크)에 데이터 셋 저장 및 불러오기 가능하도록 구조 설정 필요
- sagemaker를 통해 개발 환경 공유할 수 있도록 구조 설정 필요

# develop-preparation

+ open api 사용한 프로젝트 2개 배포해보자
  
+ 프로젝트 1 - 로그인 있는거 (redux / MUI / SNS login / localstorage / 반응형 / d3js)

# 아키텍처
+ database : serverless?
+ db 콜 => 비용
> 돈을 사용하지 않고 에러 처리 : 클라이언트-> 서버 단에서 확인
+ serverless : 비용 절가 및 대용량 auto scaling - lambda 
+ rds 추세  인스턴스 aws rds aurora serverless v2 (최소비용 4만원)

+ 아키텍처 및 배포 방식 고민 - 비용!! & 성능

aws 엘라스틱 서치 등등
railway render cloudtype 무료 (비즈니스 실패) 

ec2 / rds -> 월 7만원 : 비용을 어떻게 줄일 수 있을까?
-> aws apprunner (ip 고정 x) ecr container github action
& amplify

lambda 메모리? 컴퓨팅 파워? 
apprunner 비용
천건, 만건 성능이 받춰줄까? 비용 감당 가능할까? 서비스 매출이 서버 비용을 감당할 수 있을까?

서비스가 배포되었을 때 비용이 얼마가 발생할지 예상해보자

선택지 > 장단점 > 결론

# 시퀀스 다이어그램
react / express / db
db : 데이터 들어오는거 query parameter, path parameter 검증 (json - schema) ip 확인, 쿠키, 헤더, api 확인 : if문, 라이브러리 활용 
& 필히 나가는 거 검증 

# 클래스 다이어그램

# 성능테스트
postman load testing, heys, insomnia
간단하게 확인 
-> 무료로 insomnia load testing 사용해보자
에러율, sql 병목 확인 및 수정

# json - schema

# spring-boot-test

sampleCode 는 간단한 spring-boot 코드 입니다.

<테스트 작업 진행>
1. sampleCode 를 maven build -> jar 파일로 만든 후 개인 nexus repository 에 배포

2. 컨테이너 안에서 wget 으로 개인 nexus repository 에 배포한 jar 파일을 다운로드
<br></br>
wget --user=<계정아이디> --password=<비밀번호> "http://<로컬ip>:8081/repository/maven-3rdparty/com/example/demo/0.0.1-SNAPSHOT/demo-0.0.1-SNAPSHOT.jar" -O /root/demo-0.0.1-SNAPSHOT.jar

3. jar 파일 실행 
*** java -jar demo-0.0.1-SNAPSHOT.jar

4. NodePort 로 연결

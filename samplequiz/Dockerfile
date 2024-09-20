# Ubuntu 20.04 이미지 사용
FROM ubuntu:20.04

# 패키지 목록 업데이트 및 OpenJDK 17 설치
RUN apt update
RUN apt install -y openjdk-17-jdk

# JAR 파일을 컨테이너에 복사
COPY webprac.jar app.jar

# 애플리케이션 실행
ENTRYPOINT [ "java", "-jar", "/app.jar" ]

EXPOSE 7878

# intellij에서 gradle > build > bootJar 클릭해서 .jar 생성
# 프로젝트 폴더 > build > libs > 안에 있는 .jar 파일을 이 폴더(samplequiz)에 넣기

# docker build -t myjavaapp .
# docker run -d -p 7878:8888 --name myjavaapp-container myjavaapp
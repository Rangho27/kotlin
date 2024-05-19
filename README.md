<br/>
<br/>

<p align="center">
<img src="https://files.cloudtype.io/logo/cloudtype-logo-horizontal-black.png" width="50%" alt="Cloudtype"/>
</p>

<br/>
<br/>

# Kotlin - Spring Boot

Kotlin으로 작성된 Spring Boot 어플리케이션 템플릿입니다.
## 🖇️ 준비 및 확인사항

### 지원 JDK 버전
- 8, 11, 17, 18, 19
- Spring Boot 버전별 필요 Java 사양
    - Spring Boot 3.x: Java 17 이상
    - Spring Boot 2.x: Java 8 이상
- `build.gradle` 내의 설정과 클라우드타입에서 배포시 설정한 JDK 버전이 다른 경우 정상적으로 서비스가 실행되지 않을 수 있으니 사전에 확인해주세요.
  ```groovy
  tasks.withType(KotlinCompile) {
    kotlinOptions {
	    freeCompilerArgs = ['-Xjsr305=strict']
	    jvmTarget = [JDK 버전]
   }
  ```
- ⚠️ 로컬/테스트 환경과 클라우드타입에서 설정한 Node 버전이 상이한 경우 정상적으로 빌드되지 않을 수 있습니다.


### 패키지 명세
- 빌드 시 어플리케이션에 사용된 패키지를 설치하기 위해서는 `build.gradle` 혹은 `pom.xml` 파일에 올바르게 내용이 작성되어 있어야 합니다.


## 🏷️ 환경변수

- `SPRING_PROFILES_ACTIVE`: 배포 프로필 설정
- `TZ`: 타임존 설정


## 💬 문제해결

- [클라우드타입 Docs](https://docs.cloudtype.io/)

- [클라우드타입 FAQ](https://help.cloudtype.io/guide/faq)

- [Discord](https://discord.gg/U7HX4BA6hu)


## 📄 License

[Apache-2.0](https://github.com/spring-projects/spring-boot/blob/main/LICENSE.txt)

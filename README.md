# Cinemacloud

**Cinemacloud Web OTT Service v1.0**

![Cinemacloud Image](./images/mainImage.png)
[시네마클라우드](https://github.com/juseungpark97/FinalProject)

**개발 기간**: 2024.08 ~ 2024.09

## 버전 정보

- **JDK**: Amazon Corretto 17  
  [다운로드 링크](https://docs.aws.amazon.com/ko_kr/corretto/latest/corretto-17-ug/downloads-list.html)
  
- **Spring Boot**: 3.3.2  

- **Spring Tool Suite (STS)**: 4.24.0.RELEASE  
  [다운로드 링크](https://spring.io/tools)

- **SQL Developer**: 23.1.1.345  
  [다운로드 링크](https://www.oracle.com/database/sqldeveloper/technologies/download/)

- **Database**: Oracle Database 21c Express Edition Release 21.0.0.0.0 - Production Version 21.3.0.0.0  
  [다운로드 링크](https://www.oracle.com/database/technologies/xe-downloads.html)

- **Lombok**: 1.18.32  
  [다운로드 링크](https://mvnrepository.com/artifact/org.projectlombok/lombok/1.18.32)

- **Node.js**: v20.15.1  
  [다운로드 링크](https://nodejs.org/en)

- **React**:  
  - 프로젝트 생성: `npx create-react-app my-app` (my-app 이름은 자유롭게 설정 가능)
  - HTTP 클라이언트 설치: `npm install axios`
  - 스타일 라이브러리 설치: `npm install styled-components`
  - 페이지 라우팅 라이브러리 설치: `npm install react-router-dom`
  - 빌드: `npm run build` (배포 시 사용)
  - `node_modules`는 공유 시 제외하여 용량 문제 방지
  - 부트스트랩 패키지 설치: `npm install --save bootstrap`
  - 리액트스트랩 패키지 설치: `npm install --save reactstrap`

## 웹개발팀 인원(총 6명)

- 박주승, 이주빈, 오민혁, 이은호, 유승혁, 송용하

## 프로젝트 소개

**Cinemacloud**는 다양한 OTT 서비스를 제공하는 웹 애플리케이션으로, 사용자 맞춤형 콘텐츠 추천, 구독 관리, 멀티 프로필 설정 등 다양한 기능을 지원합니다.

### 주요 기능

- **회원가입 및 로그인**
  - JWT 기반 인증 시스템
  - 카카오 API를 이용한 소셜 로그인
- **아이디 및 비밀번호 찾기**
  - SMS 인증을 통한 아이디/비밀번호 찾기
- **영상 업로드**
  - 사용자가 직접 영상 콘텐츠를 업로드
- **구독 기능**
  - 페이팔 연동을 통한 구독 관리
- **멀티 프로필**
  - 하나의 계정에 여러 프로필 설정 가능
- **영상 슬라이더**
  - 메인 화면에서 인기 콘텐츠를 슬라이드 형식으로 제공
- **개인 맞춤 추천 알고리즘**
  - 사용자 선호도를 분석해 맞춤형 콘텐츠 추천
- **관리자 페이지**
  - 콘텐츠 관리, 사용자 관리, 통계 대시보드

### 사용된 기술 스택

- **프론트엔드**:
  - ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
  - ![Axios](https://img.shields.io/badge/Axios-5A29E4?style=flat-square&logo=axios&logoColor=white)
  - ![Styled Components](https://img.shields.io/badge/Styled--Components-DB7093?style=flat-square&logo=styled-components&logoColor=white)
  - ![React Router](https://img.shields.io/badge/React_Router-CA4245?style=flat-square&logo=react-router&logoColor=white)
- **백엔드**:
  - ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white) (프레임워크로 사용, 자체 서버)
  - JWT 기반 인증
  - Kakao API, PayPal API, GoogleSMS, AWS API, 
- **데이터베이스**:
  - ![OracleDB](https://img.shields.io/badge/OracleDB-F80000?style=flat-square&logo=oracle&logoColor=white)
- **개발 환경**:
  - ![JDK](https://img.shields.io/badge/Java-11-007396?style=flat-square&logo=java&logoColor=white)
  - ![Spring Tool Suite](https://img.shields.io/badge/STS-4.24.0.RELEASE-6DB33F?style=flat-square&logo=spring&logoColor=white)
  - ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
- **서버**:
  - ![Spring Boot 자체 서버](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white)
  - ![Amazon EC2](https://img.shields.io/badge/Amazon%20EC2-FF9900?style=flat-square&logo=amazon-aws&logoColor=white)
  - ![Amazon S3](https://img.shields.io/badge/Amazon%20S3-569A31?style=flat-square&logo=amazon-aws&logoColor=white)
  - ![Amazon RDS](https://img.shields.io/badge/Amazon%20RDS-527FFF?style=flat-square&logo=amazon-aws&logoColor=white)

### 사용된 API

- Kakao Login API
- PayPal API

## 프로젝트 설정 및 실행 방법

### 프로젝트 Import

1. `import -> Maven -> Existing Maven Projects -> FINALPROJECT(루트폴더)` 선택.

### 포트번호 변경

1. `package.json` 파일의 `scripts` 부분 변경:
   ```json
   "start": "set PORT=3002 && react-scripts start"

### 포트 중복 문제 해결

- 포트 확인: `netstat -a -o`
- 프로세스 종료: `taskkill /f /pid <PID 번호>`

### 기본 개념

- **JDK (Java Development Kit):** Java 애플리케이션 개발을 위한 도구 모음으로, 컴파일러, 표준 라이브러리, 실행 환경 등을 포함합니다.
- **Spring Boot:** 스프링 프레임워크를 기반으로 한 자바 웹 애플리케이션 개발 프레임워크로, 빠르고 간편한 설정을 제공합니다.
- **Spring Tool Suite (STS):** Spring 애플리케이션 개발을 위한 통합 개발 환경(IDE)입니다.
- **SQL Developer:** Oracle에서 제공하는 데이터베이스 관리 도구로, SQL 쿼리 작성, 데이터베이스 관리, 데이터 모델링 등을 지원합니다.
- **Oracle Database:** 오라클에서 제공하는 관계형 데이터베이스 관리 시스템(RDBMS)입니다.
- **Lombok:** 자바에서 반복적으로 작성해야 하는 코드를 자동으로 생성해주는 라이브러리로, 생산성을 높여줍니다.
- **Node.js:** JavaScript 런타임 환경으로, 서버 사이드 애플리케이션을 개발할 때 사용됩니다.
- **npm (Node Package Manager):** Node.js의 기본 패키지 관리자입니다. Node.js 패키지를 설치하고 관리하는 도구입니다.
- **React:** 사용자 인터페이스를 구축하기 위한 JavaScript 라이브러리로, 컴포넌트 기반의 개발 방식을 제공합니다.
- **Axios:** HTTP 클라이언트 라이브러리로, 브라우저와 Node.js에서 모두 사용할 수 있습니다.
- **styled-components:** CSS-in-JS 라이브러리로, JavaScript 파일 내에서 CSS를 작성할 수 있게 해줍니다.
- **react-router-dom:** React 애플리케이션에서 여러 페이지를 구현하기 위한 라이브러리입니다.

### 담당 기능
 - **aws S3 업로드 및 다운로드**
![HomePage](./images/homePage.png)
### 주요 기능
- **비디오 및 썸네일 업로드**: 사용자가 업로드한 비디오 파일과 썸네일 이미지를 Amazon S3에 업로드합니다.
- **S3 URL 생성 및 Movie 객체 생성**: 업로드된 파일의 URL을 가져와 Movie 객체를 생성하고 데이터베이스에 저장합니다.
### 코드 예시
```java
@Service
@RequiredArgsConstructor
public class MovieService {
    private final AmazonS3 amazonS3;
    private final MovieRepository movieRepository;

    @Value("${aws.s3.bucketName}")
    private String awsS3BucketName;

    public Movie uploadMovie(MultipartFile file, MultipartFile thumbnail, String title, String director,
                             String cast, int releaseYear, String synopsis, float rating, String tags) throws IOException {
        // S3 키 설정
        String videoKey = "movies/" + file.getOriginalFilename();
        String thumbnailKey = "thumbnail/" + thumbnail.getOriginalFilename();

        // S3에 비디오 및 썸네일 파일 업로드
        amazonS3.putObject(new PutObjectRequest(awsS3BucketName, videoKey, file.getInputStream(), new ObjectMetadata()));
        amazonS3.putObject(new PutObjectRequest(awsS3BucketName, thumbnailKey, thumbnail.getInputStream(), new ObjectMetadata()));

        // URL 생성
        String videoUrl = amazonS3.getUrl(awsS3BucketName, videoKey).toString();
        String thumbnailUrl = amazonS3.getUrl(awsS3BucketName, thumbnailKey).toString();

        // Movie 객체 생성 및 데이터 설정
        Movie movie = new Movie();
        movie.setTitle(title);
        movie.setUrl(videoUrl);
        movie.setThumbnailUrl(thumbnailUrl);
        movie.setTagList(Arrays.asList(tags.split(",")));
        movie.setCastList(Arrays.asList(cast.split(",")));

        return movieRepository.save(movie);
    }

    // 필터별 검색 기능
    public List<Movie> findMoviesByGenre(String genre) {
        return movieRepository.findByGenre(genre);
    }

    public List<Movie> findMoviesByTag(String tag) {
        return movieRepository.findByTagsContaining(tag);
    }

    public List<Movie> findMoviesByCast(String cast) {
        return movieRepository.findByCastContaining(cast);
    }
}



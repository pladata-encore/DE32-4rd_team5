# 🎬 영화 조회 웹 애플리케이션

## 개요
이 애플리케이션은 Java Spring Framework와 영화진흥위원회 영화 목록 API를 사용하여 영화 정보를 조회할 수 있는 웹 애플리케이션입니다. 
<br></br>

## 목차
- [기술스택](#기술스택)
- [기능 흐름도](#기능-흐름도)
- [데이터베이스 구조](#데이터베이스-구조)
- [사용방법](#사용방법)
- [시연](#시연)
- [회고](#회고)
<br></br>

## 기술스택
<img src="https://img.shields.io/badge/java-007396?style=for-the-badge&logo=java&logoColor=white"> <img src="https://img.shields.io/badge/springboot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"> <img src="https://img.shields.io/badge/Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white"> <img src="https://img.shields.io/badge/Thymeleaf-005F0F?style=for-the-badge&logo=thymeleaf&logoColor=white">
- API
  - RESTful API
  - 영화진흥위원회 영화 목록 API
<br></br>

## 기능 흐름도
![image](https://github.com/user-attachments/assets/501e185e-a51a-4a71-a378-14553393a561)

<br></br>

## 데이터베이스 구조
```sql
+-------------+-------------+------+-----+---------+----------------+
| Field       | Type        | Null | Key | Default | Extra          |
+-------------+-------------+------+-----+---------+----------------+
| ID          | int(11)     | NO   | PRI | NULL    | auto_increment |
| movieCd     | int(11)     | YES  |     | NULL    |                |
| movieNm     | varchar(50) | YES  |     | NULL    |                |
| movieNmEn   | varchar(50) | YES  |     | NULL    |                |
| openDt      | date        | YES  |     | NULL    |                |
| repGenreNm  | varchar(10) | YES  |     | NULL    |                |
| repNationNm | varchar(20) | YES  |     | NULL    |                |
| peopleNm    | varchar(30) | YES  |     | NULL    |                |
+-------------+-------------+------+-----+---------+----------------+
```
<br></br>

## 사용방법
```bash
$ git clone git@github.com:DE32-4-team5/movis.git
$ docker compose up -d --force-recreate --build
```
조회 사이트 Url : http://3.35.137.110:8080/
<br></br>

## 시연
### 웹 화면
<img src="https://github.com/user-attachments/assets/01f00478-9703-47a1-8130-608e795537a2" alt="이미지 설명" width="60%" height="60%">

### 조회 결과
<img src="https://github.com/user-attachments/assets/d7f6c800-a8ec-4f24-80c6-92ccb473ea88" alt="이미지 설명" width="50%" height="50%">

## 회고
### 좋은 점
- 초반에 진행한 영화 API와 Airflow를 복습하며, Spring Boot를 DB에 연결하고 Docker Compose를 통해 하나의 애플리케이션으로 동작시키는 방법을 다시 배울 수 있었다.
- 빠른 의사결정과 단순화된 목표 덕분에 기한 내에 프로젝트를 일정 수준 완성할 수 있었고, API 통신 및 CSV 파일을 DB에 입력하는 다양한 방법을 시도하면서 SQL 쿼리 학습의 기회를 가졌다.
- 프로젝트에 관한 원활한 소통과 열정 덕분에 기한 내에 프로젝트가 빠르게 진행 되었다.
### 아쉬운 점
- 짧은 기한으로 인해 목표가 단순화되면서 프로젝트가 너무 간단해졌다는 느낌을 받았다. 
- Java 코드를 읽을 줄은 알지만 작성하는 데 어려움이 있었고, Spring Boot 구조에 대한 이해가 부족하다고 느꼈다.
### 개선할 점
- 제한된 기한 내에도 다양한 기능을 추가할 수 있는 역량을 키워야 한다.
- Java 언어와 Spring Boot 구조에 대한 추가 학습을 통해 더 많은 기능을 구현할 수 있도록 학습해야 한다.
<br></br>

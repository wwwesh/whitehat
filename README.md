# Drupal Cross-Site Scripting by File Upload (CVE-2019-6341)
> 화이트햇 스쿨 3기 - 전소현


### 요약
- Drupal은 2000년도에 등장한 PHP 기반 콘텐츠 관리 프레임워크
- 파일 모듈이나 서브 시스템을 통해 악성 파일을 업로드함으로써 XSS 취약점 발생
<br/><br/> 
### 환경 구성 및 실행 
- docker compose up -d 를 실행하여 테스트 환경을 실행
- your-ip:8000 에 접속하여 drupal 설치
- php blog-poc.php your-ip 8080 을 실행하여 파일 업로드 
- your-ip:8080/sites/default/files/pictures/YYYY-MM 에 접속하면 XSS 취약점 발생
<br/><br/>  
### 결과
![image](https://github.com/user-attachments/assets/b776e8b7-760d-4e94-8ce4-bb2f50eaa870)

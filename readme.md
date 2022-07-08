# 크롤링 및 NBP 함수 사용하여 결과값 도출하는 REST API

## 프로젝트 실행 방법(순서대로 진행하기)

### 1. 레퍼지토리 클론
    git clone https://github.com/OIDC-JT/NBP_back.git

### 2. 가상환경 실행
    source myvenv/Scripts/activate

### 3-a. 라이브러리 설치
    pip install -r requirements.txt

### 3-b. reqirements.txt로 필요한 라이브러리 설치가 안된다면
    pip install django
    pip install djangorestframework
    pip install django-cors-headers
    pip install beautifulsoup4
    pip install rest_framework_simplejwt
    pip install pymysql

### 4. 프로젝트 폴더 위치로 이동 (manage.py 파일이 있는 위치)
    cd cloud

### 5. DB 마이그레이션
    python manage.py makemigrations
    python manage.py migrate

### 6. 서버 실행
    python manage.py runserver

### 127.0.0.1:8000 으로 접속

### 입력값 - POST 메소드 사용
ex.
    {
        "list": [1,2,3,4]
    }

![캡처1](https://user-images.githubusercontent.com/37846235/177045385-75a25c02-b7cf-48f3-8a44-4ddb3fc24d3d.JPG)

### 결과값

![캡처2](https://user-images.githubusercontent.com/37846235/177045404-21c445e9-686b-45fd-aa4e-07b5e4208737.JPG)
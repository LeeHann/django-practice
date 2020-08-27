<윈도우에서 가상환경 만들기>

1. python 설치
https://www.python.org/downloads/

2. 가상환경을 사용할 폴더 만들기

3. cmd에서 환경 설정

1) 버전 확인
py -3 -V

2)가상환경 설정
pip3 install virtualenvwrapper-win

3)가상환경 생성
mkvirtualenv (가상환경 이름)
혹은 python -m venv (가상환경 이름)

4)가상환경 활성화
만들어진 가상환경 폴더로 들어가서
Scripts\activate.bat
-가상환경 비활성화 : deactivate
=>(가상환경 이름) 으로 프롬프트가 실행되면 가상환경이 돌아가는 것.

<Django project>
참고 장고걸스 튜토리얼 https://tutorial.djangogirls.org/ko/


1. 장고 사이트 파일 생성
django-admin startproject (사이트 폴더 이름)
cd (사이트 폴더 이름)

2. 설정 변경
사용자 임의로 변경

3. 웹서버 실행
python3 manage.py runserver
=> IP주소가 나오고 그 주소를 따라 들어가면 생성된 웹 서버를 볼 수 있다.

<블로그 생성 과정>
1. python manage.py startapp blog

2. settings.py를 열어 INSTALLED_APPS 안에 'blog' 추가

3. blog/models.py를 열어 블로그 모델 설정

4. python manage.py makemigrations blog

5. python manage.py migrate blog

6. admin.py 파일 설정
python manage.py runserver 웹서버 실행
 http://127.0.0.1:8000/admin/ 서버 확인
python manage.py createsuperuser 슈퍼사용자 생성
- Username, Email address, Password 작성


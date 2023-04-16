# Flask_Test

플라스크 프로젝트 생성 및 간단 테스트
vscode 내의 wsl 터미널 사용

### WSGI를 이용하라고 경고문 뜸
export FLASK_APP=test.py (app이라는 프로젝트 내의 test.py)
flask run --host=0.0.0.0 

### Gunicorn 설치 후 바인딩
gunicorn app:test --bind 0.0.0.0:8000

## 기본 페이지 이동 테스트

### templates 폴더 생성 후 렌더링 파일 관리

template 폴더 안에 있는 fortune.html 렌더링이 가능한지 확인

@app.route('/fortune') 요청명

이후 / 요청으로 home.html로 되돌아가기 테스트


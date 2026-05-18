[vsCode GIT 연동]

# 초기 설정
1. 사용자 정보 설정
1) git config --global user.name "본인 이름"
2) git config --global user.email "깃허브 계정 이메일"

2. .gitignore 생성
e.g. cd /home/back4jo2/FastAPI → cat > .gitignore << 'EOF' → .env → venv/
→ __pycache__/ → *.pyc → *.pyo → captures/ → EOF

3. 초기화 및 원격 저장소 연결
1) git init
2) git remote add origin "원격 저장소 주소" (e.g. https://github.com/RoadAeye/Road_A_Eye.git)

4. 브랜치 전환
1) git fetch origin
2) git checkout "브랜치명"

# 작업 시작 전
1. git checkout main
2. git pull origin main
3. git checkout -b "브랜치명" (※ 개인 브랜치가 존재할 경우, git checkout "브랜치명")

# 작업 완료 후
1. git add .
2. git commit -m "깃 컨밴션 : 작업 내용"
3. git push origin "브랜치명"

※ 새로운 라이브러리 설치 시 반드시 `pip freeze` 혹은 `package.json` 업데이트 확인
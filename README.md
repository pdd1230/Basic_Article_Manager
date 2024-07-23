# 1. Git 초기 설정 확인 및 변경

## 현재 설정 확인 (현재 설정된 모든 설정 값 출력/확인)

- git config --list

# 2. 사용자 정보 설정

- git config --global user.name "Your Name"
- git config --global user.email "your.email@example.com"
- 작업을 하기전 반드시 먼저 확인하고 본인의 닉네임과 이메일로 변경합니다
- 원격지 주소를 복사해 둡니다

# 3. 환경정리

- git init
- 원격저장소에 연결하기 위한 대기 상태입니다
- 이상태에서 탐색기를 살펴보면 '.git' 이라는 폴더가 생성됩니다.  모든 준비가 끝난 상태입니다
- git remote add origin https://github.com/pdd1230/Basic_Article_Manager.git (예시)
- 해당주소를 github에서 복사하고 붙혀넣기 (sHift + inset ,  다른 방법은 (ctrl + v) 적용 안됩니다) 

# 4. 'gitignore' 파일 설정

1. 프로젝트 루트 디렉토리로 이동
2. .gitignore 파일 생성  (구글 검색)
   
### 여기서는 vim 이용하는 방법 (Git Bash Here 사용을 전제로 함)

1. vim으로 .gitignore 파일 열기
'git bash here' 클릭 후, 아래를 입력. 파일이 존재하지 않으면 새로 생성됨

- vim .gitignore

2. Insert 모드로 전환
vim은 기본적으로 Normal 모드에서 시작합니다. 텍스트를 입력하려면 Insert 모드로 전환해야 합니다. i 키를 눌러 Insert 모드로 전환합니다.

3. 무시할(형상관리 안할) 파일 및 디렉토리 추가 
.gitignore 파일에 무시할 파일 및 디렉토리를 입력합니다
- 예) 이클립스 Java
- .settings
- .classpath
- .project
- bin

- 이상 4줄 입력
4. Insert 모드 종료
텍스트 입력이 완료되면 Esc 키를 눌러 Insert 모드를 종료하고 Normal 모드로 돌아갑니다.

5. 파일 저장 및 vim 종료
vim에서 파일을 저장하고 종료하려면 :wq를 입력하고 Enter 키를 누릅니다.
- :wq

# 5. 로컬 저장소에서 원격 저장소로 올릴때 필수 항목 (3가지)

- git status (선택 사항)    
- git add .
- git commit -m "메세지"
- git push origin master

# 6. 그밖에 push 오류가 나는 경우는 구글링 O
1. The request URL returned error : '403'
- git remote set-url origin origin https://github.com/pdd1230/Basic_Article_Manager.git (예시)
- 다시
- git push origin maser
  ![image](https://github.com/user-attachments/assets/313d1bb9-a9e0-4ddf-8a30-0c42b6138426)

- github 로그인 진행
- 정상 수행

2. 기타 다른 사항으로 인한 오류는 생략 ( 구글링 O)
- 예) 로컬저장소(2대 pc), 원격저장소(동일) 한 경우 작업은?






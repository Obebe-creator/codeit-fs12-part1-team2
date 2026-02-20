# Codeit FS12 Part1 - Team2 소개 페이지

팀원들의 개인 자기소개 웹페이지를 하나의 리스트로 정리한 프로젝트입니다.
<br>
<br>
<br>
<br>
##  프로젝트 소개

이 프로젝트는 코드잇(Codeit) 파트 1 과제에 해당하는 간단한 소개 페이지입니다.

각 팀원의 페이지에는 다음과 같은 내용이 포함되어 있습니다.

- 이름  
- 자기소개  
- 취미 / 한마디 등 개인 정보  


##  팀원

- 하성민 — 메인페이지 및 개인 페이지 개발
- 장민주 — 개인 페이지 개발
- 김남진 — 메인페이지 및 개인 페이지 개발 
- 김성현 — 메인페이지 및 개인 페이지 개발
- 윤소정 — 메인페이지 및 개인 페이지 개발

##  주요 기능

- 팀원 소개 페이지 링크 리스트 제공  
- 각 링크 클릭 시 개인 자기소개 웹페이지로 이동  
- HTML / CSS 기반의 정적 웹페이지  

##  이슈 사항 정리
<img width="1689" height="1378" alt="image" src="https://github.com/user-attachments/assets/70901cab-9774-43b8-9a0e-21a7f5d17428" />

### 1️⃣ git push 시 non-fast-forward 오류 발생
 ! [rejected] main -> main (non-fast-forward)
error: failed to push some refs
Updates were rejected because the tip of your current branch is behind its remote counterpart.

#### 📌 원인

- 원격 저장소(main 브랜치)에 이미 다른 팀원의 커밋이 존재
- 로컬 브랜치가 원격 브랜치보다 **뒤쳐진 상태**
- 즉, 원격 저장소와 로컬 저장소의 히스토리가 달라진 상태에서 바로 push를 시도했기 때문에 발생

Git은 **히스토리가 다른 상태에서 덮어쓰는 것을 방지**하기 위해 push를 거부함

#### 🛠 해결 방법

1. 먼저 원격 변경사항을 pull로 불러옴
2. 충돌 발생 시 충돌 파일을 수정함
3. add / commit / push 순서로 다시 원격 저장소에 push 진행

### 2️⃣ Pull 중 Merge Conflict 발생
CONFLICT (content): Merge conflict in index.html
Automatic merge failed; fix conflicts and then commit the result.

#### 📌 원인

- 같은 파일(index.html)을 여러 명이 동시에 수정
- Git이 자동으로 병합하지 못해 충돌 발생
- 서로 다른 코드가 같은 위치에 존재했기 때문

#### 🛠 해결 방법

1. 충돌 표시 확인
2. 불필요한 부분 정리 후 코드 수동 수정
3. 충돌 마커 삭제
4. 병합 완료 처리

### 3️⃣ git push 시 non-fast-forward 오류 발생
error: Pulling is not possible because you have unmerged files.
fatal: Exiting because of an unresolved conflict.

#### 📌 원인

- Merge Conflict가 해결되지 않은 상태에서 다시 pull 시도
- Git은 충돌이 해결되지 않으면 추가 작업을 허용하지 않음

#### 🛠 해결 방법

- 충돌 파일 수정
- git add로 해결 표시
- git commit으로 병합 완료

<img width="849" height="534" alt="image" src="https://github.com/user-attachments/assets/154624b7-69fb-47c0-bae7-d47a83cdfd70" />

### 4️⃣ 강제 push (--force) 사용
git push origin main --force

#### ⚠ 주의사항

- 원격 저장소의 기존 기록을 덮어쓸 수 있음
- 협업 프로젝트에서는 팀원 코드가 사라질 위험 존재
- 반드시 팀원과 상의 후 사용해야 함

##  기술 스택
- HTML  
- CSS

##  실행 방법

1. 저장소 클론
git clone https://github.com/Obebe-creator/codeit-fs12-part1-team2.git
2. 폴더 이동 후 index.html 브라우저 실행

##  시연

https://github.com/user-attachments/assets/5c446c43-f9cb-4944-b31b-ea5512c42a9d


##  느낀점
### 🧑 (팀장)김성현

> 

### 👩 김남진

> git pull 할 때 오류가 나서 강사님께 여쭤보니 주석까지 복사해서 오류가 난 것이었습니다.  
> 수업을 잘 들었다고 생각했지만 디테일한 부분에서 많이 부족하다고 느꼈고,  
> 복습을 더 해야겠다고 생각했습니다.


### 👩 윤소정

> 팀원분들과 처음으로 협업해볼 수 있어서 좋았고,  
> 메인페이지와 개인페이지를 개발하면서 HTML, CSS로 배웠던 내용을 직접 활용해볼 수 있어 의미 있었습니다.  
> 이론으로만 배우는 것이 아니라 GitHub를 사용하며 충돌을 직접 경험해볼 수 있어서 좋은 경험이었습니다.


### 🧑 하성민

> Git 충돌보다 제 부족함이 더 많이 느껴졌던 협업이었습니다.  
> 앞으로 더 열심히 복습해서 성장하겠습니다. 감사합니다!


### 🧑 장민주

> 


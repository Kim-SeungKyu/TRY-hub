# 도전 22.07.08
 mkdir
 ls -> cd -> touch -> code .
 vscode 작성
 hub에 방파기
 vscode를 hub에 push
 GIT BASH 열고 git clone + 주소 작성
 git init과 git clone은 시작할 때 한 번만
그 이후로는 git push/pull origin master로 hub에서 주고 받는다

![](../다운로드1.png)

## + 용어 정리

mkdir + 폴더이름 : 폴더 만들기
start . : 폴더 열기, 
touch + 문서이름 : 문서만들기, 
cd + 문서 : 문서로 이동
ls : 현재 위치에 뭐 있는지 보기
git init : 현재 위치의 마스터권한 갖기
수정 + 저장
git add . 
git add +문서이름
git commit -m '메시지'
git status
git log
git log --oneline
git checkout 해쉬값
git checkout master
git clone
git push origin master
git pull origin master

---

local과 hub가 서로 다른 구슬을 생성할 경우 collide(충돌)이 나타날 수 있다. 그러면 push할 때 파일이 reject된다.

그럴 경우 pull origin master를 사용해서 파일을 선택하든지 합병하든지 해서 하나로 통합한다. 그 후에 add . 와 commit 해주고 push 해주면 충돌이 해결된다.

---

gitignore : 무시하는 방법

1. touch . gitignore (ignore파일을 생성한다)

2. 무시할 파일들을 생성한다.

3. or https://www.toptal.com/developers/gitignore/ 로 접속해서 사용하는 언어를 검색해서 붙여넣는다.

4. gitignore 는 git 으로 관리될 파일들 중에서

   관리를 하지 않을 파일을 등록하는 블랙리스트 개념의 파일입니다.

   이미 git commit 으로 한 번 관리가 되고 있는 파일을 뒤늦게 .gitignore에 작성을 하게 된다면 블랙리스트로 동작을 하지 않게 됩니다.

   - git 으로 제외하려는 파일을 `git rm -rf --cached 파일명` 으로 명령어를 실행하고 add commit push 해주시면 정상적으로 git으로 관리목록에서 제외되게 됩니다.
   
   ---
   
   ![](../다운로드.png)

---

## pull request

1. 방을 판다 (add readme 추가해서)
2. 주소를 복사해서 git clone해서 파일생성, 코드로 열기
3. 브랜치를 생성한다
4. 브랜치에서 작업한다.(수정, 저장 add, commit)
5. git push origin 브랜치명 : 을 통해 hub 브랜치를 생성
6. hub에서 pull-request를 해준다.
7. merge pull request 버튼 클릭
8. confirm merge 승인해!
9. local에서 master로 switch 해준다.
10. git pull origin master 해주면 local master에서 변경사항 받을 수 있다.

---

## 깃허브에서 다운받아 pull request

1. 원하는 파일을 fork한다. 
2. 내 repository로 가져온다
3. 복사한다
4. git bash에서 git clone 주소 붙여넣기 한다
5. vscode 열어서 branch생성하고 
6. branch로 switch한다.
7. 수정, 저장, add, commit 
8. git push origin branch명 입력! 
9. hub에 pull request가 생성된다. 
10. pull request 누르면 끝!


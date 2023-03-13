# task

## 과제방에 repo 주소로 업로드

1. task repository 포크로 본인 repository에 복사
2. 내려 받기해서 해당 README.md 문서 수정
3. 오늘까지 배운 git 내용 마크다운 형식으로 __잘__ 정리
  _markdown-cheetseat 참고_
4. 본인 repository에 업로드
5. 로컬 저장소 내용도 캡쳐해서 함께 업로드

이 아래로 내용 작성

![picture alt](https://ibb.co/gjL3H90.jpg)

# 230310 배운 내용 #


### 로컬저장소와 github연결 ###

1. github에 Repository를 생성
2. 로컬 저장소에 git을 연결
3. git remote add origin __URL__ 로 github와 연결

  - - - -

### 로컬저장소와 github   __PUSH__ ###

1. 파일 수정 및 저장
 * 한번도 commit을 하지 않았다면 git add. 후에 git commit -m " __메세지__ "
 * 한번이라도 저장을 했다면 git gommit -am " __메세지__ "

2.로컬 저장소에서 github으로 push
 * 메인이라면 git push -u origin main
 * 브런치라면 git push origin __브린치__

  - - - -

### 로컬저장소와 github   __PULL__ ###

1. github에서 Fork
2. code에 있는 링크 복사
3. git에 링크를 입력
     * 폴더 생성되어 있다면 git clone __URL__
     * 폴더 생성이 되지않았다면 git clone __URL.__
 - [x] git 파일이 없어야 가능

  - - - -

### github에서 파일 삭제와 충동 ###

  > 1. github에서 파일 방법
  >> 1. github 파일 settings
  >> 2. danger zone에서 Delete this repository

  > 2. github파일 충돌 (같은 이름의 파일의 경우)
  >> 1. github의 파일 삭제후 로컬에 있는 같은 파일을 다시 연결할 경우 같은 이름, 같은 파일 경우 충돌
  >> 2. git remote rm origin
  >> 3. 오류가 해결되었는지 git config --list를 통해 확인 (git remote __URL__이 없다면 삭제 완)
  >> 4. 오류가 없다면 다시 연결 가능

  - - - -

## 그 외의 명령어 ##
  > 브런치 옮기기
  >> git switch __브런치__

  > 삭제 된 파일 복원
  >> git restore __파일명__ . __확장명__

  > 작업 내용 전부 그래픽
  >> git log --oneline --graph --all

  > commit 메세지 수정
  >> git commit --amend -m " __메세지__ "

  > 브린치 합치기 (명령어 입력 위치 중요)
  >> git merge __브린치이름__

  > 빈 브린치 삭제
  >> git branch -d __브린치이름__

  > 파일 있는 브린치 삭제
  >> git branch -D __브린치 이름__
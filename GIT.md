#GIT 정리
***

&nbsp;
## 1. git 기본 단축키
- ```Ls``` : 목록
- ```mkdir``` : 디렉토리 생성
- ```cd``` : 디렉토리 이동
- ```cd ..``` : 현재 디렉토리에서 상위 디렉토리로 이동
- ```touch``` (파일명)(확장자) : 새로운 파일을 생성
- ```rm 파일명``` : 파일 삭제
    - 단, 파일 내 다른 파일이 있을 경우 directory라는 문구가 뜨며 삭제되지 않습니다. 이 경우에는 ```rm -r (파일명)```를 하면 됩니다.
- ```pwd``` : 현재 디렉토리 출력.

&nbsp;
## 2. git 만드는 법
1. 폴더와 깃을 같이 엽니다. 
2. ```git init```를 입력하면 ```(master)``` 상태가 되며 ```.git``` 폴더가 생깁니다.
    - .git은 숨김 폴더기에 ls해도 보이지 않으며, cd .git을 한다면 오류가 납니다.

&nbsp;
## 3. add와 commit을 이해하기
- 깃은 임의로 3가지 공간으로 나눌 수 있습니다(실제로 나뉘는 것은 아니며 이해를 돕기 위함입니다).

    1. ```Working Directory``` : 변경사항이 생긴 파일이 모여있는 곳입니다.

        이 상태의 파일을 ```Untracked```라고 부릅니다.

        다음 단계로 넘어가려면 ```git add (파일명)```을 입력합니다. 
        
    2. ```Staging Area``` : 버전(```커밋```)으로 기록하기 위해 모인 파일들의 목록입니다.

        다음 단계로 넘어가려면 ```git commit -m (파일명)```을 입력합니다.

         이 상태의 파일을 ```Staged```라고 부릅니다.
         
    3. ```Repository``` : 커밋된 파일들이 기록되는 곳입니다.

        이 상태의 파일을 ```commitied```라고 부릅니다.

&nbsp;

##

4. 기타
    - Working Directory, Staging Area의 파일 목록을 확인하려면 ```git status```를 입력합니다. 그리고, 저장소에 기록된 커밋을 조회하려면 ```git log```를 입력합니다.
    - commit을 할 때 글로벌 유저 이메일과 이름을 설정해야합니다.

        글로벌 이메일 : git config --global [user.email]http://user.email

        글로벌 유저 이름 : git config --global [user.name]http://user.name

        &nbsp;

***

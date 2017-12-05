정리 !
git commit --amend
: 가장 최근 commit을 수정할 수 있다.
git add file1.txt //변경한 후 add했다고 가정
git commit --amend 
//하면 저것까지 최근 commit에 포함하여 들어감

git reset HEAD <파일>
 staged ==> unstaged상태로 변화
 git reset HEAD file1.txt

git checkout -- <파일>
 unstaged 변경상태 취소
 git checkout -- file1.txt

 git rm --cached <file>:
이미 commit된 파일을 Git의 관리대상에서
제외함.
.gitignore에 패턴을 추가하는 것을 빼먹고 이미 파일을
commit한 경우 사용하면 됨
-------------------------------------------
다른 점이 있다면 cp는 파일을 복사하는 것이고 mv는 파일 이동인데 이동 시 원본 파일이 삭제되는 점이다
mv file1.txt fileA.txt

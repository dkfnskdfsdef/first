# HTML
## Hyper Text Markup Language
### HTML은 웹문서의 구조를 담당하는 언어이다.
* HTML에서 구조는`<>` 로 묶인 태그로 작성한다.
* `<시작태그></닫기태그>`
* `<빈태그>`
* 시작과 닫기태그는 한쌍의 요소로 불린다.
### HTML 구조태그
* HTML5 버전 선언하는 `<!doctype html>`
* HTML 웹브라우저 구조 처리하는 태그들
1. `<html></html>`
2. `<head></hesd>`
3. `<body></body>`
----
# git&gitHub
* 버전관리 프로그램 git
* 버전 파일, 폴더들을 저장하는 저장소 gitHub
## git 용어와 뜻
* 작업 디렉터리 : 실제 작업하는 로컬 저장소(윕도우 탐색기 개념)
* 스테이징 :갓허브에 작어버업로드 전 파일을 대기시키는 대기소
* repository : 대기소(stage)에 파일 대기 후 최종 gitHub 업로드 저장소
## 주의사항
* 당일 자업 시작 기준 gitHub 저장소와 로컬저장소의 파일, 폴더 상태가 같아야한다.
* 동일한 저장소를 관리하는 사람일 경우 작업 컴퓨터가 달라도
gitconfig에 등록된 이름, 이메일이 동일해야 한다.
----
# 주요 단축키 모음
* `ctrl + /` 한중 주석
* `shirf + alt + a` 선택한 영역만 주석
----
# 처음 git을 이용한 gitHub 저장소 업로드 시 해야하는 순서
1. 현재 사용중인 로컬 저장소를 git 저장소로 등록 `git init`
2. 위 1번 정상 등록 시 경로에 (master) 표시출력
3. master -> main으로 최상위 경로명칭을 변경하기 위해 `git branch -m main` 작성
4. gitHub 저장소 생성 후 저장소 주소 복사
5. 현재 로컬 저장소 gitHub 저장소 연결 `git remote add origin 주소붙여넣기`
6. `git status` 현재 상태 확인(스테이징, 작업디렉터리, 저장소)
7. 위 6번 결과 파일이 빨강색으로 출력될 경우 `git add 파일명` 스테이징 올리기
8. `git status` 위 7번에서 올린 파일이 초록색으로 변경된 걸 확인
9. `git commit -m '기록메세지'` 스테이징 파일을 저장소에 올리기 위한 기록설정
10. `git push origin main` 깃허브 저장소에 최종 파일, 폴더 업로드
11. 위 10번 처음 진행 시 깃허브 계정 인증 화면나오니 인증 진행 후 저장소 f5
----
## 다른 환경에서 이어서 작업해야 하는 경우
1. 폴더 생성하기 -> vs code 폴더 연결
2. gitHub 저장소 주소 복사
3. vs code 돌아와서 ctrl + j 터미널 실행 후 bash 환경 변경
4. `git clone 주소붙여넣기`
5. 터미널 경로 오른쪽에 `main` 또는 `master` 표시가 있는지 확인
6. 위 5번에서 표시가 없다면 `cd 복제한폴더명`
7. 자유롭게 수정 후 파일 저장
8. 터미널에 `git status` 업로드 안된 파일 빨강색 색 확인
9. `git add 파일명` 수정한 파일 스테이지에 업로드하기
10. `git status` 위 9번 업로드 됐는지 확인(초록색 변경)
11. `git commit -m '메세지'` 수정 파일에 대한 기록 메세지 작성
12. `git push origin main` 깃허브 저장소에 업로드
## HTML & meta
* HTML : 웹 페이지에서 다른 페이지로 이동할 수 있도록 웹 브라우저에게 명령을 내리는 구조적 문서를 만드는 언어
* meta : 브라우저에는 보이지않는 태그. (예) <meta charset=”utf-8”><meta name=”description” content=””><meta name=”keywords” content=”관련된 키워드”>
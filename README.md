# Today I Learned
> 매일매일 배운 것을 기록합니다.

## 2022-09-13
### RPA 1기, 웹프로그래밍 기획과 기본
#### 리눅스 커맨드라인 기초
- `pwd` : print working directory. 현재 작업 경로 출력
- `cd` : change directory. 현재 작업 경로를 변경할 때 사용
  - 절대 경로는 /로 시작함
  - 상위 경로는 ..으로 나타냄
  - tab키 사용시 자동 완성 기능
- `ls` : list. 현재 작업 경로에 있는 모든 파일, 디렉터리 출력
  - `ls -a`, `ls -l`, `ls -al` 등의 옵션 추가 가능
- 'history' : 과거에 쳤던 명령어 리스트를 보여줌
  - 8번째 명령어를 복구하고 싶으면 !8
  
#### vim 사용법
- 명령 모드와 입력 모드
  - vim에디터를 열 때는 명령 모드로 진입함
  - 명령 모드에서는 입력 불가
  - 입력하려면 `i`를 눌러 입력 모드로 전환
  - 입력 완료 후 저장하려면 `esc`를 눌러 명령 모드로 전환
  - 입력 가능한 명령어
    - `:w` : 저장/write
    - `:q` : vim에서 나오기/quit
    - `:wq` : 저장하고 나오기
  - 참고자료 [링크](https://velog.io/@717lumos/Vim-Vim-editor-%EC%82%AC%EC%9A%A9%EB%B2%95)
- 비정상적으로 종료시 해결 방법
  - vim이 비정상 종료되었을 때`swp` 파일이 생성됨
    - ATTENTION 문구가 뜨는 경우
      1. 두 프로세스, 두 사람이 동시에 한 파일을 수정하는 경우
      2. crash가 나서 vim이 비정상적으로 닫힌 경우
  - 기존에 입력했던 내용을 복구하고 싶을 때는 `vim -r 파일명`을 입력하거나 Recovery모드로 진입
  - 정상 종료 후, `swp` 파일 삭제
    - `rm .789.text.swp` <-- `rm` 명령어는 remove

#### 마크다운 문법
- 링크 추가
- * 외부링크
```
사용문법: [Title](link)
적용예: [Google](https://google.com, "google link")
```
Link: [Google](https://google.com, "google link")
- [링크](https://gist.github.com/ihoneymon/652be052a0727ad59601)


#### 버전 관리 시스템과 git

##### 버전 관리 시스템을 사용하는 이유
1. 실행 취소, 재실행기 가능함
2. 버전간 소스코드 비교가 가능함
3. 협업이 쉬워짐

##### 다양한 버전관리 방법
이름 변경하기 등의 방법이 있는데, 개발할 때는 git을 주로 사용함

##### 커밋
- 커밋은 논리적 변경이 있을 때 만듦
- 가능하면 커밋 크기가 작을수록 좋음
- 커밋 이력보기: `git log'

##### 리포지토리
- 정의: 여러 파일을 하나로 모은 컬렉션
- 일반 디렉터리와 리포지토리의 차이: `.git` 디렉터리 유무

- `rm -rf` : 해당 git 전부 삭제 (r=recrusuive, f=force)
- 캐시 = 임시저장
- git k, git 크라켄

### 저장소 상태 파악하기



## 2022-09-20

#### 브랜치
- 정의: A branch in Git is simply a lightweight movable pointer to one of these commits.
- 브랜치는 특정한 목표를 가지고 코드를 수정할 때 주로 만듦
  - 이슈 하나당 브랜치 하나를 주로 만듦

##### 명령어
1. 브랜치 목록 보기
```
git branch
```

2. 브랜치 생성하기
```
git branch 브랜치이름
```

3. 특정 브랜치로 전환하기
```
git checkout 브랜치이름
```
or
```
git switch 브랜치이름
```
4. 브랜치 생성과 체크아웃 동시에 하기
```
git checkout -b 브랜치명
```

테스트092701
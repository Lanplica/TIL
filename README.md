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

#### 마크다운 문법
- 링크 추가
- [링크](https://gist.github.com/ihoneymon/652be052a0727ad59601)
- * 외부링크
```
사용문법: [Title](link)
적용예: [Google](https://google.com, "google link")
```
Link: [Google](https://google.com, "google link")

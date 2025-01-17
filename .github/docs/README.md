## 목차
  - [1. 브랜치 전략](#1-브랜치-전략)
  - [2. 커밋 규칙](#2-커밋-규칙)
  - [3. issue 스타일 가이드](#3-issue-스타일-가이드)
  - [4. pull request 스타일 가이드](#4-pull-request-스타일-가이드)

<br>

## 1. 브랜치 전략
- 브랜치는 `feature/#이슈번호-설명간단히(영문)` 으로 생성한다.
```
feature/#이슈번호-간략한설명(영문)
ex) feature/#24-SecondView
```

<br>

### 1-1. 브랜치 규칙
```
1. develop, main 브랜치에서의 작업은 원칙적으로 금지한다.
2. 자신이 담당한 부분 이외에 다른 팀원이 담당한 부분을 수정할 때에는 반드시 변경 사항을 전달한다.
3. 본인의 Pull Request는 본인이 Merge한다.
4. Commit, Push, Merge, Pull Request 등 모든 작업은 앱이 정상적으로 실행되는 지 빌드한 후 수행한다.
```

### 1-2. 브랜치 플로우
```
1. Issue를 생성한다.
2. feature 브랜치를 생성한다.
3. feature 브랜치 내부에서 Add - Commit - Push - Pull Request 의 과정을 거친다.
4. Pull Request가 작성되면 충돌 확인 후 merge 한다.
5. 종료된 Pull Request branch는 삭제한다.
```

<br>

## 2. 커밋 규칙
```
- feat: 새로운 기능 추가
- fix: 버그 수정
- docs: 문서 수정
- style: 코드 formatting, 코드 변경이 없는 경우
- refactor: 코드 리팩토링
- test: 테스트 코드, 리팩토링 테스트 코드 추가
- chore: 빌드 업무 수정, 패키지 매니저 수정
```

<br>

## 3. Issue 스타일 가이드
### Feature Issue
```
---
name: Feature
about: 기능 추가시 작성해 주세요
title: "[Feat] "
labels: enhancement
assignees: ''

---

## Description
무슨 기능인지 간단히 작성해 주세요

## TODO
할 일 목록을 작성해 주세요

- [ ] 

## ScreenShot
추가할 기능의 스크린샷이 있다면 첨부해 주세요

### ETC
기타 참고사항을 작성해 주세요
```

<br>

### Bug Issue
```
---
name: Bug
about: 버그 발생시 작성해 주세요
title: "[Fix] "
labels: bug
assignees: ''

---

## Problem
무슨 문제인지 간단히 작성해 주세요

- [ ] 

## How to Solve
어떻게 해결했는지 작성해 주세요

- [ ] 

### ETC
기타 참고사항을 작성해 주세요
```

<br>

## 4. Pull Request 스타일 가이드
아래 템플릿을 따르고 있습니다.
```
## 개요
<!---- 변경 사항 및 관련 이슈에 대해 간단하게 작성해주세요. 어떻게보다 무엇을 왜 수정했는지 설명해주세요. -->

<!---- Resolves: #(Isuue Number) -->

## PR 유형
어떤 변경 사항이 있나요?

- [ ] 새로운 기능 추가
- [ ] 버그 수정
- [ ] CSS 등 사용자 UI 디자인 변경
- [ ] 코드에 영향을 주지 않는 변경사항(오타 수정, 탭 사이즈 변경, 변수명 변경)
- [ ] 코드 리팩토링
- [ ] 주석 추가 및 수정
- [ ] 문서 수정
- [ ] 테스트 추가, 테스트 리팩토링
- [ ] 빌드 부분 혹은 패키지 매니저 수정
- [ ] 파일 혹은 폴더명 수정
- [ ] 파일 혹은 폴더 삭제

## PR Checklist
PR이 다음 요구 사항을 충족하는지 확인하세요.

- [ ] 커밋 메시지 컨벤션에 맞게 작성했습니다. Commit message convention 참고 (Ctrl + 클릭하세요.)
- [ ] 변경 사항에 대한 테스트를 했습니다. (버그 수정/기능에 대한 테스트)

```

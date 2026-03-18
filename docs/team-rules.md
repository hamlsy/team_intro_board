# 📜 Team Rules

## 1. Git Workflow

- ❌ main 브랜치 직접 push 금지
- ✅ 모든 작업은 feature 브랜치에서 진행
- ✅ 작업 전 반드시 Issue 생성
- ✅ PR(Pull Request) 후 merge 진행

---

## 2. Branch Strategy

- 브랜치 네이밍 규칙
feature/이슈번호-작업내용


예시:
- feature/1-gangnam-restaurants
- feature/2-member-a
- feature/3-readme-update

## 2.1 Merge Flow
(feature) -> deploy -> main

deploy에서 분기 후 deploy로 merge,

추후 배포시 deploy->release->main

---

## 3. Commit Convention

- 모든 커밋 메시지는 **이슈 번호 포함 필수**
[#이슈번호] type: 작업 내용 


### 타입 종류

- feat: 기능 추가
- fix: 버그 수정
- refactor: 코드 구조 개선
- docs: 문서 작업
- init: 초기 설정

### 예시


[#1] feat: 강남 맛집 리스트 추가 
[#5] docs: README 수정 
[#6] fix: 중복 데이터 제거


---

## 4. Issue Rule

- 모든 작업은 Issue 기반으로 진행
- 하나의 Issue = 하나의 작업 단위


## 5. Pull Request Rule

- 최소 1명 이상 리뷰 필수
- PR 제목은 commit convention과 동일하게 작성

예시:

[#12] feat: 강남 맛집 리스트 추가 


- 리뷰 승인 후 merge 진행

---

## 6. Merge Strategy

- squash merge

### 기본 원칙

- 개인 브랜치 → rebase 가능
- 여러 명이 작업하는 브랜치 → merge 권장

---

## 7. Remote Sync Rule

- ❌ git pull 사용 금지
- ✅ git fetch 후 직접 merge 또는 rebase 수행


git fetch origin
git rebase origin/main


또는


git fetch origin
git merge origin/main


---

## 8. Conflict Handling

- 충돌은 협업 과정에서 자연스럽게 발생하는 것
- 충돌 발생 시:
  1. 변경 내용 확인
  2. 팀원과 협의 후 수정
  3. 충돌 해결 후 commit

---

## 9. Documentation Rule

- 모든 결과물은 docs 폴더에 정리
- 작업 내용은 changelog.md에 기록

---

## 10. Goal

- Git 협업 흐름 이해
- PR & 코드 리뷰 경험
- merge vs rebase 차이 이해
- 충돌 해결 경험

---
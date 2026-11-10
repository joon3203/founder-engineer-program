# Git / GitHub 작업 흐름

## 최초 시작 (macOS)
```bash
git clone https://github.com/joon3203/founder-engineer-program.git
cd founder-engineer-program
python3 --version
git status
```

## 과제 제출
```bash
git switch -c exercise/<short-name>
# 직접 코드 작성, 로컬 테스트
git add exercises/ challenges/
git commit -m "learn: implement <topic>"
git push -u origin exercise/<short-name>
```
GitHub에서 Pull Request를 열고 코드·테스트·궁금한 점을 설명한다.

## 주의사항
- `main`에는 검토된 코드만 병합한다.
- 비밀번호, API 토큰, 고객 정보, 로컬 DB는 절대 커밋하지 않는다.
- `git status`로 변경사항 확인 후 `git add` 한다.
- 쉬운 연습 단계에서는 브랜치가 부담되면 직접 커밋해도 되지만, 프로젝트부터는 PR을 권장한다.
- GitHub 연결에 따라 튜터가 코드/PR을 읽을 수 있다. 자동 테스트·로컬 실행 결과는 별도 확인한다.

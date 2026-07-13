# Description
**[한글]**<br/>
팀 또는 전사적으로 Git Commit message와 Pull Request 내용 포맷을 공통화 하기 위한<br/>
Git commit message, PR 내용 생성 스킬 입니다.

**[En]**<br/>
This skill automatically generates Git commit messages and Pull Request (PR) templates to standardize formats across teams or the entire company.

***

# Install
**For Claude** — commit-pr-generator.skill: Install directly using the "Save skill" button on the file card. For Claude Code, you can also unzip it into ~/.claude/skills/.

**For Codex** — commit-pr-generator-codex.zip: Install by running the following commands:
```bash
mkdir -p ~/.codex/skills
unzip commit-pr-generator-codex.zip -d ~/.codex/skills/
```

To use it on a per-project basis, extract it to .codex/skills/ within your repository. Since Codex also auto-loads skills based on descriptions, it will work exactly the same way when you request something like "Create a commit message."

# Rules
```
- 반드시 현재 워크트리를 더럽히는 코드 수정이나 파일 생성 행위를 하지 말것
- 또한 git 워크트리가 깨끗하다면 최근 commit 내역 기준으로 변경/추가 이력을 집중해서 분석해서 결과를 만들어낼것

# 결과
1. (워크트리가 존재 한다면) git commit message 생성
  -  message format : [{feat | refactor | etc...}] {number. message}
2. Pull Request 내용 생성 (제목과 내용)

# 사고 과정
- 커밋 메시지 포맷 number는 변경 항목 순번
- 커밋 메시지와 PR 내용의 언어 가급적 한글
- PR 내용에 포함할 섹션은 '요약 + 변경사항', '영향 범위'
```

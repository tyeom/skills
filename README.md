# Skills
Public AI agent skills by [tyeom(arooong)](https://github.com/tyeom).

# Available Skills
### `commit-pr-generator`
This skill automatically generates Git commit messages and Pull Request (PR)<br/>
templates to standardize formats across teams or the entire company.

# Install
If your AI agent supports skills, you can point it at the GitHub URL for a skill and ask it to install that skill:

```
Install the AI agent skill at https://github.com/tyeom/skills/tree/main/commit-pr-generator
```
You can also clone this repo and copy a skill folder into your agent's skills directory. Adjust the destination path for your agent
this example uses Codex's default skills folder:

```
git clone https://github.com/tyeom/skills.git
cd skills
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
cp -R commit-pr-generator "${CODEX_HOME:-$HOME/.codex}/skills/"
```

# License
MIT

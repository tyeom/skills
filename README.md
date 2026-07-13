# Skills
Public AI agent skills by [tyeom(arooong)](https://github.com/tyeom).

# Available Skills
### `commit-pr-generator`
This skill automatically generates Git commit messages and Pull Request (PR)<br/>
templates to standardize formats across teams or the entire company.

# Install
If your AI agent supports skills, you can point it at the GitHub URL for a skill and ask it to install that skill:

```
Install the AI agent skill at https://github.com/tyeom/skills/tree/main/codex-dynamic-workflows
```
You can also clone this repo and copy a skill folder into your agent's skills directory. Adjust the destination path for your agent; this example uses Codex's default skills folder:

```
git clone https://github.com/DannyMac180/skills.git
cd skills
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
cp -R codex-dynamic-workflows "${CODEX_HOME:-$HOME/.codex}/skills/"
```

Then start a new agent session and invoke it with:

```
Use $codex-dynamic-workflows to plan and run a supervised multi-agent workflow for this task: ...
```

# License
***
MIT

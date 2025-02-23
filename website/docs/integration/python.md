# Python

For Python projects, **git-cliff** can be configured in `pyproject.toml` via the [tool table](https://peps.python.org/pep-0518/#tool-table). To do this, simply replace the available configuration sections with `[tool.git-cliff.<section>]` and place them inside `pyproject.toml`. For example:

```toml
name = "..."

[project]
dependencies = []

[tool.git-cliff.changelog]
header = "All notable changes to this project will be documented in this file."
body = "..."
footer = "<!-- generated by git-cliff -->"
# see [changelog] section for more keys
[tool.git-cliff.git]
conventional_commits = true
commit_parsers = []
filter_commits = false
# see [git] section for more keys
```

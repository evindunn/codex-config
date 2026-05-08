# ~/.codex/AGENTS.md

## Working agreements

**Global**
- When asked for a code review, always re-read the relevant files from disk before reviewing them

**Python**
- Don't ever edit files installed within a virtual environment
- If the project is Python and a `.venv` directory exists, use that virtual environment for Python commands and checks by default
- For functions, use the following docstring conventions
  - Simple functions for obvious cases must include a one-line docstring as described in https://peps.python.org/pep-0257/#one-line-docstrings
  - More involved functions must include a multi-line docstring following the Sphinx docstring format, as described in https://sphinx-rtd-tutorial.readthedocs.io/en/latest/docstrings.html
- Generate a Sphinx-style docstring for each generated class
- Use explicit module-qualified imports for Python packages. Prefer namespaced references like functools.cache and uuid.UUID over importing members directly.
- Imports should be sorted and belong to one of the following sections, which are separted by a blank line each: stdlib imports, installed imports, filesystem imports
- Constants should always be sorted and right below the imports, separated from them by a blank line

**YAML**
- Always use the .yml suffix when generating new files
- Leave an empty line between list items iif the list items are objects

**Shell**
- Always double quote strings with variable/command substitution. Always single quote strings without any.

**Markdown**
- Always make file links relative to the file where the reference occurs

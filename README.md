# Cosplay Coding

Cosplay coding is a phenomenon that emerged after vibe coding gained popularity.
It describes the situation when contributors submit code that looks like it works but in reality does not.

## Characteristics

Cosplay code can take different forms:

- Copy-paste feel: code looks like it was generated or pasted from somewhere else, with no adaptation to the actual
project context.
- Unused imports / dead code: extra functions, imports, or variables that are never called or referenced
- Inconsistent naming: variables, methods, or classes that don’t follow project conventions, suggesting no attempt
to understand the style or standards.
- Low-effort fixes: only addressing linters/formatters or renaming variables, without meaningful contribution
to functionality.
- No integration awareness: code may work in isolation but breaks as soon as it interacts with the rest of the
application (database, APIs, services).
- Code that does not even pass quality checks (linters, formatters, CI) and contains no tests.
- Tests that pass only because they are mocked incorrectly or do not cover integration scenarios.
- Code that technically passes automated checks.
- Code that includes tests, which appear to be green.

On the surface, these may look like valid contributions.

## The Problem

When integrated into a real application, cosplay code fails.
Common reasons include:

- Missing attributes (for example, the AI or contributor assumed they existed).
- Wrong assumptions about database tables or ORM structure.
- Incorrect function signatures (wrong number or type of arguments).
- Logic that compiles but does not function in real-world usage.

This indicates that the code was never actually run in the intended environment.
Instead of genuine effort to improve the project, the goal often seems to be:

- Getting a PR reviewed and merged quickly.
- Gaining contribution credit without meaningful impact.

## Impact

- Maintainers' time is wasted reviewing and debugging non-functional contributions.
- The project's quality and credibility suffer.
- It creates noise that drowns out meaningful contributions.

## Takeaway

Cosplay coding highlights the need for contributors to run and validate their code in real scenarios, not just
rely on passing automated checks. Responsible contributions mean ensuring functionality, not just appearances.

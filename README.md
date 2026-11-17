# world-spring

The realms of Embabel for Spring, as a world other worlds inherit from.

> **Experimental.** The list and the realms in it are new and still changing. Check answers before relying on them.

A world that names this one in its `config/world.yml` gets every realm listed in `config/realms.yml`,
and keeps getting them as the list changes:

```yaml
extends:
  - embabel-worlds/world-spring
```

Realms a world adds in its own `config/realms.yml` load beside these.

## What is in it

| Realm | What it reads |
|---|---|
| `which-change` | Joins the rest: a failure in the logs to the line, the commit, its author and the pull request |
| `jvm-logs` | Java log files: exceptions, stack traces, failures grouped |
| `polyglot-code`, `code-model` | The repository's files, classes and methods, at a commit |
| `git` | Commits, blame and line history, from a clone |
| `github` | Pull requests and reviews |
| `kubernetes` | Pods, the version each runs, restarts and crash reasons |
| `dev-vocabulary` | The types the others share |

Nothing is installed in the application being examined, and nothing is copied out of the systems read.

To start a new world from this list, use [world-spring-starter](https://github.com/embabel-worlds/world-spring-starter).

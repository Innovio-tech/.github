# Contributing to Innovio repositories

Every Innovio repository follows the same workflow:
[engineering-standards/standards/git-workflow.md](https://github.com/Innovio-tech/engineering-standards/blob/main/standards/git-workflow.md).

In short:

1. Branch from `main`: `feature/short-description` (with the ticket key where the product has a
   tracker: `feature/MKT-123-short-description`).
2. Commit subjects: imperative, at most 72 characters (`[MKT-123] ` prefix with a tracker).
3. `./run.sh hooks` once per clone; `./mvnw clean verify` before every push.
4. Open a pull request, fill the template, get one approval, squash merge.

A repository's own `CONTRIBUTING.md`, when it has one, adds what is specific to it.

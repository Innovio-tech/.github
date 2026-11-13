# Contributing to Innovio repositories

The rules live in [engineering-standards](https://github.com/Innovio-tech/engineering-standards) (members only);
this page is the short version. A repository's own `CONTRIBUTING.md` adds to it.

1. **Branch** from `main`: `<type>/<short-description>`, for example `feat/household-invites` or
   `fix/login-validation`. Types: `build`, `chore`, `ci`, `docs`, `feat`, `fix`, `refactor`, `test`. A tracker key in
   the description is optional.
2. **Commit** with a Conventional Commits subject, `<type>[(scope)][!]: <description>`, at most 72 characters, in the
   imperative. Add a body when the why is not obvious. Commits carry their human author only.
3. **Check locally** what the repository's README names before pushing (its build and tests, and the hooks set up
   once per clone where it has them). New behaviour starts as an OpenSpec change in the repository that owns it.
4. **Open a pull request** with the template. One concern per pull request; its title is a Conventional Commits
   subject and becomes the squash commit.
5. **Review and merge**: one approval from someone other than the author, conversations resolved, required checks
   green, squash merge. Code owners review where the repository has `CODEOWNERS`.

Never commit secrets, keys or `.env` files. A security problem is reported privately: see [SECURITY.md](SECURITY.md).

Details: engineering-standards `standards/git-workflow.md` (branches, commits, pull requests, review) and
`standards/testing.md` (definition of done).

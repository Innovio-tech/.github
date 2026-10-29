## Ticket

<!-- The tracker link when the product has one (the PR title carries the key), otherwise "none" -->

## What changed and why

<!-- What the change does, and the reason. Link the flow / ADR it implements. -->

## Scope

- Flow(s): <!-- e.g. docs/flows/08-create-listing.md, or "none" -->
- Spec: <!-- e.g. docs/spec/entities/02-household.yaml, or "none" -->
- Clients affected: <!-- Web / iOS / Android / none -->

## How it was tested

<!-- Tests added or changed, and what you ran locally -->

## Checklist

Definition of done: [engineering-standards/standards/testing.md](https://github.com/Innovio-tech/engineering-standards/blob/main/standards/testing.md#definition-of-done)

- [ ] PR title is `[KEY-123] Short description` (product with a tracker) or `Short description`, at most 72 characters
- [ ] `./mvnw clean verify` passes locally
- [ ] Tests added or updated (bug fix → regression test; another user's or tenant's data → 404)
- [ ] No secrets, `.env`, or personal data committed
- [ ] No blocking calls in the request path (no `.block()`, JDBC, `RestTemplate`)

## Contract and docs — tick what applies, delete the rest

- [ ] API changed → `docs/api/openapi.yaml` updated (spec in `docs/spec/` first)
- [ ] Breaking API change → called out below and agreed with the client teams
- [ ] Schema changed → new Liquibase changeset (existing ones untouched)
- [ ] New config → `.env.example` updated
- [ ] New error code → error catalogue, `ErrorCode` and `openapi.yaml` updated
- [ ] Architecture decision → new or updated ADR in `docs/architecture/adr/`
- [ ] Behaviour differs from `docs/flows/` → flow doc updated
- [ ] Differs from engineering-standards → an ADR in this repository says why

## Breaking changes / notes for reviewers

<!-- "None" if none -->

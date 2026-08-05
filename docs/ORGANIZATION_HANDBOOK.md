# OmniBlitz organization handbook

> Organization-wide defaults for repositories maintained under **OmniBlitz**. A repository may strengthen these rules locally, but should not silently weaken them.

## Mission and scope

OmniBlitz maintains omnichannel campaign, publishing, and delivery automation. The `.github` repository is the canonical home for the organization profile, contribution policy, security guidance, support expectations, reusable templates, and planning links.

## Repository expectations

Every active repository should clearly document its purpose, ownership boundary, supported environments, maturity, reproducible development and test commands, authoritative interfaces and schemas, release and rollback behavior, compatibility guarantees, and links to relevant GitHub Project and Linear work.

Campaign and delivery components should also document channel capabilities, provider limits, retry and idempotency behavior, scheduling semantics, data-retention expectations, and degraded-mode behavior.

## Change workflow

1. Start from an issue, Linear item, or documented maintenance objective.
2. Keep branches and pull requests focused.
3. Explain motivation, scope, risk, validation, compatibility impact, migration, and rollback.
4. Run the narrowest relevant checks plus organization conformance checks.
5. Resolve conflicts semantically by preserving compatible intent from both sides.
6. Prefer squash merges for focused changes unless commit structure materially aids auditability.

## Quality and delivery evidence

Pull requests should include reproducible commands, environments, expected and observed outcomes, failure-path coverage, documentation changes, and CI or local-equivalent evidence. Breaking changes require explicit versioning, consumer impact analysis, migration guidance, and rollback.

## Security and data handling

Never commit credentials, provider tokens, customer data, private keys, or sensitive logs. Report vulnerabilities privately according to `SECURITY.md`. Pin dependencies, actions, containers, and generated inputs where reproducibility or supply-chain integrity matters.

## Documentation and decisions

Keep examples executable, links current, assumptions explicit, and repository boundaries unambiguous. Record architectural, provider, protocol, compatibility, privacy, and operational decisions that future maintainers would otherwise have to rediscover.

## Planning and status

GitHub is the source of truth for code, reviews, checks, releases, and delivery evidence. Linear is the source of truth for priorities, dependencies, sequencing, and cross-project planning. The organization GitHub Project provides the cross-repository execution view. See `PROJECTS.md` for routing details.

## Organization health checklist

- [ ] The profile accurately describes the organization and repository boundaries.
- [ ] Contribution, security, support, governance, issue, and PR guidance is present.
- [ ] Active repositories have owners, descriptions, topics, and maintained READMEs.
- [ ] Required checks match current delivery and security risk.
- [ ] Stale repositories are archived or clearly marked.
- [ ] GitHub Project and Linear links resolve and reflect completed work.
- [ ] Shared workflows and templates are versioned, tested, and backwards compatible.
